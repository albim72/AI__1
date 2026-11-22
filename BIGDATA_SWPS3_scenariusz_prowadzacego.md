# Big Data i Data Science na SWPS — scenariusz prowadzącego

**Do paczki BIGDATA_SWPS3.** Cytaty możesz powiedzieć grupie wprost. Wyniki pod nagłówkiem „Dla Ciebie” zachowaj na omówienie. Wszystkie liczby dotyczą plików dołączonych do warsztatu.

## Otwarcie zajęć

> Wyobraźcie sobie, że po tych zajęciach ktoś kładzie przed wami raport i mówi: „Na tej podstawie jutro przesuwamy budżet”. O co zapytacie, zanim zgodzicie się z rekomendacją? Zapiszcie jedno pytanie. Wrócimy do niego po ćwiczeniu o dwóch kanałach sprzedaży.

Poproś o rozpakowanie całego ZIP-a i otwarcie notebooka z końcówką STUDENT. Na ekranie pokazuj wersję studencką. W każdym bloku daj najpierw chwilę na przewidywanie wyniku, potem na obliczenia. Przy omawianiu poproś jedną parę o wynik, drugą o sposób jego sprawdzenia.

| Czas od początku | Co otworzyć | Pytanie do rozstrzygnięcia |
|---|---|---|
| 0–35 min | 01 · Sprzedaż i paliwo | Co wolno zsumować i co właściwie uśredniamy? |
| 35–70 min | 02 · CSV partiami | Jak policzyć wynik całego pliku przy ograniczonej pamięci? |
| 70–90 min | 03 · Dane do modelu | Co system wiedział w chwili decyzji? |
| 90–180 min | folder dotychczasowy_warsztat_Simpson, notebook 01 | Który kanał ma wyższą konwersję i od czego zależy odpowiedź? |
| 180–225 min | 04 · SQL | Jaki udział w obrocie regionu mają dwie największe kategorie? |
| 225–270 min | 05 · Model ryzyka | Ile nadużyć znajdziemy, jeśli sprawdzimy tylko 30 transakcji? |
| 270–315 min | 06 · Koszt decyzji | Kiedy opłaca się wszcząć kontrolę? |
| 315–360 min | 07 · Eksperyment z wielkością partii | Które ustawienie wybrać na tym komputerze? |

Przy **6 × 45 minut** kończysz po notebooku 05. Przy **6 × 60 minut** realizujesz również 06 i 07. Podane czasy oznaczają pracę z grupą, bez przerw.

## 01 · Sprzedaż i paliwo — 35 minut

**Jak zacząć**

> Dyrektor pyta, ile sprzedaliśmy. Otwórzcie plik sprzedaży, ale jeszcze niczego nie sumujcie. Popatrzcie na pierwszy wiersz. Czy to jest zamówienie, jeden produkt w zamówieniu, czy klient? Jak podpisalibyście liczbę wierszy w raporcie, żeby dyrektor dobrze ją zrozumiał?

**Jak poprowadzić**

1. **7 min.** Niech studenci otworzą `sales_cwiczenie.csv`, policzą wiersze i unikalne `line_id`. Pokażcie na jednym przykładzie, że klucz opisuje pozycję sprzedaży. Pytanie o liczbę zamówień wymagałoby identyfikatora zamówienia.
2. **10 min.** Poproś pary o sprawdzenie kopii, daty, ceny, rabatu i zgodności kwoty z ilością × ceną × (1 − rabat). Niech odłożą wiersze do wyjaśnienia i zachowają powód. Zapytaj, czy jeden rekord może naruszać dwie reguły.
3. **10 min.** Na pozostałych pozycjach liczą obrót i marżę, porównują średnią z medianą, układają ranking produktów i zestawienie miesięczne. Przy ujemnej marży zapytaj: „Jak mogła powstać poprawnie zapisana sprzedaż ze stratą?”.
4. **8 min.** Otwórzcie osobny plik `fuel.csv`. Zapytaj: „Trasa 10 km i trasa 500 km. Czy każda powinna mieć równy głos przy liczeniu spalania całej floty?”. Studenci liczą oba wskaźniki dla tras z dodatnim dystansem. Odkładają rekord z zerowym dystansem do wyjaśnienia.

**Dla Ciebie.** Na wejściu są 724 wiersze i 720 unikalnych pozycji. Cztery kopie oraz cztery zmienione rekordy dają 8 wierszy do wyjaśnienia. Zostaje 716 pozycji i **807 693,50 zł netto**. Liderem obrotu jest produkt A, a najwięcej poprawnych pozycji ma E. Dla paliwa średnia tras wynosi 8,196 l/100 km, a wskaźnik floty 8,192 l/100 km. Pierwszy waży każdą trasę tak samo, drugi nadaje każdemu kilometrowi tę samą wagę.

**Pytanie na wyjście.** „Wyniki spalania różnią się dopiero na trzecim miejscu po przecinku. Którego użyjecie, żeby oszacować litry potrzebne flocie na kolejny tysiąc kilometrów przy podobnym układzie tras? Dlaczego?”

## 02 · Analiza pliku partiami — 35 minut

**Jak zacząć**

> Załóżmy, że dostajecie plik większy od dostępnej pamięci. Mogę wam go podawać po kawałku. Po każdym kawałku musicie oddać pamięć. Jakie liczby zapiszecie sobie na kartce, żeby na końcu podać dokładny obrót i średnią cenę?

**Jak poprowadzić**

1. **5 min.** Otwierają pierwsze 5000 wierszy elektroniki, sprawdzają separator, przecinek dziesiętny i znaczenie ceny oraz wartości pozycji. Poproś, by podpisali wynik słowami „w pierwszych 5000 wierszy”.
2. **15 min.** Prześledźcie jedną iterację funkcji `aggregate_chunks`. Studenci uruchamiają ją na całym pliku dla partii po 17 003 wiersze. Mają pokazać, co zostaje po odrzuceniu partii: liczniki, sumy i agregaty kategorii. Kwoty sumują w całkowitych groszach.
3. **10 min.** Każda para porównuje trzy obliczenia: zwykłą średnią średnich partii, średnią cenę pozycji oraz cenę ważoną liczbą sztuk. Poproś o podpisanie mianownika każdego obliczenia.
4. **5 min.** Na dostarczonym pliku sprawdzają liczbę wierszy i obrót przez jednorazowy pełny odczyt. Wariant pięciomilionowy pozostaw jako rozszerzenie poza planem.

**Dla Ciebie.** Oczekuj **100 000 pozycji, 1 804 250 sztuk i 558 013 808 069 groszy**. Ostatnia partia ma 14 985 wierszy. Średnia cena pozycji to 3095,0505 zł, średnia średnich partii 3095,0794 zł, a cena ważona sztukami 3092,7743 zł.

**Gdy grupa utknie.** „W jednej partii macie jedną cenę 100 zł. W drugiej dziewięć cen po 10 zł. Ile wynosi średnia dziesięciu cen?” Wynik 19 zł łatwo sprawdzić w głowie. Zestaw go z 55 zł uzyskanymi przez uśrednienie dwóch średnich.

## 03 · Dane dostępne w chwili decyzji — 20 minut

**Jak zacząć**

> Jesteście systemem autoryzacji płatności. Zatrzymuję zegar w chwili, gdy klient płaci. Widzicie kwotę. A czy widzicie już, że za trzy dni dostanie zwrot? Otwórzcie listę kolumn i wskażcie, które naprawdę mogłyby być na ekranie w tej sekundzie.

**Jak poprowadzić**

1. **5 min.** Studenci dzielą pola na dostępne przy autoryzacji, powstające później i identyfikatory. Niech uzasadnią osobno każdą z tych decyzji: bieżąca kwota, wcześniejsze obciążenia zwrotne i późniejszy zwrot.
2. **8 min.** Sortują 3000 transakcji po czasie. Wcześniejsze 2400 służy do wyznaczenia median, skali i górnego progu kwoty. Późniejsze 600 przechodzi przez gotowe przekształcenie. Przy wolniejszej grupie wykonaj ten krok na ekranie.
3. **7 min.** Zanim zmienią kwoty w kopii testu na skrajne i dodadzą nowe urządzenie, poproś o przewidywanie: „Co może się zmienić w danych po przekształceniu, a jaki parametr ma zostać taki sam?”. Potem uruchamiają `transform` i sprawdzają.

**Dla Ciebie.** Próg 99,5. percentyla z treningu to ok. **1953,43**. Po zmianie testu próg i mediany pozostają takie same. Macierz testowa nadal ma 600 wierszy i 7 kolumn. Jeśli zmienił się próg, sprawdź, czy ktoś ponownie wywołał `fit` na teście.

**Pytanie na wyjście.** „Usunęliśmy kolumnę z późniejszym zwrotem. Czy przyszłość może mimo to wpłynąć na przygotowanie danych?” Oczekuj przykładu z medianą albo progiem policzonym przed podziałem.

## Warsztat o sesjach i paradoksie Simpsona — 90 minut

**Jak zacząć**

> Macie dwa kanały sprzedaży, A i B. Za chwilę poproszę was o rekomendację dla osoby, która dzieli budżet. Najpierw pokażecie jej tylko dwa wyniki. Potem dołożymy jedną informację o użytkownikach i zobaczymy, kto podtrzyma swoją rekomendację.

**Jak poprowadzić**

1. **10 min · audyt.** Otwierają `sesje.csv` i `klienci.csv` z folderu warsztatu. Liczą wiersze i sesje. Pytasz, czy brak wieku klienta odbiera nam wiedzę o tym, czy sesja zakończyła się zakupem.
2. **20 min · łączenie.** Sprawdzają identyczność kopii, porządkują zapis kwot, usuwają powtórzenia. Przy łączeniu wiele sesji → jeden klient najpierw oglądają błąd walidacji. Po uporządkowaniu tabeli klientów wykonują lewe złączenie. Liczba sesji po nim ma pozostać równa 850.
3. **15 min · pierwsza decyzja.** Oglądają rozkład znanych kwot zakupów i liczą konwersję dla A i B. Zatrzymaj grupę. Poproś o zapisanie rekomendacji jednym zdaniem, zanim otworzą podział według urządzenia.
4. **20 min · druga decyzja.** Liczą tę samą konwersję osobno dla telefonu i komputera. Na tablicy zestaw cztery ułamki. Poproś o ponowne porównanie przy wspólnej strukturze 50% telefonów i 50% komputerów.
5. **15 min · granice prognozy.** Niech wskażą, czy w chwili otwarcia sesji znali już jej końcowy czas, wartość zamówienia i późniejszy zwrot. Poproś o jedną możliwą cechę z historii sprzed sesji.
6. **10 min · raport.** Każda para oddaje tabelę z licznikami i mianownikami, wykres oraz cztery zdania: wynik ogółem, wynik po podziale, ograniczenie danych i następny krok. Wróć do pytania zapisanego na początku zajęć.

**Dla Ciebie.** Ujawniaj tabelę etapami. Ostatni wiersz oznacza średnią dwóch wskaźników dla każdego kanału przy zadanych wspólnych wagach.

| Porównanie | Kanał A | Kanał B |
|---|---:|---:|
| Wszystkie sesje | 315/480 = 65,63% | 263/370 = 71,08% |
| Komputer | 81/90 = 90% | 208/260 = 80% |
| Telefon | 234/390 = 60% | 55/110 = 50% |
| Wspólne wagi 50/50 | 75% | 65% |

**Co powiedzieć po odsłonięciu tabeli.** „W kanale B aż 260 z 370 sesji pochodzi z komputerów. W A tylko 90 z 480. Na komputerach oba kanały mają wyższą konwersję, więc skład ruchu zmienia wynik ogółem. Kto potrafi teraz obronić zdanie o tym, co zaobserwowaliśmy? A jakich danych lub jakiego eksperymentu potrzebujecie, żeby przewidzieć skutek przesunięcia budżetu?”

## 04 · Ranking regionalny w SQL — 45 minut

**Jak zacząć**

> Dyrektor sprzedaży w Lublinie prosi o dwie kategorie o największym obrocie. Przy każdej chce procent sprzedaży województwa. Zanim napiszemy SQL, dokończcie zdanie: „Te 100 procent oznacza…”. Od odpowiedzi zależy kolejność operacji w zapytaniu.

**Jak poprowadzić**

1. **15 min.** Studenci wczytują plik elektroniki partiami po 17 003 wiersze. W każdej partii sumują grosze i liczą pozycje według województwa i kategorii. Zapisują częściowe wyniki w SQLite. Przy ponownym uruchomieniu mają zacząć od pustej tabeli.
2. **20 min.** W SQL scalają wyniki tej samej kategorii ze wszystkich partii. Wyznaczają pełny obrót województwa i miejsce kategorii w regionie. Dopiero wtedy wybierają dwa pierwsze miejsca. Przy remisie rozstrzygają alfabetycznie.
3. **10 min.** Porównują liczbę pozycji i sumę groszy z zadaniem 02. Poproś jedną osobę, żeby odczytała lubelski wiersz pełnym zdaniem.

**Dla Ciebie.** W województwie lubelskim **komputery i monitory mają 30,8%**, a duże AGD 21,4% obrotu. Razem około 52,2%. Jeżeli te dwie pozycje sumują się do około 100%, poproś o pokazanie etapu, na którym odfiltrowano pozostałe kategorie. Jeśli obrót się podwoił, sprawdź, czy drugi przebieg importu dopisał te same partie.

## 05 · Kolejka kontroli transakcji — 45 minut

**Jak zacząć**

> Zmiana się skończyła. Mamy 600 transakcji i czas na 30 kontroli. Które sprawdzicie? Zanim pokażę wam model, powiedzcie, jak rozpoznacie, że jego lista jest lepsza od losowania.

**Jak poprowadzić**

1. **10 min.** Studenci układają transakcje w czasie i dzielą je na 1800 do treningu, 600 do walidacji i 600 do testu. W tym zadaniu potrzebują osobnego okresu do oceny modelu przed testem. Liczą przypadki nadużyć w każdym okresie.
2. **15 min.** Na treningu dopasowują imputację, skalowanie i regresję logistyczną. Na walidacji porównują średnią precyzję rankingu (AP) z wynikiem modelu przypisującego wszystkim ten sam poziom ryzyka.
3. **20 min.** Sortują test według ryzyka i biorą pierwsze 30 pozycji. Poproś o zapisanie dwóch ułamków opisujących te same trafienia. Dopiero kiedy podadzą oba mianowniki, wprowadź nazwy „precyzja” i „czułość”.

**Dla Ciebie.** Walidacyjne AP modelu wynosi ok. 0,484 wobec 0,0167 dla stałego wyniku. W teście wśród 30 kontroli znalazło się **8 nadużyć**, a łącznie było ich 14. Precyzja to 8/30 = **26,7%**. Czułość to 8/14 = **57,1%**. Przy losowej kolejce tej długości oczekujemy średnio 0,7 trafienia. To średnia z hipotetycznych powtórzeń.

**Zamknięcie dla wersji 6 × 45 min.** „Osobie kierującej zespołem kontroli możecie teraz powiedzieć, ilu sprawom poświęci zespół czas, ile przypadków znalazł w tym teście i ile przegapił. Która z tych liczb jest najważniejsza dla kierownika zmiany? A która dla osoby odpowiadającej za straty?”

## 06 · Koszt decyzji — dodatkowe 45 minut

**Jak zacząć**

> Zmieniamy warunki. Teraz transakcje napływają pojedynczo i od razu trzeba zdecydować, czy uruchomić kontrolę. Nie znamy jeszcze reszty zmiany, więc nie możemy wybrać jej pierwszych 30 pozycji w rankingu. Przyjmijmy, że kontrola kosztuje 8 zł, a przeoczenie nadużycia 250 zł. Przy jakim wyniku modelu podniesiecie alarm?

**Jak poprowadzić**

1. **15 min.** Na walidacji studenci porównują osiem progów z notebooka. Dla każdego liczą koszt: 8 zł × wszystkie kontrole + 250 zł × przeoczone nadużycia. Symulacja zakłada, że zlecona kontrola wykryje nadużycie.
2. **15 min.** Wybierają najtańszy próg na walidacji, zapisują go i stosują na późniejszym teście. Porównują koszt z kontrolowaniem wszystkich oraz z brakiem kontroli.
3. **15 min.** Wracają do walidacji i zmieniają koszt przeoczenia na 100, potem na 500 zł. Wyjaśniają zmianę progu lub jej brak. Poproś o wskazanie, które założenie najpierw sprawdziliby u właściciela procesu.

**Dla Ciebie.** Przy 250 zł najtańszy spośród sprawdzonych progów to **0,03**. Na teście daje 47 kontroli i 6 przeoczeń, czyli **47 × 8 + 6 × 250 = 1876 zł**. Brak kontroli kosztuje 3500 zł, kontrolowanie wszystkich 4800 zł. Oszczędność wobec braku kontroli wynosi 1624 zł w tej symulacji. Przy stracie 100 zł walidacja wybiera próg 0,10, przy 500 zł nadal 0,03.

**Pytanie do omówienia.** „Czy przenieślibyście próg 0,03 do prawdziwego banku? Jak sprawdzicie rzeczywisty koszt przeoczenia i skuteczność osoby kontrolującej?” Poproś o propozycję pomiaru, zanim grupa poda nową wartość progu.

## 07 · Eksperyment z rozmiarem partii — dodatkowe 45 minut

**Jak zacząć**

> W zadaniu 02 pokazaliście, że wynik można policzyć partiami. Teraz macie wybrać ustawienie dla komputera w laboratorium. Na pojedynczą ramkę danych wolno przeznaczyć 10 MiB. Zapiszcie hipotezę: która z partii — tysiąc, dziesięć tysięcy czy pięćdziesiąt tysięcy wierszy — okaże się najlepsza przy tym limicie?

**Jak poprowadzić**

1. **15 min.** Każda para przygotowuje pomiar pełnego odczytu. Zapisuje czas, maksymalny rozmiar ramki zmierzony przez `memory_usage(deep=True)`, liczbę pozycji i sumę groszy.
2. **15 min.** Uruchamia trzy przebiegi na rozmiar partii, za każdym razem zmieniając kolejność ustawień. Przed porównaniem czasów sprawdza, czy we wszystkich dziewięciu przebiegach obliczono to samo.
3. **15 min.** Studenci zestawiają mediany czasu i maksymalne rozmiary ramek. Spośród ustawień mieszczących się w limicie wybierają najszybsze na swoim komputerze. Oddają wykres oraz jednozdaniowe uzasadnienie.

**Dla Ciebie.** W przykładowym uruchomieniu ramki zajmowały ok. 0,55, 5,47 i 27,36 MiB. Najszybsza partia mieszcząca się w limicie miała 10 000 wierszy. Uznaj inny wynik, jeśli wynika z pomiarów grupy. Limit dotyczy pojedynczej ramki. Parser CSV, obiekty tymczasowe i interpreter również zużywają pamięć.

**Zamknięcie zajęć.** „Na początku każdy zapisał pytanie do raportu. Wybierzcie teraz jeden wynik z dzisiejszych zajęć i zadajcie to pytanie swojemu partnerowi. Odpowiadający ma pokazać konkretny wiersz tabeli, obliczenie albo pomiar, który uzasadnia odpowiedź.”
