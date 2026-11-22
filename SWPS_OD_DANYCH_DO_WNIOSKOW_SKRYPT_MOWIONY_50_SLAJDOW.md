# Od danych do wniosków
## Pełny skrypt mówiony do 50 slajdów

SWPS Poznań · 22 listopada 2026 · dr Marcin Albiniak

Zdania pod każdym slajdem są gotowe do wypowiedzenia. Wskazówek w nawiasach kwadratowych nie czytasz na głos. Zawierają pauzy, pytania i czas samodzielnej pracy. Czas bloków obejmuje mowę, wspólne obliczenia i rozmowę z uczestnikami. Tempo zależy od odpowiedzi grupy.

Prezentacja z nową oprawą: https://chatgpt.com/space/page_e1c2f7177834819188c6793c356f7c3c

### Harmonogram

| Czas | Zakres | Slajdy |
|---|---|---|
| 09:00–09:45 | Jednostka obserwacji i pytanie | 1–8 |
| 09:45–10:30 | Budowa zbioru | 9–15 |
| 10:30–10:45 | Przerwa | |
| 10:45–11:30 | Eksploracja i rozkłady | 16–22 |
| 11:30–12:15 | Porównanie kanałów | 23–29 |
| 12:15–12:45 | Przerwa | |
| 12:45–13:30 | Niepewność i zakres wniosków | 30–36 |
| 13:30–14:15 | Przygotowanie danych do predykcji | 37–43 |
| 14:15–14:30 | Przerwa | |
| 14:30–16:00 | Warsztat z omówieniem | 44–49 |
| W razie pytań | Źródła techniczne | 50 |


---

## Slajd 01. Od danych do wniosków

*A · 09:00–09:45 · plan orientacyjny: 5 min*

Dzień dobry. Wczoraj patrzyliśmy na system od strony jego konstrukcji. Rozmawialiśmy o tym, skąd napływają dane, jak je przechowujemy i jak system przechodzi od informacji do działania. Dziś wejdziemy do środka pracy analityka. Dostaniemy tabelę i spróbujemy ustalić, co rzeczywiście można z niej powiedzieć.

Zacznijmy od sytuacji, którą łatwo sobie wyobrazić. Firma prowadzi sprzedaż w dwóch kanałach. Ktoś przynosi raport i mówi: drugi kanał ma wyższą konwersję, więc powinniśmy przesunąć do niego budżet. Procenty wyglądają przekonująco. Obliczenia się zgadzają. A jednak decyzja może być przedwczesna.

Przez cały dzień będziemy wracać do tego samego przykładu. Dzięki temu zobaczycie, jak kolejne decyzje analityczne zmieniają sposób czytania wyniku. Najpierw określimy, co oznacza wiersz. Potem sprawdzimy, jak połączyć tabele. Przyjrzymy się rozkładom i porównamy grupy. Na końcu zastanowimy się, jak daleko wolno nam uogólniać obserwacje oraz które dane można wykorzystać do przewidywania przyszłości.

Wszystkie liczby w dzisiejszym przykładzie są syntetyczne. Przygotowaliśmy je do nauki. Pokazują określone zjawiska, ale nie są raportem o prawdziwej firmie.

Mam do was pierwsze pytanie. Co chcielibyście wiedzieć, zanim zgodzilibyście się na przesunięcie pieniędzy pomiędzy kanałami? Na razie zostawmy algorytmy. Interesuje mnie sama decyzja.

[PAUZA: 45–60 sekund na odpowiedzi.]

Pojawiają się koszty, marża, rodzaj klientów, okres pomiaru. Bardzo dobrze. Zauważcie, że tabela z procentami nie zawiera jeszcze całej sytuacji decyzyjnej. Dzisiaj będziemy uczyć się właśnie takiego uważnego czytania danych.

---

## Slajd 02. Plan dnia

*A · 09:00–09:45 · plan orientacyjny: 4 min*

Spójrzmy na plan. Pierwszą część dnia poświęcimy jednostce analizy i przygotowaniu zbioru. To miejsce, w którym można popełnić błąd, zanim jeszcze uruchomi się jakikolwiek model. Potem przejdziemy do eksploracji: rozkładów, typowych wartości i porównań pomiędzy grupami.

Po dłuższej przerwie zajmiemy się niepewnością wyniku. Porozmawiamy o liczebności, zależności obserwacji i o tym, dlaczego wąski przedział nie musi oznaczać, że zrozumieliśmy rzeczywistość. Następnie przygotujemy perspektywę pod przyszłe modelowanie: ustalimy, co system może wiedzieć w chwili prognozy.

Od czternastej trzydzieści pracujecie samodzielnie. Dostaniecie eksport sesji i słownik klientów. Przejdziecie od surowego pliku do krótkiego raportu. Będzie tam kilka celowych problemów. Ich rozpoznanie jest częścią zadania.

Podczas wykładu będę prosił was o odpowiedzi i proste obliczenia. Nie musimy od razu pisać kodu. Najpierw chcę, żebyście umieli wyjaśnić, co liczy dana operacja. Kod stanie się wtedy zapisem rozumowania, które już rozumiecie.

Przerwy mamy o dziesiątej trzydzieści, dwunastej piętnaście i czternastej piętnaście. Przed warsztatem potrzebne będzie środowisko do notebooka: Jupyter albo Colab. Dwa pliki CSV powinny znaleźć się w tym samym katalogu co notebook.

Na koniec dnia interesują mnie dwa rezultaty. Poprawnie policzona tabela oraz kilka zdań, za które potraficie wziąć odpowiedzialność. Zaczynamy od pierwszego raportu.

---

## Slajd 03. Decyzja o budżecie

*A · 09:00–09:45 · plan orientacyjny: 6 min*

Mamy kanał A: czterysta osiemdziesiąt sesji i trzysta piętnaście zakupów. Kanał B: trzysta siedemdziesiąt sesji i dwieście sześćdziesiąt trzy zakupy. Proszę policzyć, jaki odsetek sesji w każdym kanale zakończył się zakupem.

[PAUZA: 60 sekund na samodzielne obliczenie.]

W A otrzymujemy sześćdziesiąt pięć i sześćset dwadzieścia pięć tysięcznych procenta, czyli po zaokrągleniu sześćdziesiąt pięć przecinek sześćdziesiąt trzy procent. W B mamy około siedemdziesięciu jeden przecinek zero osiem procent. Wynik ogółem jest więc wyższy w B.

Teraz szybka decyzja: kto na podstawie tych liczb przesunąłby budżet do B? Możecie podnieść rękę albo napisać odpowiedź na czacie.

[PAUZA: 30 sekund.]

Zapiszmy tę pierwszą intuicję. Wrócimy do niej później. Sam rachunek jest poprawny. Zakres wniosku wymaga jednak doprecyzowania. Widzimy konwersję zarejestrowanych sesji. Nie znamy kosztu ruchu, marży ze sprzedaży ani sposobu kierowania klientów do kanałów.

Możliwe, że B przyciąga przede wszystkim osoby gotowe do zakupu, a A spotyka klientów dopiero rozpoczynających poszukiwania. Możliwe też, że różnią się urządzenia albo rodzaje produktów. Każda z tych możliwości zmienia interpretację porównania.

I jeszcze jedna rzecz: nazwy A i B są tutaj nazwami kanałów. Nie oznaczają losowego eksperymentu. Niczego jeszcze nie wylosowaliśmy. Mamy obserwacje. Na razie wolno nam powiedzieć, że w tym eksporcie B ma wyższą konwersję ogółem. Pytanie o skutek przesunięcia budżetu zostawmy otwarte.

---

## Slajd 04. Jednostka obserwacji

*A · 09:00–09:45 · plan orientacyjny: 6 min*

Zatrzymajmy się przy słowie „sesja”. Co dokładnie jest jednostką obserwacji? Jedna sesja oznacza jedną wizytę w serwisie. Ta sama osoba może przyjść rano, wrócić po południu i kupić dopiero wieczorem. Wtedy mamy trzy sesje, jednego klienta i być może jedno zamówienie.

Jeżeli każdą wizytę zapisaliśmy jako osobny wiersz, analizujemy zachowanie sesji. Gdybyśmy zbudowali tabelę z jednym wierszem na klienta, odpowiadalibyśmy na inne pytania. A tabela z samymi zamówieniami obejmowałaby tylko zdarzenia, w których doszło do zakupu.

Weźmy prosty przykład. Jedna osoba odwiedza sklep pięć razy i kupuje podczas jednej wizyty. Konwersja sesji tej osoby wynosi dwadzieścia procent. Odsetek kupujących wśród klientów, jeżeli obserwujemy tylko tę jedną osobę, wynosi sto procent. Oba wyniki są poprawne. Każdy opisuje coś innego.

Zapytam teraz: jeżeli nasz plik ma osiemset pięćdziesiąt sesji, ilu mamy klientów?

[PAUZA: 30–45 sekund.]

Z samej liczby sesji tego nie wiemy. Potrzebujemy identyfikatora klienta i policzenia jego unikalnych wartości. W naszym przygotowanym zbiorze będzie czterystu dwudziestu pięciu klientów, ale dowiemy się tego z danych, a nie z samego rozmiaru tabeli.

Zanim zaczniecie analizę, dokończcie zdanie: jeden wiersz w mojej tabeli oznacza… To proste zdanie ogranicza bardzo wiele późniejszych pomyłek. Dzięki niemu wiemy również, które powtórzenia identyfikatorów są oczekiwane. Powtarzający się klient jest normalny. Powtarzający się klucz tej samej sesji wymaga sprawdzenia.

---

## Slajd 05. Mianownik i zakres populacji

*A · 09:00–09:45 · plan orientacyjny: 6 min*

Wskaźnik jest ułamkiem. W liczniku mamy zdarzenia, które nas interesują, a w mianowniku zbiór, do którego je odnosimy. U nas licznik to liczba sesji zakończonych zakupem. Mianownik to wszystkie sesje zakwalifikowane do analizowanego zakresu.

Wyobraźcie sobie teraz, że ktoś przed obliczeniem konwersji usuwa wszystkie wiersze bez zamówienia. Co otrzymamy?

[PAUZA: 30 sekund.]

Sto procent. Każda pozostała sesja zakończyła się zakupem. Nie zwiększyliśmy jednak sprzedaży. Zmieniliśmy populację, na której liczymy wskaźnik. To przykład błędu, który potrafi ukryć się pod pozornie niewinnym filtrem.

Dlatego pytam nie tylko o wzór. Pytam również o zakres dat, kryteria uwzględnienia sesji i zasady wyłączeń. Czy porównujemy ten sam miesiąc? Czy w obu kanałach uwzględniamy mobile? Czy jednakowo rejestrujemy wizyty bez zakupu?

Do tego dochodzi problem niepełnej rejestracji. Część wizyt może nie trafić do eksportu. Przykładowo system śledzenia może działać inaczej na różnych urządzeniach. Duża tabela nie daje nam automatycznie kompletnego obrazu.

W naszym ćwiczeniu definicję uprościmy: bierzemy wszystkie unikalne sesje z przygotowanego eksportu. Zmienna converted ma wartość jeden, jeżeli nastąpił zakup, i zero w przeciwnym razie. Jej średnia po sesjach będzie odsetkiem zakupów na sesję.

Proszę zapamiętać pytanie, które warto zadawać przy każdym procencie: spośród czego? Bez odpowiedzi trudno ocenić zarówno wynik, jak i porównanie z innym raportem.

---

## Slajd 06. Cztery rodzaje pytań

*A · 09:00–09:45 · plan orientacyjny: 6 min*

Pod podobnie brzmiącym pytaniem biznesowym mogą kryć się bardzo różne zadania. Pierwszy rodzaj to opis. Pytamy, ile zakupów zarejestrowaliśmy i jaki odsetek sesji zakończył się zakupem. Do tego wystarczy poprawnie zdefiniowany zbiór oraz rachunek.

Drugi rodzaj to diagnoza. Sprawdzamy, w jakich przekrojach wyniki się różnią. Może urządzenia, regiony albo dni tygodnia pomagają opisać strukturę obserwowanej różnicy. W tym miejscu łatwo przejść od słowa „współwystępuje” do słowa „powoduje”, choć dowód jeszcze się nie pojawił.

Trzeci rodzaj to predykcja. Chcemy wiedzieć, która przyszła sesja prawdopodobnie zakończy się zakupem. Musimy wtedy ustalić moment prognozy i ocenić wynik na danych odpowiadających przyszłemu zastosowaniu.

Czwarty rodzaj dotyczy interwencji. Pytamy, co zmieni się po zwiększeniu budżetu, zmianie strony albo wprowadzeniu rabatu. To pytanie przyczynowe. Sama dobra predykcja nie odpowiada na nie automatycznie.

Spróbujmy sklasyfikować zdanie: „Klienci, którzy długo oglądają ofertę, częściej kupują”. To opis zależności. Teraz drugie: „Wydłużmy wizytę klienta, a zwiększymy sprzedaż”. To już twierdzenie o skutku działania. Wymaga innych dowodów.

[PAUZA: 60 sekund. Poproś o jeden własny przykład pytania z każdej kategorii.]

W praktyce analityk powinien umieć rozpoznać, kiedy rozmówca zmienia rodzaj pytania. Możemy przygotować poprawny raport opisowy, a ktoś przeczyta go jako instrukcję działania. Naszą rolą jest wtedy jasno wskazać, gdzie kończy się dostarczony dowód.

---

## Slajd 07. Chwila pomiaru

*A · 09:00–09:45 · plan orientacyjny: 6 min*

W analizie danych czas określa, co możemy wiedzieć. Załóżmy, że chcemy przewidzieć zakup dokładnie w momencie rozpoczęcia sesji. W tej chwili znamy pewne informacje: urządzenie, być może kanał wejścia i wcześniejszą historię klienta. Nie znamy jeszcze wyniku obecnej wizyty.

Po zakończeniu sesji tabela będzie bogatsza. Poznamy długość całej wizyty, wartość zamówienia i wynik zakupowy. Po kilku dniach może pojawić się również zwrot. Tabela, którą oglądamy dzisiaj, zawiera więc informacje pochodzące z różnych momentów procesu.

Do raportu historycznego możemy użyć czasu całej sesji. Chcemy przecież opisać to, co już się wydarzyło. Ale jeżeli na podstawie tej samej kolumny ocenimy model działający na wejściu, damy mu informację, której w prawdziwej pracy jeszcze by nie miał.

Podobnie z kwotą zwrotu. Może być interesującym wynikiem obsługi klienta. W chwili rozpoczęcia zakupu nie istnieje jednak w swojej późniejszej postaci.

Pomyślcie teraz o rabacie przyznanym przy finalizacji. Czy rabat jest dopuszczalną cechą modelu? Odpowiedź zależy od chwili prognozy. Jeśli prognozujemy przed przyznaniem rabatu, późniejsza informacja nie jest dostępna. Jeśli inne zadanie wykonujemy już po tej decyzji, sytuacja może wyglądać inaczej.

[PAUZA: 45 sekund na wskazanie momentów procesu.]

Dlatego sama nazwa kolumny nie rozstrzyga o jej przydatności. Potrzebujemy osi czasu i konkretnego zadania. Ten warunek wróci podczas przygotowania danych do modelowania.

---

## Slajd 08. Specyfikacja analizy

*A · 09:00–09:45 · plan orientacyjny: 6 min*

Zamknijmy pierwszy fragment krótką specyfikacją. Naszą jednostką jest sesja. Wynik oznacza zakup podczas tej sesji. Porównujemy dwa kanały, a później sprawdzimy także przekrój urządzeń. Na podstawie tego eksportu opisujemy różnice. Nie przypisujemy im jeszcze interpretacji przyczynowej.

Do tego dopiszmy zasady pracy z danymi. Identyfikator sesji powinien być unikalny. Jeżeli znajdziemy identyczne kopie tego samego rekordu, sprawdzimy je i zachowamy jedną obserwację. Jeżeli pod jednym identyfikatorem pojawią się sprzeczne treści, samodzielny wybór pierwszej wersji nie rozstrzyga konfliktu.

Błędnej kwoty nie zmienimy automatycznie w zero. Nie usuniemy też sesji tylko dlatego, że nie znamy wieku klienta. Wiek nie jest potrzebny do policzenia konwersji kanałów. Każdy filtr musi mieć związek z pytaniem analitycznym.

Proszę teraz powiedzieć własnymi słowami, co dokładnie będziemy mierzyć.

[PAUZA: 60 sekund na dwie odpowiedzi.]

Jeżeli w odpowiedzi pojawia się sformułowanie „odsetek klientów”, doprecyzujmy je. Na tym etapie mierzymy odsetek sesji. Zmiana jednego słowa zmienia jednostkę i oczekiwany rachunek.

Taka specyfikacja może zajmować pół strony. Oszczędza później wiele pracy, bo pozwala oceniać kolejne operacje. Przy każdej z nich zapytamy: czy nadal mamy jedną obserwację na sesję? Czy mianownik pozostał zgodny z deklaracją? Czy wynik odpowiada temu samemu pytaniu? Z tym opisem przejdźmy do budowy tabeli.

---

## Slajd 09. Tabela analityczna

*B · 09:45–10:30 · plan orientacyjny: 6 min*

Tabela analityczna powstaje dla określonego pytania. Nie musimy wrzucać do niej wszystkich pól, które udało się wyeksportować. Najpierw określamy wiersz i klucz, potem dobieramy informacje potrzebne do analizy.

U nas jeden wiersz odpowiada jednej sesji. Session_id identyfikuje wizytę, customer_id klienta. Dalej mamy czas rozpoczęcia, kanał i urządzenie. Zmienna converted opisuje wynik, a order_value_pln kwotę zamówienia.

Sama lista nazw nie wystarcza. Potrzebujemy słownika danych. W słowniku wyjaśniamy, czy czas podano w sekundach, co oznacza zero, jak zapisujemy brak informacji i kiedy dana wartość staje się dostępna. Osoba przejmująca analizę nie powinna zgadywać tych rzeczy na podstawie nazwy kolumny.

Wyobraźcie sobie, że do sesji dołączamy pozycje zamówienia. Jedno zamówienie może mieć pięć produktów. Jeżeli połączymy tabele bez wcześniejszego przygotowania, jedna sesja może zamienić się w pięć wierszy. Dane wyglądają wtedy bogatsze, ale nasza jednostka uległa zmianie.

Jak można zachować jeden wiersz na sesję? Możemy wcześniej zagregować pozycje, na przykład obliczyć liczbę produktów lub sumę zamówienia. Możemy też świadomie zbudować osobny zbiór do analizy pozycji. Ważne, żebyśmy wiedzieli, które zadanie realizujemy.

[PAUZA: 60–90 sekund. Poproś o wskazanie klucza tabeli zamówień i tabeli pozycji.]

Po każdej większej transformacji będziemy wracać do tej samej kontroli: czy klucz sesji nadal jest unikalny? Dzięki temu sprawdzamy, czy rachunek pozostaje zgodny z konstrukcją naszego zbioru.

---

## Slajd 10. Typ danych i znaczenie pomiaru

*B · 09:45–10:30 · plan orientacyjny: 6 min*

Typ techniczny i znaczenie wartości to dwie powiązane, ale odrębne sprawy. Python może odczytać kolumnę jako liczbę, mimo że zawiera ona identyfikator. Może też odczytać kwotę jako tekst, ponieważ w jednym wierszu pojawił się przecinek albo błędny zapis.

Weźmy identyfikatory klientów: sto jeden, sto dwa, sto trzy. Ich średnia wynosi sto dwa. Rachunkowo wszystko się zgadza. Biznesowo wynik niczego nie opisuje. Identyfikator służy do rozróżniania obiektów, a nie mierzenia ich wielkości.

Podobnie z urządzeniem. Możemy zakodować desktop jako zero i mobile jako jeden. To nie znaczy, że klient z telefonu ma o jedną jednostkę więcej jakiejś fizycznej cechy. Liczba jest w tym miejscu kodem kategorii.

Przy kwocie mamy natomiast skalę ilościową i jednostkę: PLN. Jeżeli dwie tabele używają różnych walut albo jedna przechowuje grosze, proste połączenie wartości może dać absurdalny wynik. Ten sam problem dotyczy czasu w sekundach i minutach.

W ćwiczeniu zobaczycie zapis sto dwadzieścia pięć przecinek pięćdziesiąt oraz dwa teksty, których nie da się odczytać jako kwoty. Zamiana przecinka na kropkę pozwala odczytać pierwszy przypadek. Pozostałe wymagają oznaczenia jako nieznane. Zachowamy też oryginalny zapis, żeby móc wrócić do przyczyny problemu.

Proszę podać po jednym przykładzie kolumny, na której sensownie liczymy średnią, oraz takiej, na której średnia byłaby myląca.

[PAUZA: 45–60 sekund.]

To jest moment, w którym wiedza o pomiarze spotyka się z typami danych w programie. Potrzebujemy obu.

---

## Slajd 11. Brak wartości i zero

*B · 09:45–10:30 · plan orientacyjny: 7 min*

Brak informacji i zero niosą inne znaczenie. W naszym przykładzie sesja bez zakupu ma wartość zamówienia równą zero. To uzasadniony zapis biznesowy: podczas tej wizyty nie powstało zamówienie.

Jeżeli natomiast nie znamy wieku klienta, wpisanie zera oznaczałoby coś zupełnie innego. Zmienilibyśmy brak wiedzy w twierdzenie, że klient ma zero lat. Średnia wieku obniżyłaby się, choć nie poznaliśmy żadnej nowej osoby.

Pusta komórka może mieć różne przyczyny. Informacji nie zebrano. Pytanie nie dotyczyło danego przypadku. Dane zaginęły podczas eksportu. A czasem użytkownik świadomie ich nie podał. Sposób postępowania powinien zależeć od przyczyny i celu analizy.

Czy możemy uzupełnić wiek medianą? Technicznie tak. Ale mediana nie jest odzyskanym wiekiem tej osoby. Tworzymy wartość zastępczą, a wraz z nią określone założenie. Rozkład po imputacji będzie inny niż rozkład rzeczywiście zaobserwowanych wartości.

Przy kwocie zamówienia ostrożność jest szczególnie ważna. Jeśli zakup nastąpił, ale kwoty nie znamy, zero zaniżałoby przychód. W naszym zbiorze zachowamy taki rekord przy liczeniu konwersji, bo wynik zakupowy jest znany. Ujawnimy natomiast brak kwoty przy analizie wartości zakupów.

Co zrobilibyście z sesją klienta, któremu brakuje wieku, jeżeli pytanie dotyczy wyłącznie kanału i zakupu?

[PAUZA: 45 sekund.]

Nie ma powodu usuwać jej automatycznie. Potrzebne informacje są dostępne. Stosowanie dropna do całej tabeli mogłoby zmienić naszą populację bez uzasadnienia.

---

## Slajd 12. Duplikat techniczny i kolejna wizyta

*B · 09:45–10:30 · plan orientacyjny: 6 min*

Słowo „duplikat” wymaga dopowiedzenia: duplikat czego? Dwa wiersze z tym samym klientem mogą oznaczać dwie prawdziwe wizyty. Dwa identyczne wiersze z tym samym kluczem sesji mogą natomiast pochodzić z ponownego dołączenia tego samego eksportu.

W naszym pliku przygotowaliśmy dwanaście dodatkowych kopii sesji. To powtórzenia identyczne. Po sprawdzeniu zgodności treści możemy zachować po jednym rekordzie. Nie powinniśmy jednak zaczynać od usuwania powtórzeń po identyfikatorze klienta. W ten sposób skasowalibyśmy jego kolejne wizyty.

Rozważmy trudniejszy przypadek. Ten sam identyfikator sesji pojawia się dwa razy, ale w jednym wierszu jest zakup, a w drugim go nie ma. Czy wystarczy wybrać pierwszy rekord?

[PAUZA: 45–60 sekund.]

Nie znamy jeszcze reguły rozstrzygnięcia. Być może jeden zapis jest późniejszą aktualizacją. Być może połączono dwa źródła o różnym zakresie. Potrzebujemy informacji o wersji, czasie aktualizacji i znaczeniu pól. Kolejność w pliku sama tego nie wyjaśnia.

Warto więc oddzielić dwa kroki. Najpierw rozpoznajemy powtórzenia według klucza i porównujemy ich zawartość. Dopiero potem stosujemy regułę, którą potrafimy uzasadnić. W prostym ćwiczeniu reguła będzie łatwa. W realnym projekcie może wymagać kontaktu z właścicielem źródła.

Pomyślcie o tym również jako o kontroli licznika i mianownika. Kopia sesji z zakupem zwiększa oba. Kopia sesji bez zakupu zwiększa tylko mianownik. Nawet identyczne techniczne powtórzenie może więc przesunąć wskaźnik.

---

## Slajd 13. Połączenie tabel może pomnożyć wynik

*B · 09:45–10:30 · plan orientacyjny: 7 min*

Łączenie tabel jest jednym z miejsc, w których można otrzymać wiarygodnie wyglądający, ale błędny wynik. Mamy tabelę sesji i słownik klientów. Chcemy dołączyć region oraz wiek. Oczekujemy wielu sesji przypisanych do jednego rekordu klienta.

Wyobraźcie sobie klienta z trzema sesjami. W słowniku pojawia się on dwa razy. Po zwykłym połączeniu każda jego sesja znajdzie dwa dopasowania. Trzy obserwacje zamienią się w sześć. Program nie musi uznać tego za błąd, bo z punktu widzenia operacji łączenia oba dopasowania istnieją.

Co stanie się z liczbą zakupów i sumą przychodu tego klienta? Zostaną policzone dwukrotnie. Jeśli problem dotyczy tylko niektórych klientów, może zniekształcić porównanie kanałów.

W pandas możemy zadeklarować oczekiwaną relację przez validate równe many_to_one. Czytamy to: wiele rekordów po lewej stronie może odpowiadać jednemu rekordowi po prawej. Słownik powinien mieć unikalny klucz klienta. Jeżeli warunek nie jest spełniony, chcemy dostać błąd, zanim policzymy raport.

W ćwiczeniu celowo wystąpi jedna identyczna kopia klienta. Najpierw zobaczycie błąd połączenia. Potem sprawdzicie duplikat i uporządkujecie słownik. Po poprawnym left join nadal powinno być osiemset pięćdziesiąt sesji.

Dlaczego left join? Chcemy zachować wszystkie sesje i sprawdzić dopasowania. Inner join mógłby usunąć rekordy bez klienta w słowniku, zmieniając populację.

[PAUZA: 60–90 sekund. Policzcie razem przykład trzech sesji i dwóch rekordów słownika.]

Kontrolujemy więc równocześnie relację, liczbę wierszy i brak dopasowań. Sam komunikat, że merge się wykonał, nie potwierdza poprawności analizy.

---

## Slajd 14. Granularność agregacji

*B · 09:45–10:30 · plan orientacyjny: 6 min*

Przy agregacji wybieramy poziom, na którym opisujemy dane. Możemy policzyć wszystkie sesje. Możemy policzyć unikalnych klientów. Możemy też najpierw obliczyć wskaźnik dla każdej grupy, a dopiero potem go uśrednić. Te operacje nie muszą dawać tej samej odpowiedzi.

Sprawdźmy prosty przykład. W pierwszej grupie kupuje jedna osoba na dwie. Mamy pięćdziesiąt procent. W drugiej grupie kupuje dziewięćdziesiąt osób na sto. Mamy dziewięćdziesiąt procent. Ile wynosi odsetek zakupów w obu grupach razem?

[PAUZA: 60 sekund na obliczenie.]

Średnia z pięćdziesięciu i dziewięćdziesięciu procent to siedemdziesiąt procent. Ale udział łączny liczymy inaczej: dziewięćdziesiąt jeden zakupów dzielimy przez sto dwie osoby. Otrzymujemy około osiemdziesięciu dziewięciu przecinek dwudziestu dwóch procent.

Różnica wynika z wag. Przy zwykłej średniej procentów obie grupy dostają identyczną wagę, mimo że jedna ma dwie osoby, a druga sto. Przy wskaźniku łącznym waga wynika z liczebności.

Nie oznacza to, że średnia nieważona jest zawsze błędna. Może odpowiadać pytaniu o przeciętną jednostkę organizacyjną, jeśli rzeczywiście chcemy każdej jednostce nadać taką samą wagę. Musimy jednak umieć nazwać to pytanie.

W naszym raporcie zachowamy osobno liczbę zakupów i liczbę sesji. Dzięki temu wskaźnik można poprawnie przeliczyć na wyższym poziomie. Sam gotowy procent bez mianownika utrudnia kontrolę.

Na tym mechanizmie opiera się także zjawisko, które zobaczymy za chwilę przy porównaniu kanałów. Zmiana struktury grup może zmienić wynik ogółem.

---

## Slajd 15. Szybki audyt przed analizą

*B · 09:45–10:30 · plan orientacyjny: 7 min*

Zanim przejdziemy do wykresów, zróbmy krótki audyt. Pierwsze pytanie: ile jest wierszy i ile unikalnych sesji? Drugie: czy typy oraz zakresy wartości pasują do znaczenia kolumn? Trzecie: jakie informacje są nieznane? Czwarte: czy połączenie tabel zachowało naszą jednostkę?

W przygotowanym eksporcie zobaczycie osiemset sześćdziesiąt dwa wiersze i osiemset pięćdziesiąt unikalnych sesji. Dwanaście dodatkowych wierszy to identyczne kopie. W słowniku klientów są czterysta dwadzieścia sześć wierszy i czterystu dwudziestu pięciu klientów. Tam także znajduje się jedna kopia.

Po uporządkowaniu kopii i prawidłowym połączeniu chcemy nadal mieć osiemset pięćdziesiąt sesji. Jednocześnie wiemy, że dwie kwoty pozostają nieznane. To nie jest sprzeczność. Klucz może być poprawny, a pojedyncze pole nadal wymagać uwagi.

Proszę teraz powiedzieć: czy brak wieku powinien usuwać wizytę z analizy konwersji kanałów?

[PAUZA: 30 sekund.]

Nie wynika to z naszego pytania. Wiek nie jest tu potrzebny do licznika ani mianownika. Gdybyśmy analizowali konwersję według wieku, musielibyśmy osobno ustalić, jak opisać grupę bez tej informacji.

Ostatnia kontrola dotyczy odtwarzalności. Powinniśmy potrafić wrócić do surowego pliku i ponownie otrzymać ten sam wynik, wykonując zapisane kroki. Ręczne poprawianie komórek bez śladu utrudnia taką kontrolę.

Mamy więc przygotowaną podstawę. Po przerwie zajmiemy się tym, jak wyglądają wartości i co ukrywają ich proste podsumowania. Wracamy o dziesiątej czterdzieści pięć.

---

## Slajd 16. Rozkład wartości zamówienia

*C · 10:45–11:30 · plan orientacyjny: 6 min*

Spójrzmy teraz na rozkład wartości zamówienia. Gdybym podał wam tylko najmniejszą i największą kwotę, wiedzielibyście, jaki zakres występuje w danych. Nadal nie wiedzielibyście, gdzie znajduje się większość obserwacji.

Możliwe są bardzo różne sytuacje. W jednym sklepie niemal wszystkie zakupy mieszczą się w pobliżu dwustu złotych. W innym większość jest niewielka, ale kilka bardzo dużych zamówień podnosi przychód. Podobny zakres minimum–maksimum nie musi oznaczać podobnego zachowania klientów.

Histogram dzieli oś wartości na przedziały i pokazuje, ile obserwacji do nich trafia. Zobaczymy dzięki temu skupienia, skośność oraz długi ogon. Dobór szerokości przedziałów wpływa na obraz, więc warto sprawdzić więcej niż jedną rozsądną konfigurację.

Przed narysowaniem wykresu musimy jednak ustalić populację. Czy interesuje nas wartość zamówienia, czy przychód przypadający na sesję? W pierwszym przypadku analizujemy wizyty zakończone zakupem. W drugim zostawiamy także sesje bez zakupu, z kwotą równą zero.

To będą dwa różne rozkłady. Zera nie są w tym miejscu błędem. Odpowiadają innej części zachowań. Ich wykluczenie powinno wynikać z pytania, a nie z tego, że histogram bez zer wygląda ładniej.

[PAUZA: 60 sekund. Jak zmieni się histogram po włączeniu sesji bez zakupu?]

W naszym ćwiczeniu pokażemy rozkład poprawnie odczytanych kwot zakupów. Podamy również, ile kwot było nieznanych. Później porównamy średnią i medianę, żeby zobaczyć wpływ dużych transakcji.

---

## Slajd 17. Średnia i mediana

*C · 10:45–11:30 · plan orientacyjny: 6 min*

Na slajdzie mamy pięć zamówień: sto, sto, sto, sto i tysiąc sześćset złotych. Suma wynosi dwa tysiące. Dzielimy ją przez pięć i otrzymujemy średnią równą czterysta złotych.

Teraz uporządkujmy wartości. Środkowym elementem jest trzecie sto złotych. Mediana wynosi więc sto. Średnia i mediana opisują ten sam zbiór, ale odpowiadają na inne pytania.

Jeżeli chcę odtworzyć przychód łączny z liczby zamówień i jednej miary, średnia jest użyteczna. Pięć razy czterysta daje dwa tysiące. Mediana nie ma takiej własności. Pięć razy sto nie odtworzy sumy.

Jeżeli natomiast pytam o zamówienie środkowe, mediana może być bardziej intuicyjna. Cztery z pięciu transakcji miały wartość sto złotych. Średnia czterysta nie oznacza, że taka kwota była najczęściej spotykana. W tym przykładzie nie wystąpiła ani razu.

Co zrobimy, jeżeli największe zamówienie wzrośnie z tysiąca sześciuset do szesnastu tysięcy? Mediana pozostanie równa sto. Średnia silnie wzrośnie. To pokazuje jej wrażliwość na duże wartości.

Którą miarę podalibyście w raporcie dla zarządu?

[PAUZA: 60 sekund na uzasadnienia.]

Możemy podać obie, razem z liczbą zamówień i krótkim opisem rozkładu. Nie trzeba wybierać jednej miary do wszystkich zastosowań. Ważne, żeby każda miała właściwą interpretację.

Podczas ćwiczenia wśród znanych kwot zakupów otrzymamy średnią około dwustu dziewięćdziesięciu pięciu złotych i pięćdziesięciu dziewięciu groszy, a medianę sto dziewięćdziesiąt trzy złote i sześć groszy. Zobaczymy, skąd bierze się ta różnica.

---

## Slajd 18. Kwantyle i zróżnicowanie

*C · 10:45–11:30 · plan orientacyjny: 6 min*

Średnia albo mediana opisują położenie, ale nie mówią jeszcze, jak bardzo wartości się różnią. Dwa zbiory mogą mieć tę samą średnią, choć jeden jest mocno skupiony, a drugi rozciągnięty na szerokim zakresie.

Kwartyl pierwszy i trzeci pomagają opisać środkową połowę danych. W uproszczeniu jedna czwarta obserwacji leży poniżej Q1, a trzy czwarte poniżej Q3. Różnica pomiędzy tymi kwartylami to IQR, rozstęp międzykwartylowy.

W praktyce małych prób dokładny wynik zależy od przyjętej konwencji wyznaczania kwantyli. Różne programy mogą stosować inną interpolację. Jeżeli wyniki narzędzi się nie zgadzają, sprawdźmy ustawienia, zanim uznamy jedną analizę za błędną.

Drugą znaną miarą jest odchylenie standardowe. Mierzy rozproszenie wokół średniej. Jeśli kwoty są w złotych, odchylenie również podajemy w złotych. Wariancja, z której je wyprowadzamy, ma jednostkę złotych do kwadratu.

Wyobraźcie sobie dwie serie: sto, sto, sto oraz zero, sto, dwieście. Obie mają średnią sto. Pierwsza nie ma rozproszenia, druga je ma. Sama średnia ukrywa tę różnicę.

Czy niewielki IQR wyklucza pojedyncze bardzo duże zamówienie?

[PAUZA: 45 sekund.]

Nie. IQR dotyczy środkowej połowy obserwacji. Pojedynczy punkt daleko w ogonie może mieć duży wpływ na średnią, a niewielki na kwartyle. Dlatego do rozumienia rozkładu potrzebujemy kilku uzupełniających się spojrzeń. Miary liczbowe i wykres pomagają się wzajemnie kontrolować.

---

## Slajd 19. Obserwacja odstająca

*C · 10:45–11:30 · plan orientacyjny: 7 min*

Obserwacja odstająca oznacza, że jakiś przypadek wyraźnie różni się od większości. To jeszcze nie rozstrzyga, czy jest błędem. Duże zamówienie może być całkowicie prawidłową transakcją ważnego klienta.

Z drugiej strony bardzo wysoka kwota może powstać po pomyleniu złotych z groszami. Wartość ujemna może być błędem, ale w odpowiedniej tabeli może też oznaczać zwrot albo korektę. Znaczenie ustalamy w kontekście procesu.

Często spotkacie regułę półtora IQR. W klasycznym boxplocie pomaga ona wyznaczyć granice, poza którymi zaznacza się punkty odstające. Dobrze działa jako sygnał: przyjrzyj się temu przypadkowi. Sama nie stanowi uzasadnienia do usunięcia rekordu.

Przygotujmy sobie pytania. Czy zapis ma prawidłową jednostkę? Czy istnieje dokument źródłowy? Czy taki zakup jest możliwy w tej firmie? Czy wartość pochodzi z tego samego rodzaju operacji co pozostałe rekordy?

W naszym zbiorze bardzo duże zamówienia są celowo poprawne. Mamy między innymi kwoty pięć tysięcy dziewięćset, siedem tysięcy dwieście i osiem tysięcy czterysta złotych. Nie chcemy ich usuwać tylko dlatego, że przeszkadzają w uzyskaniu gładkiego histogramu.

Możemy natomiast wykonać analizę wrażliwości: policzyć wynik z pełnym zakresem i sprawdzić, jak zmienia się po jawnie opisanym ograniczeniu ogona. Odbiorca zobaczy wtedy wpływ tej decyzji.

[PAUZA: 60–90 sekund. Kiedy wykluczenie obserwacji byłoby uzasadnione?]

Dobrym uzasadnieniem jest rozpoznany błąd albo jasno określona populacja. Sama niewygoda dla naszej hipotezy nim nie jest.

---

## Slajd 20. Wykres odpowiada pytaniu

*C · 10:45–11:30 · plan orientacyjny: 6 min*

Dobór wykresu zaczyna się od pytania. Jeśli interesuje nas rozkład jednej wielkości, możemy użyć histogramu. Zobaczymy, gdzie skupiają się wartości i jak wygląda ogon.

Jeżeli chcemy porównać rozkłady pomiędzy kanałami, przydatny będzie boxplot. Pokazuje medianę oraz kwartyle. Trzeba jednak pamiętać, że jego skrótowa forma może ukryć dodatkowe skupienia w danych. Przy ważnej decyzji warto wrócić również do bardziej szczegółowego obrazu.

Wykres rozrzutu pomaga zobaczyć współzmienność dwóch wielkości. Na jednej osi może być czas sesji, na drugiej wartość zakupu. Przy wielu punktach pojawia się nakładanie obserwacji, dlatego czasem potrzebujemy przezroczystości albo agregacji.

Słupki dobrze pokazują proporcje w kategoriach, ale sam procent nie ujawnia liczebności. Dziewięćdziesiąt procent z dziesięciu wizyt to inna sytuacja niż dziewięćdziesiąt procent z dziesięciu tysięcy wizyt. Podajmy mianowniki albo liczebności obok wykresu.

Teraz szybkie zadanie. Chcę zobaczyć typowe koszyki i skrajne wartości osobno w A i B. Co proponujecie? Następnie chcę sprawdzić, czy dłuższe sesje współwystępują z większym koszykiem. Jaki wykres wybierzecie?

[PAUZA: 60 sekund na odpowiedzi.]

Nie ma potrzeby używania najbardziej efektownej formy w każdym miejscu. Wykres ma pomóc sprawdzić określoną zależność. Grafika w tle buduje oprawę prezentacji, natomiast dane liczbowe powinny pozostać dokładne, opisane i możliwe do porównania.

---

## Slajd 21. Skala wykresu zmienia odbiór

*C · 10:45–11:30 · plan orientacyjny: 7 min*

Spójrzmy na różnicę pomiędzy siedemdziesięcioma a siedemdziesięcioma jednym procentem. Jeśli oś słupków zaczniemy od sześćdziesięciu dziewięciu procent, wizualna różnica długości może wyglądać olbrzymio. Przy osi od zera do stu procent zobaczymy właściwą skalę udziałów.

W słupkach długość jest podstawowym nośnikiem wartości, dlatego punkt zerowy ma szczególne znaczenie. W innych rodzajach wykresów zawężenie osi bywa uzasadnione, jeśli jest jawne i pomaga w analizie. Nie warto zamieniać dobrej praktyki w regułę oderwaną od sposobu kodowania informacji.

Podobnej uwagi wymaga skala logarytmiczna. Potrafi pokazać wartości różniące się o wiele rzędów wielkości, ale trzeba ją wyraźnie oznaczyć. Równe odległości na takiej osi nie odpowiadają równym przyrostom wartości.

Do tego dochodzi język. Wzrost z pięćdziesięciu do sześćdziesięciu procent wynosi dziesięć punktów procentowych. Względem wartości początkowej jest to wzrost o dwadzieścia procent. Te zdania nie są zamienne.

Policzmy jeszcze przykład: wzrost z dwóch do trzech procent. Ile to punktów procentowych, a ile procent względnie?

[PAUZA: 45–60 sekund.]

Jeden punkt procentowy i pięćdziesiąt procent względnie. Oba opisy mogą być prawdziwe, ale robią inne wrażenie. Dlatego w raporcie podajemy wartości początkową i końcową oraz jednostkę różnicy. Przy ocenie wyniku pomagają również liczebności i odpowiednio uzasadnione przedziały niepewności.

---

## Slajd 22. Dziennik analityka

*C · 10:45–11:30 · plan orientacyjny: 7 min*

Proponuję prosty dziennik analityka. Każdy interesujący wynik zapisujemy w czterech krokach. Najpierw obserwacja: co dokładnie widzę? Potem hipoteza: jakie wyjaśnienie chcę sprawdzić? Następnie kontrola: jaki rachunek może tę hipotezę podważyć? Na końcu ograniczenie: czego dane nie rozstrzygają?

Zwróćcie uwagę na pierwszy krok. Zdanie „średnia kwota w A jest wyższa” opisuje obserwację. Zdanie „klienci A są zamożniejsi” proponuje wyjaśnienie. Drugie nie wynika automatycznie z pierwszego.

Wyższa średnia może być skutkiem kilku dużych transakcji. Może wynikać z innego rodzaju produktów. Może też pojawić się po błędnym połączeniu tabel. Zanim wybierzemy jedną historię, warto rozważyć konkurencyjne możliwości.

Jakie kontrole zaproponujecie? Możemy porównać mediany i kwantyle, sprawdzić rozkłady, rozbić dane na segmenty oraz wrócić do klucza połączenia. Każdy z tych kroków odpowiada na trochę inne podejrzenie.

[PAUZA: 90 sekund. Zapiszcie jedną obserwację bez słowa „ponieważ” i dwie możliwe hipotezy.]

W codziennej pracy największą pokusą bywa szybkie znalezienie przekonującego opowiadania. Człowiek łatwo dopasowuje sens do wykresu. Dlatego dobrze jest zapisać również to, co mogłoby naszą pierwszą odpowiedź osłabić.

Za chwilę zobaczymy przykład, w którym pierwszy wynik będzie poprawny, a późniejsze spojrzenie pokaże zupełnie inną strukturę porównania. Dziennik pomoże nam utrzymać porządek pomiędzy rachunkiem, wyjaśnieniem i rekomendacją.

---

## Slajd 23. Agregat wskazuje kanał B

*D · 11:30–12:15 · plan orientacyjny: 6 min*

Wracamy do pierwszego raportu. A ma trzysta piętnaście zakupów na czterysta osiemdziesiąt sesji. B ma dwieście sześćdziesiąt trzy zakupy na trzysta siedemdziesiąt sesji. Na wykresie pokazujemy udziały od zera, żeby wizualnie nie przesadzać z różnicą.

Konwersja A wynosi około sześćdziesięciu pięciu przecinek sześćdziesięciu trzech procent. Konwersja B około siedemdziesięciu jeden przecinek zero osiem procent. Różnica B minus A wynosi około pięciu przecinek czterdziestu sześciu punktu procentowego.

Proszę przypomnieć sobie pierwszą odpowiedź o przesunięciu budżetu. Czy teraz, po rozmowie o mianowniku i agregacji, chcielibyście zadać jakieś dodatkowe pytanie?

[PAUZA: 60–90 sekund na propozycje przekrojów.]

Możemy pytać o urządzenie, okres, rodzaj klienta i źródło ruchu. W naszym przykładzie przyjrzymy się urządzeniom. Nie dlatego, że każde porównanie trzeba obowiązkowo segmentować właśnie w ten sposób. Dlatego, że znamy konstrukcję tego dydaktycznego przypadku i chcemy ujawnić konkretną strukturę.

Podkreślę: w następnym kroku nie poprawimy tych procentów. One już są poprawne. Rozłożymy je na części. Czasem po analizie segmentów trzeba skorygować błędny rachunek, ale tutaj zobaczymy coś subtelniejszego: kilka prawdziwych opisów tego samego zbioru może prowadzić do różnych intuicji.

Zanim odsłonię tabelę, zapytam: czy kanał może mieć niższy wynik ogółem, a jednocześnie wyższy w każdej z dwóch grup urządzeń? Spróbujcie odpowiedzieć bez liczenia. Za chwilę sprawdzimy to na konkretnych liczbach.

---

## Slajd 24. W obrębie urządzenia prowadzi A

*D · 11:30–12:15 · plan orientacyjny: 7 min*

Spójrzcie najpierw na desktop. Kanał A: osiemdziesiąt jeden zakupów na dziewięćdziesiąt sesji. To dziewięćdziesiąt procent. Kanał B: dwieście osiem zakupów na dwieście sześćdziesiąt sesji. To osiemdziesiąt procent. W tej grupie wyżej wypada A.

Teraz mobile. A ma dwieście trzydzieści cztery zakupy na trzysta dziewięćdziesiąt sesji, czyli sześćdziesiąt procent. B ma pięćdziesiąt pięć zakupów na sto dziesięć sesji, czyli pięćdziesiąt procent. Także tutaj wyżej wypada A.

A jednak przed chwilą ogółem wygrywało B. Nie ma błędu dodawania. Sprawdźmy sumy: w A osiemdziesiąt jeden plus dwieście trzydzieści cztery daje trzysta piętnaście. Dziewięćdziesiąt plus trzysta dziewięćdziesiąt daje czterysta osiemdziesiąt. W B otrzymujemy odpowiednio dwieście sześćdziesiąt trzy i trzysta siedemdziesiąt.

Co różni kanały? Ich struktura. W A ponad osiemdziesiąt jeden procent sesji pochodzi z mobile. W B mobile stanowi około trzydziestu procent. Desktop ma w tym przykładzie wyższą konwersję w obu kanałach. B zawiera dużo więcej sesji z tej grupy.

[PAUZA: 90 sekund. Policzcie udziały urządzeń w każdym kanale.]

Kanał A ma więc wyższy wskaźnik w obrębie obu urządzeń, ale jego wynik ogółem mocno waży grupa o niższej konwersji. W B większą wagę ma grupa o wyższej konwersji.

To nadal opis obserwacji. Nie powiedzieliśmy jeszcze, że przełączenie klienta do A spowoduje wzrost prawdopodobieństwa zakupu. Najpierw zrozummy mechanizm odwrócenia porównania.

---

## Slajd 25. Paradoks Simpsona

*D · 11:30–12:15 · plan orientacyjny: 7 min*

To zjawisko nazywamy paradoksem Simpsona. Po połączeniu grup kierunek porównania może się odwrócić względem kierunku widocznego w grupach. Mechanizm wynika z połączenia dwóch informacji: wyników wewnątrz grup oraz udziałów tych grup w agregacie.

W naszym przykładzie każdy kanał zawiera desktop i mobile, ale w innych proporcjach. Łączny procent nie jest prostą średnią dziewięćdziesięciu i sześćdziesięciu albo osiemdziesięciu i pięćdziesięciu. To średnia ważona rzeczywistymi liczebnościami.

Możemy zapytać, czy więcej danych rozwiązałoby problem. Jeśli powielilibyśmy ten sam układ wiele razy, proporcje pozostałyby takie same. Obraz byłby równie stabilny i równie wymagający interpretacji. Rozmiar nie zastępuje znajomości struktury.

Nie chciałbym jednak, żebyście zapamiętali uproszczenie: zawsze dodaj wszystkie możliwe podziały. Przy opisie przekroje mogą pomagać ujawniać strukturę. Przy wnioskowaniu przyczynowym dobór zmiennych wymaga wiedzy o procesie. Kontrolowanie niektórych zmiennych może nawet wprowadzić dodatkowe obciążenie.

Na przykład zmienna może powstawać już po działaniu, którego efekt chcemy badać. Wtedy jej użycie ma inne konsekwencje niż uwzględnienie cechy znanej wcześniej. Dlatego ważne są czas pomiaru i mechanizm powstawania danych.

[PAUZA: 60 sekund. Jak jednym zdaniem wyjaśnilibyście ten paradoks osobie bez przygotowania statystycznego?]

Możemy powiedzieć: kanały mają inny skład ruchu, a skład wpływa na łączny wynik. To krótka odpowiedź. Pełny raport powinien pokazać również tabelę liczebności, żeby odbiorca mógł sprawdzić rachunek.

---

## Slajd 26. Wspólna struktura porównania

*D · 11:30–12:15 · plan orientacyjny: 6 min*

Spróbujmy porównać kanały przy identycznej strukturze urządzeń. Przyjmiemy dla ilustracji, że w obu kanałach połowa sesji pochodzi z desktopu i połowa z mobile. To jawnie wybrane wagi dydaktyczne.

Dla A liczymy połowę dziewięćdziesięciu procent i połowę sześćdziesięciu procent. Otrzymujemy siedemdziesiąt pięć procent. Dla B połowa osiemdziesięciu i połowa pięćdziesięciu daje sześćdziesiąt pięć procent.

Przy wspólnych wagach A wypada wyżej. Ta operacja to przykład standaryzacji opisowej. Ograniczamy wpływ tego, że kanały mają inny udział urządzeń.

Dlaczego akurat pięćdziesiąt na pięćdziesiąt? W tym ćwiczeniu dlatego, że ułatwia zobaczenie rachunku. W realnej analizie możemy chcieć użyć struktury docelowego ruchu albo innej uzasadnionej populacji odniesienia. Musimy tę decyzję ujawnić.

Sprawdźmy skrajny wariant: sto procent mobile. Jakie wyniki dostaniemy?

[PAUZA: 30 sekund.]

Sześćdziesiąt procent dla A i pięćdziesiąt dla B. Gdyby całość stanowił desktop, byłoby dziewięćdziesiąt i osiemdziesiąt. W tym konkretnym przykładzie różnica wewnątrz obu grup wynosi dziesięć punktów procentowych.

Standaryzacja pomaga uczciwiej opisać porównanie według wskazanych wag. Nadal nie dowodzi skutku interwencji. Nie znamy wszystkich różnic pomiędzy klientami ani sposobu kierowania ruchu. Mamy lepiej zdefiniowany opis, a pytanie o zmianę budżetu wciąż wymaga dodatkowej pracy.

---

## Slajd 27. Korelacja i wspólna przyczyna

*D · 11:30–12:15 · plan orientacyjny: 6 min*

Rozważmy inną zależność. Załóżmy, że w jakimś rzeczywistym raporcie dłuższe sesje częściej kończą się zakupem. To przykład do rozumowania. W naszym syntetycznym zbiorze czas sesji został wygenerowany osobno, więc samą taką zależność należałoby najpierw sprawdzić.

Gdybyśmy ją zaobserwowali, czy moglibyśmy powiedzieć: wydłużmy wizyty, a zwiększymy sprzedaż? Sam wykres tego nie rozstrzyga.

Istnieje kilka możliwych mechanizmów. Klient z silną intencją zakupu może jednocześnie dłużej oglądać ofertę i częściej kupować. To wspólna przyczyna obu obserwowanych wielkości. Możliwe też, że sam proces zakupu wydłuża sesję: trzeba przejść koszyk, podać dane i dokonać płatności.

W tej drugiej sytuacji część czasu sesji jest konsekwencją zdarzenia zakupowego. Gdybyśmy sztucznie dodali użytkownikowi dwie minuty oczekiwania, nie odtworzylibyśmy mechanizmu, który widzimy w danych. Moglibyśmy wręcz utrudnić zakup.

Proszę zaproponować jeszcze jedno wyjaśnienie, które pasuje do tej samej obserwacji.

[PAUZA: 60 sekund na hipotezy.]

To ćwiczenie pokazuje, dlaczego zgodność wzorca z intuicyjną historią nie wystarcza. Potrzebujemy wiedzy o kolejności zdarzeń i mechanizmie. W pewnych sytuacjach pomoże eksperyment. W innych analiza obserwacyjna może wspierać wnioskowanie przyczynowe, ale wymaga jawnych, mocnych założeń.

Dziś naszym celem jest rozpoznanie granicy: opis współwystępowania stanowi początek pytania o przyczynę, a nie gotową odpowiedź.

---

## Slajd 28. Projekt eksperymentu

*D · 11:30–12:15 · plan orientacyjny: 6 min*

Jeśli chcemy zbadać skutek działania, musimy zaprojektować porównanie odpowiadające temu działaniu. W eksperymencie ustalamy jednostkę losowania, przydział wariantów, wynik oraz reguły analizy, zanim zobaczymy efekt.

Załóżmy, że zmieniamy element strony. Możemy rozważyć losowanie klientów do wariantów. Powracający klient powinien wtedy otrzymywać spójny wariant. Gdyby przy każdej wizycie trafiał gdzie indziej, jego wcześniejsze doświadczenie mogłoby wpływać na późniejsze zachowanie w obu grupach.

Przy kampaniach marketingowych jednostka może wyglądać inaczej. Być może sensowne jest losowanie obszarów, kampanii albo innych grup. Nie można automatycznie przenieść jednego schematu na każde zastosowanie. Trzeba uwzględnić sposób działania interwencji i możliwe oddziaływanie pomiędzy jednostkami.

Ustalamy także główny miernik. Sam wzrost liczby zakupów może nie wystarczyć, jeśli rabaty niszczą marżę. Warto wcześniej określić również mierniki, których pogorszenie byłoby nieakceptowalne.

Co z zakończeniem badania? Jeżeli codziennie zaglądamy do wyników i kończymy w chwili pierwszego korzystnego odchylenia, zmieniamy własności procedury. Taki sposób zatrzymywania wymaga odpowiedniego planu analizy.

[PAUZA: 60–90 sekund. Jaką jednostkę losowania wybralibyście przy zmianie procesu obsługi całego oddziału?]

Wróćmy do naszego eksportu. Litery A i B nie czynią z niego eksperymentu. To nazwy kanałów obserwacyjnych. Dlatego wnioski o efekcie zmiany budżetu powinny poczekać na badanie zaprojektowane pod ten cel.

---

## Slajd 29. Zdanie, które wolno opublikować

*D · 11:30–12:15 · plan orientacyjny: 7 min*

Spróbujmy teraz przygotować komentarz, który można przekazać odbiorcy. Pierwsze zdanie: w analizowanym eksporcie kanał B ma wyższą konwersję ogółem. To zdanie jest prawdziwe i ma jasno wskazany zakres.

Drugie zdanie: kanał A ma wyższą konwersję w obu grupach urządzeń. To również jest prawdziwe. Nie musimy unieważniać pierwszego zdania, żeby wypowiedzieć drugie.

Trzecie: odmienne udziały desktopu i mobile odwracają porównanie łączne. Pokazujemy w ten sposób mechanizm agregacji. Możemy poprzeć go tabelą liczebności i wynikiem standaryzacji.

Czwarte: te dane nie ustalają efektu przesunięcia budżetu. Brakuje nam między innymi informacji o kosztach, marży i mechanizmie kierowania ruchu. Nie mamy też losowego przydziału, który stanowiłby podstawę prostego eksperymentalnego porównania.

Zauważcie, że taki raport nadal jest użyteczny. Odbiorca dowiaduje się, dlaczego pierwszy procent nie wystarcza, jakie zjawisko występuje w danych i jakiego pytania jeszcze nie rozstrzygnięto.

Proszę teraz dopisać jeden uzasadniony następny krok. Co konkretnie zbliżyłoby nas do decyzji budżetowej?

[PAUZA: 90 sekund na odpowiedzi.]

Możemy ustalić koszt pozyskania i marżę, przejrzeć zasady kierowania klientów albo zaprojektować porównanie skutków interwencji. Ważne, żeby następny krok odpowiadał brakującej informacji. Kolejny efektowny wykres tych samych procentów nie zawsze przybliża decyzję.

W tym miejscu kończymy blok porównywania grup. Po przerwie zapytamy, co oznacza niepewność wyniku i dlaczego duża liczba wierszy nie rozwiązuje każdego problemu. Wracamy o dwunastej czterdzieści pięć.

---

## Slajd 30. Estymata i niepewność

*E · 12:45–13:30 · plan orientacyjny: 6 min*

Zacznijmy od rozróżnienia opisu i estymacji. Jeżeli pytamy, jaki odsetek sesji w naszym konkretnym eksporcie zakończył się zakupem, możemy go dokładnie policzyć. Po ustaleniu definicji i oczyszczeniu kopii licznik oraz mianownik są znane.

Jeżeli pytamy o przyszły miesiąc albo szerszą populację klientów, wykonujemy dodatkowy krok. Uogólniamy obserwacje. Potrzebujemy wtedy założeń o tym, jak dane powstały i co ma pozostać podobne w przyszłości.

Niepewność losowa dotyczy zmienności, którą uwzględnia przyjęty model próbkowania. Błąd pomiaru i obciążenie doboru to inne problemy. Przedział ufności nie obejmie ich automatycznie tylko dlatego, że został policzony przez program.

Wyobraźcie sobie bardzo duży zbiór wizyt, ale pochodzący wyłącznie od użytkowników jednego urządzenia. Możemy bardzo precyzyjnie opisać ten zbiór. Nadal nie musimy znać zachowania osób korzystających z innych urządzeń.

Wąska niepewność wokół niewłaściwie zdefiniowanej wielkości może dawać fałszywe poczucie bezpieczeństwa. Dlatego najpierw pytamy, co szacujemy. Dopiero potem wybieramy metodę liczenia niepewności.

Czy pełny eksport wszystkich sesji z ustalonego okresu potrzebuje przedziału, żeby opisać właśnie ten okres?

[PAUZA: 45 sekund.]

Sam opis zarejestrowanego okresu nie wymaga takiego uogólnienia. Przedział staje się istotny, gdy przechodzimy do wnioskowania o innym zakresie lub procesie generującym obserwacje. Na naszych sztucznych danych uczymy się techniki. Nie traktujemy jej wyniku jako dowodu dotyczącego prawdziwej kampanii.

---

## Slajd 31. Liczebność i zależność obserwacji

*E · 12:45–13:30 · plan orientacyjny: 7 min*

Mamy osiemset pięćdziesiąt sesji i czterystu dwudziestu pięciu klientów. Czy możemy po prostu potraktować każdą wizytę jako całkowicie niezależną obserwację? Tego nie należy zakładać automatycznie.

Wizyty tej samej osoby mają wspólny kontekst. Klient ma określone potrzeby, możliwości finansowe i wcześniejsze doświadczenia. Decyzja przy jednej wizycie może wpływać na następną. W realnych danych pojawia się więc potencjalna zależność wewnątrz klienta.

Jeżeli zastosujemy wzór wymagający niezależności do obserwacji silnie zależnych, ocena niepewności może być zbyt optymistyczna. Osiemset pięćdziesiąt wierszy nie musi nieść tyle samo niezależnej informacji co osiemset pięćdziesiąt odrębnych osób.

Jak można uwzględnić tę strukturę w resamplingu? Wylosować klientów, a następnie wziąć wszystkie sesje należące do każdego z nich. Jeśli klient trafi do próbki dwa razy, jego cały zestaw sesji również pojawi się dwa razy.

Uważajmy jednak na wielkość, którą liczymy. Nadal interesuje nas konwersja sesji. Nie zamieniamy jej po cichu na średnią z konwersji klientów. Klient jest jednostką losowania, a sesja jednostką wskaźnika.

[PAUZA: 60–90 sekund. Co zrobilibyście, gdyby obserwacje były dodatkowo zależne w obrębie oddziału?]

Trzeba rozważyć strukturę wynikającą z tego procesu. Losowanie klientów nie naprawia wszystkich możliwych zależności. W naszym rozszerzeniu pokażemy prosty schemat klastrowy i jawnie nazwiemy założenie o niezależności klientów. To dobry punkt wyjścia do rozmowy o doborze metody.

---

## Slajd 32. Bootstrap

*E · 12:45–13:30 · plan orientacyjny: 7 min*

Bootstrap polega na wielokrotnym tworzeniu próbek ze zwracaniem i liczeniu w każdej tej samej statystyki. Dzięki temu przybliżamy zmienność naszego estymatora na podstawie obserwowanego zbioru.

Wyobraźcie sobie pudełko z identyfikatorami klientów. Losujemy tyle identyfikatorów, ilu klientów mamy w zbiorze. Po każdym losowaniu odkładamy identyfikator do pudełka. Dlatego jedna osoba może pojawić się kilka razy, a inna nie pojawić się wcale.

Do wylosowanych klientów dołączamy ich sesje. Dla tak zbudowanej próbki liczymy konwersję A i konwersję B, a potem różnicę B minus A. Powtarzamy to wiele razy. Dostajemy rozkład różnic, które pojawiają się przy takim schemacie ponownego próbkowania.

W najprostszym wariancie percentylowym bierzemy odpowiednie kwantyle tego rozkładu. Dla dwustronnego poziomu dziewięćdziesięciu pięciu procent będą to okolice dwóch i pół oraz dziewięćdziesięciu siedmiu i pół procenta. Istnieją również inne warianty bootstrapu, z innymi własnościami.

Najważniejszy jest schemat losowania. Przy zależnych punktach szeregu czasowego dowolne mieszanie pojedynczych obserwacji może zniszczyć strukturę. Potrzebny bywa bootstrap blokowy. Przy klientach powracających rozważamy klastry.

[PAUZA: 60 sekund. Co stracilibyśmy, losując osobno każdą sesję?]

Tysiące powtórzeń nie naprawią błędnego projektu. Bootstrap nie odzyskuje też automatycznie klientów, których nigdy nie zarejestrowaliśmy, i nie zamienia porównania obserwacyjnego w eksperyment. Jest narzędziem oceny zmienności pod określonymi założeniami. W notebooku prowadzącego znajdziecie wykonywalny przykład z losowaniem klientów.

---

## Slajd 33. Przedział ufności

*E · 12:45–13:30 · plan orientacyjny: 6 min*

Poziom dziewięćdziesięciu pięciu procent w przedziale ufności opisuje własność procedury. W ujęciu częstotliwościowym wyobrażamy sobie, że wiele razy zbieramy dane według tego samego poprawnego schematu i za każdym razem wyznaczamy przedział.

Jeżeli procedura działa zgodnie z założeniami, około dziewięćdziesięciu pięciu procent tak otrzymanych przedziałów obejmowałoby prawdziwą wartość parametru. To wypowiedź o powtarzanej metodzie.

Po policzeniu jednego przedziału parametr traktujemy w tym ujęciu jako stały. Dlatego nie interpretujemy automatycznie wyniku jako dziewięćdziesięciu pięciu procent prawdopodobieństwa, że stały parametr znalazł się w tym konkretnym przedziale. Taka interpretacja wymagałaby innej konstrukcji probabilistycznej.

W zastosowaniach równie ważne jest pytanie: przedział dla czego? W naszym rozszerzeniu liczymy surową różnicę konwersji sesji B minus A. Nie liczymy przyczynowego efektu przeniesienia klientów albo pieniędzy między kanałami.

W przygotowanym rozwiązaniu ilustracyjny bootstrap klastrowy daje przedział mniej więcej od minus czterech dziesiątych do plus jedenastu i sześciu dziesiątych punktu procentowego. Dokładne wartości zależą od danych, schematu i losowania. Zapisaliśmy ziarno, żeby odtworzyć ten przykład.

Czy uwzględnienie zera dowodzi, że kanały są identyczne?

[PAUZA: 45–60 sekund.]

Nie. To nie jest dowód równości. Wynik trzeba czytać w odniesieniu do szacowanej wielkości, zakresu zgodnych z danymi wartości i założeń procedury. Ponieważ dane są syntetyczne, traktujemy ten rachunek jako naukę interpretacji, a nie informację o rzeczywistym rynku.

---

## Slajd 34. Znaczenie statystyczne i praktyczne

*E · 12:45–13:30 · plan orientacyjny: 6 min*

Precyzja oszacowania i znaczenie biznesowe to różne elementy oceny. Przy bardzo dużej próbie możemy precyzyjnie oszacować niewielką różnicę. Nadal trzeba zapytać, czy ta różnica ma praktyczne znaczenie.

Wyobraźcie sobie wzrost konwersji o jedną dziesiątą punktu procentowego. Przy milionie wizyt odpowiada to tysiącowi dodatkowych zakupów, jeżeli rozważana interpretacja i warunki rzeczywiście na takie przeliczenie pozwalają. Wartość tego efektu zależy od marży oraz kosztu zmiany.

Teraz wyobraźmy sobie różnicę pięciu punktów procentowych przy dwudziestu obserwacjach. Wygląda na dużą, ale może być bardzo niepewna. Dodatkowe dane mogą istotnie zmienić ocenę.

W raporcie potrzebujemy więc skali efektu, oceny niepewności i kryterium decyzji. Kryterium powinno wynikać z zadania. Jeżeli wdrożenie jest drogie, mała poprawa może nie pokryć kosztu. Jeżeli działanie jest tanie i odwracalne, sytuacja wygląda inaczej.

Jeśli spotkacie p-value, pamiętajcie, że nie jest ono prawdopodobieństwem prawdziwości hipotezy zerowej. Jego interpretacja dotyczy danych i przyjętego modelu pod określonym założeniem. Sam próg nie mierzy zysku ani szkody.

[PAUZA: 60–90 sekund. Podajcie przykład małej zmiany procentowej o dużym znaczeniu finansowym.]

Na dzisiejszych zajęciach najpierw pilnujemy estymandu i właściwego porównania. Nie będziemy polować na jedną liczbę, która miałaby automatycznie podjąć decyzję. Statystyka pomaga opisać dowody, a decyzja wymaga również wiedzy o konsekwencjach działania.

---

## Slajd 35. Wiele porównań

*E · 12:45–13:30 · plan orientacyjny: 6 min*

W eksploracji często sprawdzamy wiele przekrojów. Kanały, urządzenia, regiony, dni tygodnia, kategorie produktów. Im więcej kombinacji obejrzymy, tym więcej okazji, żeby przypadkowe odchylenie wyglądało interesująco.

Wyobraźmy sobie, że analizujemy setki segmentów i wybieramy tylko ten, w którym różnica jest największa. Jeśli pokażemy odbiorcy wyłącznie zwycięski wykres, może odnieść wrażenie, że właśnie ten segment był zaplanowanym przedmiotem badania.

Eksploracja jest potrzebna. Pozwala zauważyć problemy i zaproponować nowe hipotezy. Ważne jest rozróżnienie pomiędzy odkryciem pomysłu w danych a jego niezależnym potwierdzeniem.

Do potwierdzenia możemy potrzebować nowych danych, odłożonego zbioru lub wcześniej ustalonego planu, który uwzględnia wiele porównań. W zależności od zadania istnieją różne procedury kontroli błędów. Sama zmiana nazwy pliku na „analiza końcowa” nie zmienia sposobu, w jaki znaleźliśmy wynik.

Jeżeli po analizie odkryliśmy interesującą różnicę wyłącznie w jednym segmencie, uczciwie powiedzmy: to hipoteza wyłoniona podczas eksploracji. Odbiorca ma wtedy szansę właściwie ocenić jej status.

[PAUZA: 60 sekund. Jak opisalibyście zakres poszukiwań w krótkim raporcie?]

Możemy wymienić sprawdzone przekroje, oddzielić planowane analizy od dodatkowych i wskazać, które obserwacje wymagają potwierdzenia. Dzięki temu nie ukrywamy ścieżki wyboru wyniku. To ma szczególne znaczenie wtedy, gdy na podstawie analizy ktoś zamierza zmienić proces lub wydać pieniądze.

---

## Slajd 36. Analiza wrażliwości

*E · 12:45–13:30 · plan orientacyjny: 7 min*

Analiza wrażliwości pyta, od jakich decyzji zależy nasz wniosek. Nie chodzi o znalezienie takiej wersji rachunku, która da najbardziej atrakcyjny rezultat. Chodzi o sprawdzenie jego stabilności przy uzasadnionych alternatywach.

Możemy zacząć od dużych zamówień. Czy różnica średnich wynika głównie z kilku transakcji? Porównajmy pełny rozkład, mediany i wynik po jawnie opisanym ograniczeniu ogona. Jeżeli wniosek mocno się zmienia, powinniśmy to pokazać.

Możemy też sprawdzić okresy i segmenty. Czy opis utrzymuje się w obu grupach urządzeń? Czy wybrany tydzień zachowuje się podobnie do pozostałych? W naszym przykładzie właśnie segmentacja ujawniła odwrócenie porównania.

Kolejna kwestia to jednostka. Analiza klienta może dać inny obraz niż analiza sesji. Tego nie należy przedstawiać jako prostej korekty tej samej liczby. To odpowiedź na inne pytanie, którą warto postawić obok pierwszej.

Możemy wreszcie pytać o alternatywne wyjaśnienie. Czy taką samą obserwację da się uzyskać przez inny skład ruchu albo błąd połączenia? Jeśli tak, jaki dodatkowy test pozwoli te możliwości rozróżnić?

[PAUZA: 90 sekund. Wybierzcie jedną kontrolę, która mogłaby osłabić waszą pierwszą intuicję o kanale B.]

Dobra analiza pozwala zobaczyć zarówno wynik, jak i jego zależność od założeń. Nie musimy udawać, że jeden rachunek wyczerpuje temat. Odbiorca powinien wiedzieć, które elementy są stabilne, a które szczególnie wrażliwe na konstrukcję zbioru i wybór populacji.

---

## Slajd 37. Zbiór do predykcji na wejściu

*F · 13:30–14:15 · plan orientacyjny: 6 min*

Przygotujmy teraz dane do innego zadania. Chcemy przewidzieć zakup w chwili rozpoczęcia sesji. Na razie nie wybieramy modelu. Budujemy tabelę, która wiernie odtworzy informacje dostępne systemowi w tym momencie.

W każdym wierszu musimy wskazać chwilę prognozy. U nas będzie nią started_at. Wynik, czyli zakup podczas sesji, poznamy później. To normalne: dane treningowe zawierają późniejszą etykietę, ale cechy wejściowe powinny odpowiadać wcześniejszemu stanowi wiedzy.

Jakie informacje możemy rozważyć? Urządzenie, kanał wejścia przy ustalonej definicji atrybucji i historię klienta sprzed obecnej wizyty. Możemy policzyć liczbę wcześniejszych sesji albo wcześniejsze zakupy, o ile naprawdę były już dostępne.

Nie możemy użyć końcowej wartości bieżącego zamówienia do przewidywania, czy to zamówienie powstanie. Nie możemy też wykorzystać zwrotu, który wydarzy się kilka dni później.

Załóżmy, że ktoś przekazuje wam gotową tabelę z kolumną „łączna liczba zakupów klienta”. Jakie pytanie zadacie?

[PAUZA: 45–60 sekund.]

Do jakiego momentu policzono tę liczbę? Jeżeli obejmuje cały okres po dacie prognozy, zawiera przyszłość. Nazwa kolumny wygląda niewinnie, a problem tkwi w konstrukcji czasowej.

Przygotowanie zbioru do predykcji polega więc na odtworzeniu historycznego stanu wiedzy. Dzięki temu późniejsza ocena modelu będzie bliższa temu, czego możemy oczekiwać podczas rzeczywistego użycia. Sam algorytm nie naprawi zbioru, do którego wcześniej wprowadziliśmy przyszły wynik.

---

## Slajd 38. Historia klienta z datą odcięcia

*F · 13:30–14:15 · plan orientacyjny: 6 min*

Prześledźmy jednego klienta. Odwiedza sklep pierwszego, piątego i dziewiątego listopada. W wierszu z pierwszego listopada liczba wcześniejszych sesji wynosi zero. Piątego listopada wynosi jeden. Dziewiątego wynosi dwa.

To bardzo prosta cecha, ale już wymaga czasu. Jeśli policzymy wszystkie sesje klienta w całym eksporcie i dołączymy wynik do każdej jego wizyty, wpiszemy mu pełną historię także w pierwszym dniu. System dostanie wiedzę o przyszłych powrotach.

Przy liczniku poprzednich sesji możemy posortować dane po kliencie i czasie, a następnie użyć cumcount. Przy historii zakupów potrzebujemy również wyłączenia bieżącego wyniku. Samo sortowanie nie wystarczy, jeśli agregacja uwzględni aktualny wiersz.

Wyobraźcie sobie, że pierwszy zakup następuje podczas wizyty piątego listopada. Na początku tej wizyty klient nie ma jeszcze wcześniejszego zakupu. Informacja o zakupie z tej samej sesji należy do późniejszej etykiety.

Co z nowym klientem? Potrzebujemy jawnej wartości początkowej i ewentualnej informacji, że historii nie ma. Brak wcześniejszych zakupów i brak możliwości rozpoznania klienta mogą oznaczać różne sytuacje.

[PAUZA: 90 sekund. Rozpiszcie trzy wizyty i licznik historii dostępnej na wejściu.]

Jeszcze jedna uwaga: jeśli zdarzenia mają identyczny czas, kolejność w pliku nie tworzy automatycznie kolejności ich dostępności. Potrzebujemy reguły wynikającej ze źródła. W przygotowanym ćwiczeniu czasy sesji są różne, żebyśmy mogli skupić się na podstawowym mechanizmie.

---

## Slajd 39. Podział danych wynika z zastosowania

*F · 13:30–14:15 · plan orientacyjny: 7 min*

Sposób podziału danych powinien odpowiadać przyszłemu zastosowaniu. Nie ma jednego podziału, który bez dodatkowych pytań rozwiązuje każde zadanie.

Jeżeli system ma przewidywać przyszłe sesje, naturalnym punktem wyjścia jest rozdzielenie po czasie. Uczymy się na wcześniejszym okresie i oceniamy późniejszy. Musimy przy tym uważać, żeby także cechy dla późniejszych obserwacji odtwarzały wiedzę dostępną w chwili prognozy.

Jeśli pytamy o zupełnie nowych klientów, pojawia się inny wymóg. Klienci testowi nie powinni występować w treningu. W przeciwnym razie ocena może częściowo korzystać ze znajomości tych samych osób.

Ale obecność klienta w obu okresach nie zawsze jest błędem. Jeżeli w produkcji obsługujemy przyszłe wizyty naszych obecnych klientów, taki układ może odpowiadać zadaniu. Trzeba jedynie poprawnie rozdzielić czas i dostępność historii.

Wyobraźcie sobie bank albo serwis abonamentowy. Wiele przyszłych decyzji dotyczy tych samych osób. Test wyłącznie na nowych klientach odpowiadałby wtedy ważnemu, ale innemu pytaniu niż ocena całej przyszłej populacji.

[PAUZA: 60–90 sekund. Kiedy wybralibyście podział po kliencie, a kiedy po czasie?]

W realnym projekcie można potrzebować kilku ocen: dla przyszłych wizyt obecnych klientów i osobno dla nowych osób. Dziś nie trenujemy jeszcze klasyfikatora. Ustalamy, jak zaprojektować tabelę i sprawdzian, aby następne zajęcia mogły rozpocząć się od wiarygodnej podstawy.

---

## Slajd 40. Przekształcenia uczone na treningu

*F · 13:30–14:15 · plan orientacyjny: 7 min*

Niektóre przekształcenia mają parametry uczone z danych. Imputacja medianą wymaga policzenia mediany. Skalowanie wymaga poznania odpowiednich charakterystyk. Wybór cech może korzystać z zależności zaobserwowanych w zbiorze.

Jeżeli oceniamy model na odłożonych danych, parametry tych operacji dopasowujemy na treningu. Test przechodzi przez te same, wcześniej ustalone przekształcenia. Nie używamy go do ich ponownego dopasowania.

Dlaczego? Chcemy odtworzyć sytuację, w której nowa obserwacja trafia do już przygotowanego procesu. Jeżeli mediana powstanie z całej tabeli, wykorzystamy również rozkład przyszłych obserwacji testowych. Nawet bez odczytania ich etykiet przenosimy informację przez granicę oceny.

Nie każdy taki błąd dramatycznie zmieni wynik. Nadal jednak procedura przestaje odpowiadać temu, co zadeklarowaliśmy. Przy doborze cech lub wielu próbach może to prowadzić do bardzo optymistycznej oceny.

Do uporządkowania kolejnych kroków służy pipeline. Łączy przekształcenia z modelem i pomaga zachować właściwe dopasowanie wewnątrz kolejnych podziałów danych.

Teraz ważne doprecyzowanie. Jeśli przygotowujemy czysto opisowy raport o zarejestrowanym miesiącu, nie musimy sztucznie dzielić go na trening i test. Mówimy tutaj o ocenie procesu, który ma działać na nowych danych.

[PAUZA: 60 sekund. Czy policzenie średniego wieku całego miesiąca do raportu opisowego jest tym samym co użycie tej średniej do przygotowania testu modelu?]

To różne zadania. Regułę stosujemy do celu analizy, a nie mechanicznie do każdej operacji na tabeli.

---

## Slajd 41. Kod analizy i weryfikacja przez człowieka

*F · 13:30–14:15 · plan orientacyjny: 6 min*

W tej pracy może pomagać asystent AI. Może zaproponować kod, podsunąć kontrolę albo pomóc sformułować konkurencyjne hipotezy. Nadal musimy sprawdzić, co dokładnie policzył.

Dobry komunikat do takiego narzędzia może brzmieć: mam jeden wiersz na sesję, chcę policzyć konwersję kanałów, pokaż osobno liczniki i mianowniki, a potem rozbij wynik po urządzeniu. Sprawdź unikalność klucza i zachowanie liczby wierszy po połączeniu.

Taki opis daje narzędziu konkretny cel i ograniczenia. Jeśli napiszemy tylko „zrób analizę sprzedaży”, otrzymamy być może efektowny kod, ale niekoniecznie odpowiedź na nasze pytanie.

Co trzeba szczególnie sprawdzić? Czy program nie usunął kolejnych wizyt po identyfikatorze klienta? Czy nie policzył zwykłej średniej z procentów grup? Czy inner join nie wykluczył części sesji? Czy cecha nie zawiera informacji z przyszłości?

Wygenerowany komentarz może brzmieć bardzo pewnie. Dowód wyniku powinien jednak prowadzić do uruchomionego rachunku, który umiemy skontrolować. W naszym przykładzie wystarczą cztery grupy, liczniki i mianowniki, żeby sprawdzić główny mechanizm.

[PAUZA: 60–90 sekund. Jakie jedno polecenie kontrolne dopisalibyście do odpowiedzi asystenta?]

Możemy poprosić o asercję liczby sesji, o tabelę liczebności albo o wskazanie dokładnej definicji wskaźnika. To konkretny sposób używania AI w analizie: narzędzie przyspiesza zapis i poszukiwanie, a my pilnujemy znaczenia danych oraz granic wniosku.

---

## Slajd 42. Raport z analizy

*F · 13:30–14:15 · plan orientacyjny: 6 min*

Dobry raport da się zrozumieć bez czytania całego notebooka. Powinien wskazać pytanie, jednostkę obserwacji i zakres danych. Odbiorca musi wiedzieć, czy analizujemy sesje, klientów, czy zamówienia.

Następnie krótko opisujemy przekształcenia, które mają wpływ na wynik. W naszym przypadku usunęliśmy potwierdzone kopie sesji, uporządkowaliśmy słownik klientów i zachowaliśmy osiemset pięćdziesiąt wizyt po połączeniu. Dwie nieznane kwoty ujawniamy w analizie wartości zakupów.

Wynik przedstawiamy razem z licznikami i mianownikami. Pokazujemy agregat oraz ważną kontrolę w segmentach. Dzięki temu odbiorca widzi, że B ma wyższą konwersję ogółem, ale A wyższą w obu grupach urządzeń.

Potem nazywamy ograniczenie. W naszym przykładzie dane obserwacyjne nie ustalają efektu przesunięcia budżetu. Nie znamy też wszystkich elementów potrzebnych do oceny opłacalności.

Na końcu proponujemy następny krok powiązany z tym ograniczeniem. Może to być zebranie kosztów albo projekt badania interwencji. Unikamy rekomendacji, która nie wynika z wykonanej analizy.

[PAUZA: 90 sekund. Spróbujcie powiedzieć taki raport w czterech zdaniach.]

Zauważcie, że nie opowiadamy odbiorcy kolejno każdej instrukcji kodu. Pokazujemy decyzje i dowody potrzebne do oceny wniosku. Szczegóły techniczne pozostają dostępne w notebooku. Raport i kod pełnią różne role, ale powinny opisywać ten sam rachunek i tę samą populację.

---

## Slajd 43. Przygotowanie do warsztatu

*F · 13:30–14:15 · plan orientacyjny: 7 min*

Przygotujmy warsztat. W folderze znajdziecie plik sesje.csv, słownik klienci.csv oraz notebook studenta. Rozwiązanie prowadzącego jest osobnym plikiem. Na początku samodzielnej pracy korzystajcie z wersji studenckiej.

Jeżeli pracujecie lokalnie w Jupyter, umieśćcie oba pliki CSV obok notebooka. W Colab trzeba dodatkowo przesłać CSV do bieżącego środowiska. Samo otwarcie notebooka nie przenosi automatycznie plików z komputera.

Nie potrzebujemy kluczy API ani zewnętrznych źródeł. Dane są małe i syntetyczne. Dzięki temu możemy skupić się na poprawności analizy, a każdy główny wynik sprawdzić także prostym rachunkiem.

Warsztat ma pięć etapów. Najpierw audyt, potem czyszczenie i połączenie, następnie eksploracja, porównanie po urządzeniach oraz ocena dostępności cech. Dla osób, które skończą wcześniej, jest rozszerzenie z bootstrapem klientów.

Na końcu oddajecie tabelę porównań, jeden czytelny wykres i cztery zdania. Pytanie o budżet pojawi się w podsumowaniu, ale nie musicie na siłę wybierać kanału. Wasza odpowiedź ma odpowiadać temu, co rzeczywiście ustaliliście.

Jeżeli środowisko nie działa, zgłoście to od razu. Możecie pracować w parze. Część porównania da się także policzyć w arkuszu, bo liczniki i mianowniki pozostają te same.

[PAUZA: 2 minuty na kontrolę plików i uruchomienie pierwszej komórki.]

Teraz przerwa. Wracamy o czternastej trzydzieści. Po powrocie zaczynamy od obejrzenia surowych danych, bez automatycznego usuwania braków i powtórzeń.

---

## Slajd 44. Ćwiczenie 1 · audyt plików

*WARSZTAT · 14:30–16:00 · plan orientacyjny: 10 min*

Zaczynamy od audytu. Otwórzcie oba pliki i obejrzyjcie pierwsze wiersze. Proszę jeszcze niczego nie poprawiać. Najpierw chcemy wiedzieć, jaki obiekt otrzymaliśmy.

Ustalcie, co oznacza jeden wiersz w tabeli sesji i które pole powinno go identyfikować. Policzcie liczbę wszystkich wierszy oraz liczbę unikalnych identyfikatorów sesji. To samo zróbcie dla klientów w słowniku.

Następnie obejrzyjcie typy, nieznane wartości i przykłady zapisów kwot. Zapiszcie trzy obserwacje. Na tym etapie interesuje mnie rozpoznanie problemu, a nie jak najszybsze usunięcie wszystkich wierszy, które wyglądają nietypowo.

Macie dziesięć minut. Jeżeli znajdziecie powtórzenia klienta w tabeli sesji, przypomnijcie sobie różnicę między kolejną wizytą a techniczną kopią.

[PRACA STUDENTÓW: około 7 minut.]

Sprawdźmy wyniki. Surowy plik sesji ma osiemset sześćdziesiąt dwa wiersze i osiemset pięćdziesiąt unikalnych sesji. W słowniku mamy czterysta dwadzieścia sześć wierszy i czterystu dwudziestu pięciu klientów.

Czy sam ten wynik dowodzi już, że wszystkie powtórzenia wolno usunąć? Jeszcze potrzebujemy sprawdzenia zgodności ich treści. W tym przygotowanym przykładzie kopie są identyczne, ale chcę, żeby reguła postępowania była świadoma.

Jeśli ktoś zastosował dropna do całej tabeli, zatrzymajmy się na chwilę. Która brakująca informacja jest potrzebna do konwersji kanałów? Wiek nie jest warunkiem uwzględnienia sesji w tym zadaniu. Następny etap to poprawienie rozpoznanych problemów przy zachowaniu naszej populacji.

---

## Slajd 45. Ćwiczenie 2 · budowa zbioru

*WARSZTAT · 14:30–16:00 · plan orientacyjny: 20 min*

Teraz budujemy zbiór analityczny. Po sprawdzeniu identyczności kopii zachowajcie po jednej obserwacji na sesję. Oryginalny zapis kwoty pozostawcie w osobnej kolumnie. Dopiero obok utwórzcie wersję liczbową.

W zapisie z przecinkiem rozpoznajcie separator dziesiętny. Teksty, które nie dają się odczytać jako kwota, oznaczcie jako nieznane. Nie zamieniajcie ich w zera. Zero ma już w naszym zbiorze określone znaczenie: brak zakupu podczas sesji.

Przy połączeniu ze słownikiem zadeklarujcie relację many_to_one. Najpierw zobaczcie, czy słownik ją spełnia. Jeżeli pojawi się błąd, sprawdźcie powtórzenia klienta. W tym ćwiczeniu identyczną kopię można uporządkować po potwierdzeniu zgodności.

Wykonajcie left join z kontrolą dopasowań. Na końcu chcę zobaczyć dwie rzeczy: osiemset pięćdziesiąt wierszy oraz unikalny klucz sesji. Sprawdźcie również, czy wszystkie sesje znalazły klienta w słowniku.

Macie dwadzieścia minut.

[PRACA STUDENTÓW: około 15 minut.]

Omówmy kontrole. Po połączeniu ma zostać osiemset pięćdziesiąt sesji i pełne dopasowanie do słownika. Dwie kwoty powinny być nieznane. Przy sesjach bez zakupu kwota wynosi zero, a przy zakupach jest dodatnia albo nieznana.

Jeżeli liczba wierszy wzrosła, sprawdźcie unikalność słownika. Jeżeli spadła, sprawdźcie rodzaj join i filtry. Proszę poprawiać przyczynę, a nie dopasowywać końcową liczbę przez przypadkowe usuwanie wierszy. Za chwilę na tej tabeli policzymy pierwszy raport.

---

## Slajd 46. Ćwiczenie 3 · eksploracja

*WARSZTAT · 14:30–16:00 · plan orientacyjny: 15 min*

Przejdźcie do eksploracji. Najpierw wybierzcie sesje zakończone zakupem i opiszcie ich kwoty. Podajcie liczbę zakupów, liczbę znanych kwot, średnią, medianę oraz kilka kwantyli. Narysujcie histogram z podpisaną jednostką.

Dużych, poprawnych transakcji nie usuwamy automatycznie. Jeśli chcecie pokazać dodatkowy widok bez górnego ogona, nazwijcie go osobno i wyjaśnijcie filtr. Główny wynik powinien pozostać możliwy do odtworzenia.

Potem policzcie tabelę kanałów. Potrzebujemy liczby sesji, liczby zakupów i konwersji. Brak kwoty nie usuwa zakupu z licznika, jeżeli converted jest znane. Wskaźnik opiera się tutaj na wyniku zakupowym, a nie na kompletności ceny.

Macie piętnaście minut.

[PRACA STUDENTÓW: około 11 minut.]

Sprawdźmy klucz. Mamy pięćset siedemdziesiąt osiem sesji z zakupem. Znanych kwot jest pięćset siedemdziesiąt sześć. Dwie pozostają nieznane. Średnia znanych kwot wynosi około dwustu dziewięćdziesięciu pięciu złotych i pięćdziesięciu dziewięciu groszy. Mediana to sto dziewięćdziesiąt trzy złote i sześć groszy.

Kanał A ma trzysta piętnaście zakupów na czterysta osiemdziesiąt sesji. Kanał B ma dwieście sześćdziesiąt trzy na trzysta siedemdziesiąt. Jeśli wasze liczby są inne, wróćcie do deduplikacji, połączenia i mianownika.

Proszę teraz opisać różnicę między średnią i medianą jednym zdaniem odnoszącym się do rozkładu. Następnie przejdziemy do sprawdzenia, co ukrywa wynik ogółem.

---

## Slajd 47. Ćwiczenie 4 · sprzeczne porównanie

*WARSZTAT · 14:30–16:00 · plan orientacyjny: 20 min*

Rozbijcie konwersję jednocześnie po kanale i urządzeniu. Chcę zobaczyć cztery grupy, a w każdej liczbę sesji i liczbę zakupów. Sam gotowy procent nie wystarczy do sprawdzenia rachunku.

Następnie policzcie udział urządzeń wewnątrz każdego kanału. Później przyjmijcie wspólne wagi: połowa desktopu i połowa mobile. Na ich podstawie obliczcie standaryzowany wynik A i B.

Na końcu zapiszcie dwa zdania wyjaśnienia. Pierwsze ma opisać, co stało się z porównaniem. Drugie ma wskazać mechanizm. Proszę nie używać samego hasła „paradoks Simpsona” jako zamiennika wyjaśnienia.

Macie dwadzieścia minut.

[PRACA STUDENTÓW: około 14 minut.]

Sprawdźmy tabelę. Desktop A: osiemdziesiąt jeden na dziewięćdziesiąt, czyli dziewięćdziesiąt procent. Desktop B: dwieście osiem na dwieście sześćdziesiąt, czyli osiemdziesiąt procent. Mobile A: dwieście trzydzieści cztery na trzysta dziewięćdziesiąt, czyli sześćdziesiąt procent. Mobile B: pięćdziesiąt pięć na sto dziesięć, czyli pięćdziesiąt procent.

Przy wspólnych wagach otrzymujemy siedemdziesiąt pięć procent w A i sześćdziesiąt pięć w B. Różna struktura urządzeń wyjaśnia, dlaczego wynik ogółem wskazywał wcześniej B.

Czy ktoś zapisał, że A powoduje wzrost zakupów? Jeśli tak, doprecyzujmy: ustaliliśmy opis różnic wewnątrz grup. Nie zidentyfikowaliśmy efektu przyczynowego przełączenia klienta albo zmiany budżetu. Tę granicę proszę zachować w końcowym raporcie.

---

## Slajd 48. Ćwiczenie 5 · granice użycia kolumn

*WARSZTAT · 14:30–16:00 · plan orientacyjny: 15 min*

Ostatnie zadanie dotyczy dostępności informacji. Wyobraźcie sobie, że model ma wydać prognozę dokładnie przy wejściu klienta. Oceńcie trzy kolumny: session_seconds, order_value_pln i refund_pln.

Przy każdej napiszcie, kiedy znamy jej wartość w obecnej definicji. Następnie zaproponujcie jedną cechę z wcześniejszej historii klienta, która może być dostępna na wejściu. Zwróćcie uwagę na datę odcięcia.

Dla osób, które mają już podstawowy raport, jest rozszerzenie: bootstrap klastrowy. Losujcie klientów, zachowujcie ich sesje razem i liczcie różnicę konwersji sesji B minus A. Nazwijcie założenie o niezależności klientów. To zadanie dodatkowe.

[PRACA STUDENTÓW: około 10 minut.]

Sprawdźmy pierwszą część. Długość całej sesji poznajemy po jej przebiegu. Końcowa wartość zamówienia wiąże się z późniejszym wynikiem zakupowym. Kwota zwrotu opisuje jeszcze późniejsze zdarzenie. W tej postaci żadna z tych kolumn nie jest dostępna na samym wejściu.

Możemy natomiast policzyć liczbę wcześniejszych wizyt. Dla kolejnych sesji jednego klienta otrzymamy zero, jeden, dwa i tak dalej, zgodnie z chronologią. Nie liczymy całej przyszłej historii i nie wstawiamy jej do pierwszego wiersza.

W rozszerzeniu bootstrapowym nadal szacujemy surową różnicę wskaźników sesji. Resampling klientów uwzględnia określoną strukturę zależności, ale nie nadaje wynikowi interpretacji przyczynowej. Proszę teraz przygotować krótki końcowy komentarz. Za chwilę usłyszymy dwa zespoły.

---

## Slajd 49. Oddanie i omówienie

*WARSZTAT · 14:30–16:00 · plan orientacyjny: 10 min*

Poproszę o końcową tabelę: kanał, urządzenie, licznik, mianownik i odsetek. Do tego jeden wykres, na którym widać jednostkę i zakres porównania. Ostatni element to cztery zdania: wynik ogółem, wynik w segmentach, ograniczenie i następny krok.

Zaczniemy od dwóch zespołów. Każdy ma około półtorej minuty. Proszę powiedzieć przede wszystkim, co ustaliliście, a nie odczytywać kolejne instrukcje Pythona.

[PREZENTACJE DWÓCH ZESPOŁÓW: około 3 minut.]

Przykładowy komentarz brzmi tak. W analizowanym eksporcie B ma konwersję około siedemdziesięciu jeden procent, a A około sześćdziesięciu sześciu. W obu grupach urządzeń A ma wynik wyższy o dziesięć punktów procentowych, a różne udziały urządzeń odwracają agregat. Dane obserwacyjne i brak kosztów nie pozwalają ustalić efektu oraz opłacalności przesunięcia budżetu. Następnym krokiem będzie uzupełnienie informacji ekonomicznych i zaprojektowanie porównania odpowiadającego planowanej interwencji.

Przy ocenie ćwiczenia liczy się jednostka, poprawny mianownik, kontrola czyszczenia i połączenia, właściwy rachunek oraz granice wniosku. To propozycja kryteriów dla dzisiejszego zadania, a nie zmiana formalnych zasad zaliczenia przedmiotu.

Najważniejsze, co chciałbym wam zostawić po tych zajęciach, to nawyk sprawdzania znaczenia każdej liczby. Co jest wierszem? Skąd bierze się mianownik? Co zrobiło połączenie tabel? Kiedy informacja była dostępna? Na jakie pytanie odpowiada wynik?

Na kolejnych warsztatach możemy rozbudować tę analizę o historię klientów, dodatkowe przekroje i przygotowanie cech. Dzisiaj wykonaliście pełną drogę od surowego eksportu do komentarza, który inna osoba potrafi sprawdzić.

---

## Slajd 50. Dokumentacja techniczna

*ANEKS · źródła · plan orientacyjny: 0 min*

Na końcu zostawiam dokumentację narzędzi wykorzystanych w przykładach. W pandas warto wrócić do łączenia tabel i obsługi brakujących danych. W dokumentacji scikit-learn przydatny jest rozdział o typowych błędach oraz właściwym przygotowaniu procesu modelowania. Opis bootstrapu w SciPy pokazuje również, że istnieją różne warianty tej procedury.

Nie musicie uczyć się wszystkich wywołań na pamięć. Ważniejsze jest rozumienie, co mają sprawdzić. Jeśli zmienicie narzędzie, nadal będzie trzeba kontrolować klucz, mianownik, dostępność informacji i sens porównania.

Przypomnę jeszcze, że wszystkie dane kanałów i dzisiejsze liczby przygotowaliśmy jako przykład syntetyczny. Grafiki w prezentacji są metaforami tematów. Wyniki analizy znajdują się w tabelach, wykresach i wykonywalnym notebooku.

Dziękuję. Zostawmy chwilę na ostatnie pytania o rachunek, interpretację albo pracę w notebooku.

[PYTANIA KOŃCOWE: według dostępnego czasu. Slajd źródłowy nie wydłuża osobno harmonogramu.]

---

## Źródła techniczne

- https://pandas.pydata.org/docs/user_guide/merging.html
- https://pandas.pydata.org/docs/user_guide/missing_data.html
- https://scikit-learn.org/stable/common_pitfalls.html
- https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.bootstrap.html

Wartości kanałów, statystyki koszyków i przykład bootstrapu dotyczą danych syntetycznych z pakietu ćwiczeń. Fragment o czasie sesji na slajdzie 27 jest przykładem hipotetycznym, nie wynikiem analizy wygenerowanej kolumny session_seconds.
