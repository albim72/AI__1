# AI w biznesie II. Od ewolucji do sztucznej sprawczości
**Scenariusz wykładu: 77 slajdów.** Tekst do wygłoszenia, zgodny z numeracją prezentacji PowerPoint. Przykłady biznesowe są ilustracjami dydaktycznymi; instrukcje sceniczne ujęto w nawiasy kwadratowe.

## Slajd 01. Od ewolucji do sztucznej sprawczości
*Prolog*

Dzień dobry Państwu. Na poprzednim wykładzie budowaliśmy mapę sztucznej inteligencji. Dzisiaj chciałbym tę mapę odłożyć i zapytać o coś znacznie bardziej fundamentalnego: skąd bierze się zdolność systemu do znajdowania rozwiązań, których nikt wcześniej nie zaprojektował w szczegółach? Zaczniemy nie od komputera, ale od życia. Od organizmów, które przez kolejne pokolenia zmieniały się pod wpływem warunków środowiska.

Nie będę twierdził, że współczesna sztuczna inteligencja jest żywym organizmem. Interesuje mnie podobieństwo pewnych mechanizmów: powstawanie wariantów, ocena ich skutków, zachowywanie tego, co się sprawdza, oraz powtarzanie procesu. Zobaczymy, jak człowiek wykorzystał tę logikę w obliczeniach, jak buduje i trenuje modele, a następnie jak przekazuje systemom możliwość działania.

Na końcu zadamy pytanie, które wykracza poza technologię. Jeżeli coraz więcej decyzji będzie wynikiem działania zaprojektowanych przez nas systemów, kto będzie kształtował środowisko, w którym sami podejmujemy decyzje? To będzie wykład o AI, ale w równym stopniu o organizacjach i o człowieku.

## Slajd 02. Osiem aktów. Jedna idea: selekcja.
*Prolog*

Proszę spojrzeć na osiem aktów naszego dzisiejszego spotkania. Nie jest to osiem niezależnych tematów. Każdy z nich odpowiada na pytanie pozostawione przez poprzedni. Biologia pokaże nam, jak bez centralnego planu powstają złożone adaptacje. Algorytmy ewolucyjne pokażą, co się dzieje, kiedy konstruujemy podobny mechanizm celowo. Heurystyki pozwolą nam zrozumieć, dlaczego zarówno człowiek, jak i maszyna potrzebują skrótów.

Później otworzymy zaplecze współczesnego AI. Zobaczymy, że Python jest tylko drzwiami do całego ekosystemu danych, bibliotek, infrastruktury i procedur selekcji modeli. Następnie przejdziemy od modelu, który odpowiada, do agenta, który może wykonać operację, i do systemów złożonych z wielu współpracujących jednostek.

Ostatnie dwa akty będą celowo inne. Będziemy rozbierać na części to, czego nie widać w oknie rozmowy, a co ma fundamentalne znaczenie dla biznesu. Proszę przez cały wykład pamiętać o jednym pytaniu: co w danym systemie jest nagradzane, przez kogo i z jakim skutkiem?

## Slajd 03. Inteligencja przed komputerem
*I · Biologia*

Zanim powstały komputery, zanim powstał język, a nawet zanim istniały układy nerwowe, życie już podlegało procesom, które zmieniały jego zdolność funkcjonowania w środowisku. To niezwykle ważne, ponieważ zwykle myślimy, że złożony rezultat musi być konsekwencją złożonego projektu. Ewolucja biologiczna pokazuje, że nie zawsze tak jest.

Wyobraźmy sobie powstawanie skrzydła, oka albo niezwykle skomplikowanych zachowań owadów społecznych. Nie trzeba zakładać, że istniał biologiczny plan końcowego rozwiązania, który organizmy konsekwentnie realizowały. Wystarczy, że w kolejnych pokoleniach występują dziedziczne różnice, a niektóre z nich wpływają na sukces reprodukcyjny. Proces może kumulować zmiany.

Nie utożsamiam tu adaptacji z myśleniem. Bakteria odporna na antybiotyk nie musi rozumieć antybiotyku. Właśnie to jest fascynujące: skuteczne dostosowanie może powstać bez świadomego rozumienia problemu. Za chwilę zobaczymy, że w informatyce możemy projektować mechanizmy poszukiwania, które również nie potrzebują semantycznego zrozumienia zadania.

## Slajd 04. Życie nie powstało po to, by myśleć
*I · Biologia*

Czy oko powstało dlatego, że organizmy potrzebowały widzieć? To brzmi intuicyjnie, ale odwraca kierunek wyjaśnienia. Potrzeba sama w sobie nie tworzy odpowiedniej dziedzicznej cechy. W populacji istnieje zmienność. Część tej zmienności jest dziedziczna. Jeżeli określona cecha w danych warunkach zwiększa względny sukces reprodukcyjny, jej częstość może rosnąć w kolejnych pokoleniach.

Zmienność oznacza, że organizmy nie są identyczne. Dziedziczenie oznacza, że część ich właściwości jest przekazywana potomstwu. Selekcja oznacza, że nie wszystkie warianty pozostawiają taką samą liczbę potomków. To trzy składniki, które pozwalają zrozumieć mechanizm doboru naturalnego. Nie jest to pełny opis ewolucji, bo istnieją także inne procesy, ale jest to punkt wyjścia.

Ważne jest również rozróżnienie skali czasu. Osobnik może nauczyć się nowego zachowania w ciągu życia. Ewolucja biologiczna dotyczy zmian dziedzicznych właściwości populacji przez pokolenia. W biznesie będziemy używać obu analogii, ale nie będziemy ich mylić. Zmiana pracownika i zmiana struktury całej organizacji to dwa różne procesy.

## Slajd 05. Nie wygrywa najsilniejszy. Wygrywa dopasowany.
*I · Biologia*

Sformułowanie, że w ewolucji wygrywa najsilniejszy, jest bardzo mylące. Najsilniejszy pod jakim względem? Szybkości, wielkości, odporności na głód, liczby potomstwa? Bez wskazania środowiska takie pytanie nie ma sensownej odpowiedzi. Cecha, która pomaga w jednym otoczeniu, może stać się obciążeniem w innym.

Weźmy bakterie i antybiotyk. Jeżeli w populacji istnieją warianty odporne, po zastosowaniu antybiotyku mogą mieć przewagę reprodukcyjną. Nie oznacza to, że każda bakteria dowiedziała się, czego od niej oczekujemy, i celowo skonstruowała mechanizm odporności. Zmieniliśmy warunki selekcji.

Przenieśmy tę obserwację do biznesu. Firma zoptymalizowana pod sprzedaż stacjonarną może być wysoce efektywna w stabilnym otoczeniu. Kiedy rynek przesuwa się w stronę zakupów internetowych, jej dotychczasowe zasoby i procedury mogą utrudniać zmianę. Nie dlatego, że nagle wszyscy pracownicy stali się mniej kompetentni. Zmieniło się środowisko oceny ich działań. Dlatego nie pytajmy wyłącznie, czy rozwiązanie jest dobre. Pytajmy, w jakich warunkach jest dobre.

## Slajd 06. Mutacja: przypadek nie jest przeciwieństwem porządku
*I · Biologia*

Mutacja kojarzy nam się z czymś wyjątkowym, spektakularnym, czasem nawet z deformacją. Tymczasem w ewolucji jest jednym ze źródeł zmienności. Jej wystąpienie nie jest na ogół podporządkowane aktualnemu zapotrzebowaniu organizmu. To nie znaczy, że wszystkie mutacje są jednakowo prawdopodobne. Znaczy, że nie są zamawiane przez przyszły cel adaptacyjny.

Ta sama zmiana może być neutralna, szkodliwa albo korzystna, zależnie od kontekstu. Jeśli jest dziedziczna, może uczestniczyć w procesach prowadzących do zmiany populacji. Rekombinacja może łączyć istniejące warianty, przepływ genów wprowadzać warianty z innych populacji, a dryf zmieniać ich częstości bez przewagi adaptacyjnej.

Dla algorytmów to bardzo ciekawa lekcja. Jeżeli mamy rozwiązanie i nigdy nie pozwolimy na żadne odstępstwo od niego, zamkniemy przestrzeń poszukiwań. Jeśli natomiast będziemy zmieniać wszystko bez jakiejkolwiek oceny, otrzymamy chaos. Siła mechanizmu polega na połączeniu generowania zmian z oceną ich konsekwencji. Zmienność sama nie jest inteligencją, ale może być surowcem procesu poszukiwania.

## Slajd 07. Dryf: przypadek może zmienić historię
*I · Biologia*

Nie każda cecha, którą obserwujemy w populacji, musi być najlepszym możliwym rozwiązaniem. To jedna z najważniejszych korekt naiwnego myślenia o ewolucji. Wyobraźmy sobie niewielką populację, w której istnieją dwa neutralne warianty. Czysto przypadkowo osobniki z jednym wariantem mogą pozostawić więcej potomstwa. Po wielu pokoleniach drugi wariant może zniknąć, mimo że nie był gorszy adaptacyjnie.

Nazywamy to dryfem genetycznym. Szczególnie wyraźnie działa w małych populacjach. Dobór i dryf mogą oczywiście występować równocześnie. Nie mamy prostego prawa mówiącego, że wszystko, co przetrwało, musiało być optymalne.

Podobnie w eksperymentach obliczeniowych nie powinniśmy automatycznie uznawać jednego udanego uruchomienia za dowód wyższości metody. Inny start lub inne losowanie może poprowadzić algorytm zupełnie inną drogą. W organizacji analogicznie: jedna firma odniosła sukces, stosując określoną strategię. Nie oznacza to jeszcze, że sukces został spowodowany wyłącznie przez tę strategię. Potrzebujemy porównania, a nie tylko atrakcyjnej historii zwycięzcy.

## Slajd 08. Krajobraz przystosowania
*I · Biologia*

Spójrzmy na krajobraz. To metafora przestrzeni możliwości, a nie mapa, którą rzeczywiście ogląda organizm. Wysokość może przedstawiać umowną wartość przystosowania. Niektóre obszary mają wiele lokalnych wzniesień, a pomiędzy nimi występują doliny. Można osiągnąć szczyt najbliższego wzgórza i nadal znajdować się daleko od najwyższego punktu całego krajobrazu.

Jeżeli mechanizm dopuszcza wyłącznie zmiany poprawiające bieżący wynik, może nie znaleźć drogi do lepszego obszaru. Czasem potrzebna jest zmiana, która chwilowo pogarsza sytuację. W rzeczywistej biologii obraz jest jeszcze bardziej skomplikowany, bo warunki się zmieniają, a sukces jednego organizmu zależy od innych organizmów. Sam krajobraz może się przekształcać.

W biznesie wyobraźmy sobie firmę, która każdego kwartału doskonali aktualny produkt. Zmniejsza koszty, usprawnia sprzedaż, poprawia marżę. Jest na coraz wyższym lokalnym szczycie. Jednocześnie gdzieś obok może powstawać rynek, do którego nie da się przejść samym doskonaleniem tego produktu. Potrzebna jest eksploracja. Właśnie dlatego optymalizacja i innowacja nie są tym samym.

## Slajd 09. Koszt specjalizacji
*I · Biologia*

Specjalizacja jest jedną z dróg do bardzo wysokiej efektywności. Jeżeli wiemy, jakie warunki będą panowały jutro, możemy ograniczyć zbędne zasoby i dostosować się dokładnie do nich. Problem pojawia się wtedy, gdy nasze założenie o jutrze jest błędne.

Wyobraźmy sobie firmę, która całą sprzedaż prowadzi przez jedną platformę. Zna jej algorytm, potrafi skutecznie reklamować produkty, ma doskonale zoptymalizowane procedury. To realna przewaga. Ale zmiana regulaminu, opłat lub sposobu pozycjonowania może jednocześnie uderzyć w cały biznes. Utrzymywanie drugiego kanału wyglądało wcześniej jak niepotrzebny koszt. Po zmianie może okazać się zasobem umożliwiającym przetrwanie.

Z biologicznej analogii nie wynika, że każda różnorodność jest dobra i należy utrzymywać wszystkie warianty. Wynika raczej pytanie o wartość opcji. Ile kosztuje nas pozostawienie możliwości zmiany kierunku? W projektach AI taką opcją może być alternatywny dostawca, możliwość wyłączenia automatyzacji albo zachowanie kompetencji pracowników. Efektywność mierzymy dzisiaj, odporność ujawnia się w innych warunkach.

## Slajd 10. Ewolucja nie ma planu. My już mamy.
*I · Biologia*

Dotarliśmy do fundamentalnej granicy naszej analogii. Ewolucja biologiczna nie jest realizacją projektu z zapisaną funkcją celu. W naturze nie ma centralnego programu, który przyznaje wszystkim organizmom punkty według jednej skali. Natomiast gdy przenosimy inspirację ewolucyjną do komputera, sami definiujemy przestrzeń rozwiązań, sposób ich oceny i warunek zakończenia procesu.

To ogromna różnica. Jeśli algorytm ma zaprojektować harmonogram pracy, ktoś decyduje, czy nagradzamy liczbę wykonanych zleceń, zysk, terminowość, czy może ograniczenie przeciążenia pracowników. Te wartości nie pojawią się w algorytmie z samego faktu, że jest inspirowany naturą.

Zatem w momencie, w którym zaczynamy projektować cyfrową ewolucję, stajemy się projektantami środowiska selekcji. Możemy tworzyć środowisko, w którym wygrywa skuteczność, uczciwość, odporność lub wyłącznie szybkość. Możemy również stworzyć środowisko nagradzające coś innego, niż deklarujemy. Proszę zachować tę myśl do końca wykładu. Powróci przy treningu modeli, agentach i wskaźnikach biznesowych.

## Slajd 11. Maszyna, która przeszukuje możliwości
*II · Ewolucja cyfrowa*

W klasycznym programowaniu często dokładnie określamy sekwencję kroków, która prowadzi do wyniku. Jeśli chcemy policzyć podatek według znanej stawki, zapisujemy odpowiednią regułę. Ale istnieją problemy, w których nie znamy dobrej sekwencji prowadzącej do rozwiązania. Możliwości jest ogromnie dużo, a każda z nich ma inne konsekwencje.

Algorytmy ewolucyjne proponują inną strategię. Nie zapisujemy od razu najlepszego harmonogramu produkcji ani najlepszej trasy. Definiujemy, jak reprezentować kandydatów, jak ich oceniać i jak tworzyć nowe warianty. Wiele rozwiązań może zostać sprawdzonych bez konieczności ręcznego wymyślania każdego z nich.

Zwróćmy uwagę, że nie jest to gwarancja znalezienia globalnego optimum. Jest to metoda poszukiwania, której wartość oceniamy na tle innych dostępnych metod. Ale z perspektywy biznesu następuje istotna zmiana roli projektanta. Człowiek nie musi już sam zaprojektować wszystkich szczegółów rozwiązania. Musi natomiast wiedzieć, czym jest rozwiązanie dopuszczalne i według jakich kryteriów uznamy je za lepsze.

## Slajd 12. Od DNA do reprezentacji rozwiązania
*II · Ewolucja cyfrowa*

Posłużmy się prostym przykładem. Mamy sześć punktów dostawy. Kandydat może być zapisany jako lista: punkt trzeci, pierwszy, szósty, drugi, piąty i czwarty. Taki zapis pełni w algorytmie rolę genotypu. Nie jest DNA. Jest reprezentacją rozwiązania, na której możemy wykonywać operacje.

Fenotypem w naszej analogii jest wynikający z tej listy rzeczywisty plan przejazdu, z kolejnością wizyt i długością odcinków. Następnie oceniamy, jak ten plan działa. Najprostsza funkcja fitness może mierzyć całkowitą długość trasy. W realnej firmie prawdopodobnie potrzebujemy czegoś więcej: godzin otwarcia odbiorców, kosztów paliwa, czasu pracy kierowcy, pojemności samochodu oraz obowiązujących ograniczeń.

Wybór reprezentacji to bardzo poważna decyzja. Jeśli zapisujemy wyłącznie kolejność klientów, nie możemy bezpośrednio poszukiwać rozwiązań dotyczących liczby samochodów, chyba że rozszerzymy zapis. Algorytm może znaleźć jedynie rozwiązania, które da się wyrazić w jego przestrzeni. W tym sensie granice reprezentacji stają się granicami tego, co system jest w stanie rozważyć.

## Slajd 13. Pętla ewolucyjna
*II · Ewolucja cyfrowa*

Przyjrzyjmy się pętli. Najpierw tworzymy populację kandydatów. Mogą być losowi lub częściowo pochodzić z rozwiązań opracowanych wcześniej. Następnie obliczamy ocenę każdego z nich. Niektóre wybieramy jako podstawę następnego pokolenia, a z ich udziałem tworzymy nowe warianty. Później znowu oceniamy populację.

Jeżeli zastosujemy elitaryzm, możemy zachować najlepsze dotychczasowe rozwiązania. Jeżeli wprowadzimy zmiany losowe, dajemy szansę na odkrycie czegoś, czego wcześniej nie sprawdziliśmy. Powtarzamy tę procedurę do osiągnięcia limitu pokoleń, czasu, kosztu lub innego warunku zatrzymania.

Warto zauważyć, że nie ma tu jednej magicznej operacji powodującej inteligentny wynik. Efekt wynika z wielokrotnego sprzężenia zwrotnego między generowaniem a oceną. Podobny wzorzec widzimy w zarządzaniu: mały eksperyment, pomiar, wybór i kolejna wersja. Ale organizacja nie jest algorytmem genetycznym tylko dlatego, że eksperymentuje. To analogia pomagająca nam rozumieć cykl poszukiwania, a nie utożsamienie mechanizmów.

## Slajd 14. Krzyżowanie i mutacja
*II · Ewolucja cyfrowa*

Krzyżowanie, mutacja i elitaryzm odpowiadają za różne aspekty procesu. Krzyżowanie próbuje połączyć fragmenty rozwiązań rodzicielskich. Mutacja wprowadza zmianę, na przykład zamienia dwa punkty trasy miejscami. Elitaryzm zachowuje część dobrych kandydatów, aby nie utracić dotychczasowych osiągnięć.

Ale uwaga: operacja musi pasować do reprezentacji. Jeśli połączymy pierwszą połowę jednej trasy z drugą połową innej trasy, może się okazać, że odwiedzimy klienta dwa razy, a innego pominiemy. Potrzebujemy operatora, który zachowa poprawną permutację, albo procedury naprawczej. W przeciwnym razie będziemy optymalizowali coś, co nie jest nawet dopuszczalnym rozwiązaniem.

Pomyślmy o projektowaniu grafiku pracowników. Mutacja polegająca na przeniesieniu jednej osoby na inną zmianę może naruszyć wymagane kwalifikacje albo odpoczynek. Niektóre warunki powinny być traktowane jako twarde ograniczenia, a nie jako drobne ujemne punkty, które można skompensować zyskiem. Dobre projektowanie algorytmu zaczyna się więc od zrozumienia rzeczywistego procesu, nie od wyboru operatora genetycznego.

## Slajd 15. Genetyczne, ewolucyjne, roju
*II · Ewolucja cyfrowa*

W literaturze spotkają Państwo wiele nazw: algorytmy genetyczne, strategie ewolucyjne, programowanie genetyczne, optymalizacja rojem cząstek czy algorytmy mrówkowe. Wszystkie można umieścić w szerszej przestrzeni metod poszukiwania i optymalizacji, ale nie są jednym algorytmem.

W algorytmach ewolucyjnych szczególne znaczenie ma populacja, tworzenie wariantów i selekcja. Programowanie genetyczne może operować na strukturach programów. W optymalizacji rojem cząstek kandydaci przemieszczają się w przestrzeni, korzystając z informacji o własnych i zbiorowych doświadczeniach. Algorytmy mrówkowe wykorzystują mechanizmy inspirowane wzmacnianiem ścieżek poprzez pośrednie przekazywanie informacji.

Nie chcę, żeby zapamiętali Państwo te nazwy jako zestaw modnych technologii. Chcę, żebyście rozpoznawali różne filozofie poszukiwania. Czy wykorzystujemy selekcję wariantów? Czy budujemy rozwiązanie krok po kroku? Czy jednostki dzielą się informacją? Wybór metody zależy od struktury problemu, kosztu oceny kandydatów oraz wymaganej jakości rozwiązania. Czasami klasyczny solver lub prosta reguła wystarczą. Inspiracja naturą nie stanowi sama w sobie uzasadnienia biznesowego.

## Slajd 16. Firma jako problem wielokryterialny
*II · Ewolucja cyfrowa*

W przedsiębiorstwie niemal nigdy nie mamy tylko jednego celu. Możemy chcieć minimalizować koszt, maksymalizować terminowość, ograniczać ryzyko, zapewniać jakość oraz zachować rezerwę na nieprzewidziane zdarzenia. Te cele mogą być ze sobą w konflikcie.

Wyobraźmy sobie zakład produkcyjny. Jeśli wypełnimy harmonogram wszystkich maszyn do ostatniej minuty, teoretyczne wykorzystanie zasobów będzie znakomite. Ale jedna awaria może spowodować przesunięcie całego planu. Harmonogram z rezerwą będzie wyglądał gorzej w mierniku zajętości, a lepiej w odporności na zakłócenia. Nie jest to błąd matematyczny. To różnica wartości, które próbujemy osiągnąć.

Można zbudować funkcję oceny, która łączy kilka kryteriów przy użyciu wag. Wtedy jednak wagi stanowią ukrytą decyzję biznesową: ile jesteśmy gotowi zapłacić za mniejsze ryzyko? Alternatywnie można wyznaczać zbiór kompromisów i przedstawić go osobie odpowiedzialnej. Właśnie tutaj algorytm powinien wspierać zarząd, a nie pozorować, że istnieje jedna obiektywna odpowiedź na każde pytanie.

## Slajd 17. Front Pareto: wybór, którego algorytm nie zrobi za zarząd
*II · Ewolucja cyfrowa*

Na wykresie widzimy poglądowy front Pareto. Każdy punkt oznacza inne rozwiązanie, opisane tutaj przez koszt i ryzyko. Załóżmy, że obydwie wartości chcemy minimalizować. Jeśli rozwiązanie A jest tańsze od rozwiązania B i jednocześnie nie jest bardziej ryzykowne, a przynajmniej w jednym kryterium jest ściśle lepsze, możemy uznać B za zdominowane.

Po odrzuceniu takich punktów zostają rozwiązania, wśród których poprawa jednego kryterium wymaga pogorszenia drugiego. To właśnie front kompromisów. Algorytm może pomóc go znaleźć, ale sam fakt, że punkt znajduje się na froncie, nie rozstrzyga, który punkt jest dla nas właściwy.

Wyobraźmy sobie trzy warianty dostaw: najtańszy z niewielką rezerwą, umiarkowany i droższy z wysoką odpornością. Który wybieramy? To zależy od tego, jakie konsekwencje niesie niedotrzymanie terminu. W przypadku dostawy zwykłych materiałów biurowych wybór może być inny niż w przypadku krytycznego komponentu produkcyjnego. Algorytm ujawnia strukturę decyzji. Odpowiedzialność za zaakceptowanie kompromisu pozostaje po stronie organizacji.

## Slajd 18. Eksperyment: trasa, która ewoluuje
*II · Ewolucja cyfrowa*

Teraz zobaczmy prawdziwy eksperyment obliczeniowy, a nie ilustrację koncepcyjną. Mamy dwadzieścia syntetycznych punktów. Zadanie polega na znalezieniu możliwie krótkiej zamkniętej trasy odwiedzającej wszystkie punkty. Odległość mierzymy w geometrii euklidesowej. Nie uwzględniamy ruchu ulicznego, okien czasowych ani ładowności pojazdu.

Najlepsza trasa w populacji początkowej miała długość około 866,3 jednostki. Po stu pokoleniach uzyskaliśmy około 371,7. Dla porównania prosta heurystyka najbliższego sąsiada dała około 404,5 jednostki. W tym konkretnym uruchomieniu ewolucja znalazła rozwiązanie lepsze od obu punktów odniesienia. Proszę jednak uważać na wniosek: nie udowodniliśmy, że algorytm ewolucyjny jest zawsze najlepszy. Nie wykazaliśmy również globalnej optymalności trasy.

Za chwilę możemy otworzyć notebook i zobaczyć, jak wynik powstaje. Zachęcam Państwa do zmiany ziarna losowego, liczby pokoleń i wielkości populacji. To bardzo ważny element myślenia o AI: zamiast podziwiać pojedynczy wynik, badajmy zachowanie metody w różnych warunkach. Dopiero wtedy zaczynamy odróżniać efekt demonstracyjny od dowodu przydatności.

## Slajd 19. Python: proces w kilkunastu liniach
*II · Ewolucja cyfrowa*

Proszę teraz spojrzeć na kod. To pseudokod, czyli uproszczony zapis idei, a nie samodzielny program gotowy do uruchomienia. Najpierw generujemy populację tras. Potem wielokrotnie wybieramy najlepsze rozwiązania, tworzymy ich zmodyfikowane warianty i budujemy następną populację. Na końcu zwracamy najlepszego kandydata.

W dołączonym notebooku te operacje są rozwinięte do rzeczywistego kodu. Funkcja odległości oblicza wartość trasy, selekcja sortuje kandydatów, a mutacja zmienia ich kolejność. Ten konkretny przykład nie wymaga krzyżowania. Wystarczy odpowiednio zorganizowane tworzenie wariantów i zachowanie elit.

Najciekawsze jest to, czego w kodzie nie ma. Nie ma pojęcia klienta jako człowieka. Nie ma rozumienia obietnicy dostawy ani konsekwencji spóźnienia. System operuje na liczbach i reprezentacji. Jeśli chcemy, aby uwzględniał określony aspekt rzeczywistości, musimy go wprowadzić do danych, ograniczeń lub oceny. To ważna lekcja także dla modeli językowych: skuteczność w reprezentacji problemu nie jest automatycznie pełnym rozumieniem świata, którego problem dotyczy.

## Slajd 20. To, co nagradzasz, zaczyna dominować.
*II · Ewolucja cyfrowa*

Załóżmy, że zleciliśmy algorytmowi maksymalizację wykorzystania maszyn. Algorytm znalazł harmonogram, w którym wykorzystanie wynosi niemal sto procent. Gratulujemy sobie sukcesu. Następnego dnia jedna maszyna ulega awarii i nie mamy żadnej rezerwy. Cały proces zaczyna się rozpadać.

Czy algorytm zawiódł? Być może wykonał dokładnie zadanie, które mu powierzono. To my nie uwzględniliśmy istotnego aspektu rzeczywistości. Właśnie tutaj pojawia się problem optymalizacji zastępczego wskaźnika. System nie musi mieć złych intencji ani świadomie nas oszukiwać. Wystarczy, że konsekwentnie wykorzysta możliwość uzyskania wysokiej oceny.

Im bardziej skuteczny mechanizm poszukiwania, tym ważniejsze jest sprawdzanie, czy funkcja celu naprawdę odpowiada naszym wartościom. Dlatego testujemy nie tylko wynik na metryce, ale również skutki uboczne i przypadki skrajne. Pytanie do Państwa: gdyby w Waszej firmie pewien system został nagrodzony wyłącznie za obecny główny KPI, w jaki sposób mógłby osiągnąć znakomity wynik, nie poprawiając rzeczywistej sytuacji? Zachowajmy to pytanie, bo wróci w drugiej połowie wykładu.

## Slajd 21. Inteligencja ograniczonych zasobów
*III · Heurystyki*

Przejdźmy od ewolucji populacji do decyzji pojedynczego podmiotu. Jeżeli świat jest ogromny, a czas i zasoby ograniczone, pełne rozważenie wszystkich możliwości jest często niewykonalne. Wyobraźmy sobie, że przed każdym wyjściem z domu analizujemy wszystkie możliwe drogi, ich historyczne obciążenie, pogodę oraz wszystkie konsekwencje spóźnienia. Zanim skończymy analizę, prawdopodobnie stracimy więcej czasu, niż moglibyśmy zaoszczędzić.

Heurystyka jest sposobem radzenia sobie z takim ograniczeniem. Umożliwia ukierunkowanie poszukiwania lub podjęcie decyzji bez pełnego rozwiązania problemu. Nie gwarantuje zawsze najlepszego wyniku. Nie oznacza też automatycznie błędnego myślenia. Jej jakość zależy od środowiska, w którym ją stosujemy.

To będzie ważna część wykładu, ponieważ często stawiamy maszynie nierealistyczne oczekiwania. Chcemy, aby była jednocześnie szybka, dokładna, tania i odporna na wszystkie nieznane przypadki. Tymczasem inteligentne projektowanie polega również na ustalaniu, kiedy warto szukać dalej, a kiedy koszt kolejnej informacji jest większy niż jej wartość.

## Slajd 22. Codzienność pełna skrótów
*III · Heurystyki*

Każdy z nas używa heurystyk. W sklepie wybieramy markę, która wcześniej się sprawdziła. W nieznanym mieście szukamy drogi prowadzącej w ogólnym kierunku celu. Podczas rozmowy rekrutacyjnej próbujemy z ograniczonej liczby sygnałów wywnioskować, czy kandydat będzie dobrze wykonywał pracę. Nie badamy wszystkiego od początku, ponieważ byłoby to zbyt kosztowne.

Takie skróty bywają bardzo skuteczne. Doświadczony pracownik może zauważyć symptomy problemu, których osoba początkująca nie rozpoznaje. Ale heurystyka może też przenieść dawne doświadczenie do sytuacji, w której przestało ono obowiązywać. Znana marka nie zawsze jest najlepszym produktem. Swoboda wypowiedzi nie zawsze świadczy o kompetencji zawodowej.

W rekrutacji szczególnie niebezpieczne jest utożsamianie podobieństwa do wcześniejszych pracowników z rzeczywistą zdolnością wykonania pracy. W systemie AI ten sam skrót może zostać zakodowany w danych historycznych lub regułach oceny. Dlatego dobra praktyka polega na sprawdzaniu heurystyk względem rzeczywistego wyniku. Pytajmy, kiedy działają, kiedy przestają działać i komu przypisują koszt własnych błędów.

## Slajd 23. Szybkie myślenie i ograniczona racjonalność
*III · Heurystyki*

Herbert Simon wprowadził ideę ograniczonej racjonalności, która pozwala inaczej spojrzeć na decyzje ekonomiczne. Człowiek nie dysponuje pełną informacją, nieskończonym czasem i nieograniczoną zdolnością obliczeniową. W realnej organizacji często nie maksymalizujemy wszystkich możliwych korzyści. Poszukujemy rozwiązania spełniającego wymagania, które uznajemy za wystarczające.

Wyobraźmy sobie dział ofertowania. Możemy przez trzy tygodnie szukać absolutnie najlepszej konfiguracji produktu, a klient może w tym czasie podpisać umowę z konkurencją. Oferta przygotowana w godzinę, spełniająca wymagania i zapewniająca akceptowalną marżę, może mieć znacznie większą wartość. Ten mechanizm określa się pojęciem satisficing, czyli poszukiwania rozwiązania satysfakcjonującego względem określonego progu.

Proszę zauważyć, że próg jest znowu decyzją projektową. Nie chcemy zadowalać się dowolną odpowiedzią. Musimy ustalić minimalną jakość, maksymalny koszt i warunki, których nie wolno naruszyć. W zastosowaniach AI to praktyczna alternatywa dla bezrefleksyjnego pytania o najlepszy model. Najlepszy do czego, w jakim czasie, przy jakim budżecie i przy jakim poziomie ryzyka?

## Slajd 24. Dostępność, zakotwiczenie, reprezentatywność
*III · Heurystyki*

Psychologia poznawcza pokazuje kilka sposobów, w jakie szybkie osądy mogą się systematycznie odchylać od bardziej kompletnej oceny. Dostępność oznacza, że łatwo przywoływane przykłady mogą wydawać się częstsze, niż są naprawdę. Głośna historia awarii może zdominować ocenę ryzyka, mimo że nie znamy rzeczywistej częstości takich zdarzeń.

Zakotwiczenie polega na tym, że początkowa wartość wpływa na dalsze osądy. Jeśli najpierw pokażę Państwu ofertę za sto tysięcy, a później ofertę za sześćdziesiąt tysięcy, druga może wydawać się korzystna, nawet jeśli jej niezależna wartość wynosi znacznie mniej. Reprezentatywność natomiast wykorzystuje podobieństwo do pewnego wzorca, czasami pomijając częstości bazowe. Kandydat wyglądający na typowego świetnego sprzedawcę nie musi nim być.

Nie sprowadzajmy całej ludzkiej intuicji do błędów. Jej efektywność może wynikać z doświadczenia w danym środowisku. Ale w biznesie powinniśmy rozróżnić sygnał od dowodu. To samo dotyczy odpowiedzi AI: płynność, znajomy styl i pewność wypowiedzi są sygnałami, które mogą wpłynąć na naszą ocenę, chociaż nie gwarantują prawdziwości treści.

## Slajd 25. Od intuicji do algorytmu zachłannego
*III · Heurystyki*

Przełóżmy intuicję na prosty algorytm. Jeśli jesteśmy w punkcie A i mamy odwiedzić wiele kolejnych punktów, możemy zawsze wybierać najbliższy jeszcze nieodwiedzony punkt. To przykład strategii zachłannej. Każdy krok ma prostą zasadę, a decyzja jest lokalnie uzasadniona.

Problem w tym, że sekwencja dobrych lokalnych wyborów nie musi tworzyć najlepszego globalnego rozwiązania. Możemy odwiedzić wiele punktów położonych blisko siebie, a na końcu pozostawić jeden bardzo odległy. Wtedy koszt ostatniego przejazdu może zniwelować wcześniejsze oszczędności. W naszym notebooku najbliższy sąsiad stanowi punkt odniesienia dla algorytmu ewolucyjnego. Jest szybki, prosty i warto go traktować poważnie, nawet jeśli nie zapewnia optimum.

W organizacji strategia zachłanna może oznaczać wybieranie w każdym miesiącu zlecenia z najwyższą natychmiastową marżą, bez uwzględnienia relacji z kluczowymi klientami lub przyszłych zobowiązań. Nie jest to dowód, że każda lokalna optymalizacja jest zła. Jest to przypomnienie, że sposób wyboru kolejnego kroku i sposób oceny całego procesu to odrębne rzeczy.

## Slajd 26. A*: kierunek zamiast błądzenia
*III · Heurystyki*

Algorytm A z gwiazdką pokazuje, jak do przeszukiwania można wprowadzić wiedzę o kierunku. Nie patrzymy wyłącznie na koszt dotychczasowego przejścia ani wyłącznie na pozorną bliskość celu. Łączymy obydwie informacje. Litera g oznacza koszt już poniesiony, h jest oszacowaniem kosztu pozostałego, a ich suma wyznacza priorytet dalszego poszukiwania.

W nawigacji dobrym przykładem heurystyki może być odległość w linii prostej, jeśli optymalizujemy długość drogi. Jest ona dolnym oszacowaniem dystansu potrzebnego do dotarcia do celu. Droga, która prowadzi geometrycznie w jego stronę, nie musi jednak być dostępna. Algorytm potrzebuje reprezentacji rzeczywistych połączeń. Przy odpowiednich warunkach, między innymi dopuszczalnej heurystyce i prawidłowym prowadzeniu wyszukiwania, A z gwiazdką może znaleźć optymalne rozwiązanie.

To pokazuje, że heurystyka nie zawsze oznacza rezygnację z gwarancji. Może być elementem metody, która w określonych warunkach zachowuje gwarancję poprawności. Biznesowa lekcja jest prosta: dobry szacunek potrafi radykalnie ograniczyć zakres poszukiwania, ale warto wiedzieć, na czym opiera się ten szacunek i w jakich sytuacjach przestaje być wiarygodny.

## Slajd 27. Wyżarzanie: czasem pogorszyć, by poprawić
*III · Heurystyki*

Wyżarzanie symulowane wykorzystuje ideę, która może wydawać się sprzeczna z intuicją zarządzania: czasami warto zaakceptować pogorszenie bieżącego wyniku, aby mieć szansę na znalezienie lepszego rozwiązania. Gdy poruszamy się po krajobrazie przystosowania wyłącznie pod górę, możemy zatrzymać się na pierwszym lokalnym szczycie.

W wyżarzaniu symulowanym parametr nazywany temperaturą steruje gotowością do przyjęcia gorszego ruchu. Przy wyższej temperaturze takie ruchy są bardziej prawdopodobne, co sprzyja eksploracji. W miarę obniżania temperatury proces zwykle coraz bardziej koncentruje się na dobrych obszarach. Jeśli schłodzimy go zbyt szybko, może utknąć w niezbyt dobrym miejscu. Jeśli zbyt wolno, obliczenia mogą być niepotrzebnie kosztowne.

Niech analogią biznesową będzie inwestycja w nowy proces produkcyjny. Na początku może obniżyć wydajność z powodu szkoleń i kosztów przejścia. Nie oznacza to jeszcze, że projekt jest zły. Ale nie wynika z tego również, że każde pogorszenie warto akceptować. Potrzebujemy kontrolowanej eksploracji: budżetu, kryterium oceny i warunku zakończenia eksperymentu.

## Slajd 28. Decyzja o metodzie jest decyzją ekonomiczną.
*III · Heurystyki*

Wyobraźmy sobie dyspozytora, który musi w ciągu trzydziestu sekund ułożyć trasę dla kurierów. Ma do dyspozycji prostą heurystykę, algorytm ewolucyjny i metodę dokładną. Którą powinien wybrać? Nie da się odpowiedzieć, zanim nie zdefiniujemy wymagań.

Jeśli metoda dokładna potrzebuje kilku godzin, może być bezużyteczna w tej konkretnej sytuacji. Jeśli prosta heurystyka daje wynik o kilka procent gorszy, ale umożliwia natychmiastową reakcję, może mieć większą wartość biznesową. Jeśli z kolei opracowujemy plan na następny miesiąc i różnica kosztów będzie znacząca, dodatkowy czas obliczeń może być uzasadniony. Możemy nawet połączyć metody: zacząć od heurystyki i poprawiać jej wynik tak długo, jak pozwala budżet.

Proszę teraz zastanowić się, ile w Państwa organizacji kosztuje dodatkowy jeden procent poprawy. Czy liczymy tylko koszt pracy programu, czy również koszt oczekiwania, infrastruktury i ryzyka? To pytanie prowadzi nas do kolejnego aktu. W świecie modeli AI również nie wystarczy wiedzieć, który model uzyskuje najlepszy wynik. Musimy zrozumieć środowisko, w którym powstaje i w którym będzie używany.

## Slajd 29. Python jest wejściem do ekosystemu
*IV · Hodowanie AI*

Kiedy mówię, że Python jest jednym z najważniejszych języków współczesnego AI, nie mam na myśli jedynie pętli, funkcji i instrukcji warunkowych. Sam język jest narzędziem umożliwiającym wejście do znacznie większego ekosystemu. To ekosystem, w którym dane są przygotowywane, modele trenowane, porównywane, przechowywane, udostępniane, monitorowane i zastępowane kolejnymi wersjami.

Proszę wyobrazić sobie laboratorium, w którym badacze stale przeprowadzają eksperymenty. Nie wystarczy mieć probówki. Potrzebują aparatury, metod pomiaru, dokumentacji, kontroli warunków oraz procedur pozwalających odtworzyć eksperyment. Python pełni w naszym przypadku rolę języka, którym możemy organizować znaczną część pracy tego laboratorium.

Nie chcę teraz prowadzić Państwa przez kurs programowania. Chcę, żeby po tej części potrafili Państwo rozpoznać, co znajduje się za prostą demonstracją w notebooku, kto wykonuje poszczególne elementy pracy i dlaczego czasami napisanie kodu jest najmniejszą częścią projektu. Gdy mówimy o wdrożeniu sztucznej inteligencji w firmie, naprawdę mówimy o zbudowaniu procesu, nie tylko o uruchomieniu programu.

## Slajd 30. Co naprawdę uruchamiamy, pisząc Python?
*IV · Hodowanie AI*

Co dzieje się, gdy w notebooku zapisujemy kilka linii Pythona i naciskamy przycisk uruchomienia? Najpierw mamy środowisko wykonawcze, które interpretuje nasz kod. Jeżeli wywołujemy funkcję biblioteki numerycznej, ciężka praca nie musi odbywać się bezpośrednio w samym Pythonie. Biblioteka może przekazać obliczenia do skompilowanego kodu lub wyspecjalizowanego akceleratora.

Notebook jest interfejsem pracy. Interpreter wykonuje instrukcje. Biblioteka zapewnia gotowe operacje, a procesor lub GPU wykonuje obliczenia. To różne warstwy. Dzięki temu badacz może w kilku liniach kodu zainicjować operację, która obejmuje ogromną liczbę działań matematycznych. Nie oznacza to, że sama prostota kodu powoduje niski koszt obliczeń.

Z biznesowego punktu widzenia jest tu ważna konsekwencja. Wygoda tworzenia prototypu nie jest równoznaczna z prostotą utrzymywania rozwiązania. Kod może mieć pięćdziesiąt linii, ale za nim mogą stać rozbudowane biblioteki, zewnętrzne usługi, konkretne wersje sterowników i wymagania sprzętowe. Przy odbiorze projektu warto zatem pytać nie tylko o kod, lecz także o to, czego ten kod potrzebuje, aby rzeczywiście działać.

## Slajd 31. Środowisko jest częścią wyniku
*IV · Hodowanie AI*

Załóżmy, że pracownik przekazuje Państwu notebook, który na jego komputerze osiąga bardzo dobry wynik. Próbujemy uruchomić go na innym komputerze i pojawia się błąd. Albo wynik jest nieco inny. Czy oznacza to, że kod jest zły? Niekoniecznie. Mogły zmienić się wersje bibliotek, dane, parametry wykonania lub sposób losowania.

Dlatego środowisko jest częścią eksperymentu. Musimy znać wersję Pythona i pakietów, pochodzenie danych, parametry modelu oraz konfigurację uruchomienia. Ziarno losowe pozwala kontrolować niektóre źródła losowości, ale nie zawsze gwarantuje identyczny wynik na różnych urządzeniach. Niektóre operacje mogą zależeć od sprzętu i sposobu równoległego wykonywania obliczeń.

W przedsiębiorstwie ma to ogromne znaczenie. Jeżeli system podjął rekomendację trzy miesiące temu, a klient kwestionuje jej uzasadnienie, powinniśmy potrafić ustalić, jaka wersja systemu wtedy działała i na jakich danych. Dokumentacja eksperymentu nie jest zatem biurokratycznym dodatkiem do AI. Jest elementem odpowiedzialności. Notebook bez danych, zależności i historii konfiguracji może być demonstracją, ale niekoniecznie powtarzalnym procesem biznesowym.

## Slajd 32. Mapa ekosystemu
*IV · Hodowanie AI*

Spójrzmy na mapę ekosystemu. NumPy umożliwia wydajne operacje na tablicach numerycznych. Pandas ułatwia pracę z danymi tabelarycznymi. Scikit-learn zawiera wiele klasycznych metod uczenia maszynowego i narzędzi służących do przygotowania danych oraz oceny modeli. PyTorch i TensorFlow pozwalają budować i trenować modele głębokie.

To jednak tylko część środowiska. Jupyter i Colab służą do pracy eksperymentalnej. Ekosystem Hugging Face umożliwia między innymi dostęp do modeli, tokenizatorów i zbiorów danych. Narzędzia takie jak MLflow wspierają rejestrowanie przebiegu eksperymentów. W zależności od projektu potrzebne mogą być także bazy danych, systemy kolejkowania, repozytoria kodu, rejestry modeli i infrastruktura wdrożeniowa.

Proszę nie traktować tej mapy jako listy technologii, które każda firma musi kupić lub zainstalować. Ważniejsze jest rozpoznanie funkcji. Kto odpowiada za dane? Co wykonuje trening? Gdzie zapisujemy wynik? Co pozwala porównać dwie wersje? Jak uruchamiamy model dla użytkownika? Jeżeli dostawca potrafi wymienić dwadzieścia bibliotek, lecz nie potrafi odpowiedzieć na te pytania, sama znajomość narzędzi nie daje nam jeszcze pewności jakości systemu.

## Slajd 33. Od danych do systemu produkcyjnego
*IV · Hodowanie AI*

Zbudowanie modelu to początek dłuższej drogi. W typowym projekcie najpierw pozyskujemy i przygotowujemy dane, następnie przeprowadzamy trening, a potem sprawdzamy wyniki na danych lub zadaniach, które nie służyły bezpośrednio do dopasowywania modelu. Jeżeli model spełnia wymagania, możemy zarejestrować jego wersję i wdrożyć go do określonego procesu.

Po wdrożeniu zaczyna się kolejny etap. Musimy obserwować, czy nie zmieniają się dane wejściowe, czy system nadal osiąga oczekiwaną jakość i czy nie rośnie liczba wyjątków. Zmiana rynku, zachowania klientów albo sposobu rejestrowania danych może sprawić, że model, który wcześniej dobrze działał, przestanie być odpowiedni. Zarządzanie tym cyklem nazywamy szeroko MLOps, czyli połączeniem praktyk uczenia maszynowego i utrzymywania systemów.

Warto zastanowić się, kto w organizacji ma prawo powiedzieć, że model powinien zostać wymieniony lub wyłączony. Jeśli nikt nie jest właścicielem jego jakości po wdrożeniu, to prawdopodobnie nie mamy jeszcze dojrzałego produktu. Mamy eksperyment podłączony do rzeczywistego procesu. Odpowiedzialne skalowanie wymaga zaprojektowania całego cyklu życia.

## Slajd 34. Trening nie jest inferencją
*IV · Hodowanie AI*

Musimy bardzo wyraźnie rozdzielić dwa pojęcia: trening i inferencję. Podczas treningu system dopasowuje parametry na podstawie danych oraz wybranego sygnału uczenia. Podczas inferencji wykorzystuje już wyuczone parametry, aby przetworzyć nowe dane lub wygenerować odpowiedź. To nie jest ta sama operacja.

Wyobraźmy sobie model językowy, który otrzymuje dokument z procedurą firmową. Może odpowiedzieć na pytanie dotyczące procedury, ponieważ treść została umieszczona w kontekście. Nie musimy z tego powodu aktualizować jego wag. Jeśli aplikacja zapamięta dokument i będzie go później przywoływać, to również nie musi oznaczać zmiany parametrów modelu. Pamięć aplikacji, kontekst oraz trening należą do różnych warstw systemu.

W biznesie nieporozumienie dotyczące tego rozróżnienia może prowadzić do nietrafionych inwestycji. Ktoś mówi, że chce nauczyć model aktualnego cennika. Być może wystarczy zapewnić mu kontrolowany dostęp do bazy aktualnych cen. Z kolei jeśli chcemy zmienić sposób klasyfikowania określonych przypadków, może być potrzebna inna metoda adaptacji. Najpierw nazywamy oczekiwaną zmianę zachowania, dopiero potem wybieramy mechanizm jej uzyskania.

## Slajd 35. Hodowla: od korpusu do preferencji
*IV · Hodowanie AI*

Używam słowa hodowla jako metafory procesu kształtowania modelu. Nie oznacza to, że model jest organizmem biologicznym. Oznacza, że końcowe zachowanie systemu nie wynika wyłącznie z jednego projektu architektury. Wpływ mają również dane, cele treningowe, późniejsze dostrajanie i kryteria wyboru wersji.

W przypadku wielu modeli językowych pierwszym etapem jest pretraining, czyli uczenie ogólnych regularności na dużych zbiorach danych. Późniejsze etapy mogą obejmować nadzorowane dostrajanie do zadań, uczenie na podstawie preferencji lub metody wykorzystujące sygnały nagrody. Nie wszystkie modele powstają identycznie. Wreszcie przeprowadzamy ewaluację i podejmujemy decyzję, które wersje zostaną wykorzystane. Poszczególne etapy mogą kształtować odmienne właściwości systemu.

To prowadzi do istotnego pytania: kto reprezentuje użytkownika w procesie treningu i ewaluacji? Jeśli jeden zestaw przykładów premiuje zwięzłość, a inny premiuje szczegółowość, model może otrzymywać odmienne sygnały. Jeśli w ocenie nie uwzględnimy umiejętności odmowy w przypadku braku danych, płynna odpowiedź może zostać uznana za bardziej pożądaną niż uczciwe przyznanie niewiedzy. Model jest kształtowany również przez to, jak definiujemy pożądane zachowanie.

## Slajd 36. Dane to środowisko rozwojowe
*IV · Hodowanie AI*

Dane nie są rzeczywistością. Są jej zapisem, zawsze w pewien sposób wybranym. Firma może posiadać piętnaście lat dokumentów, faktur, ofert i korespondencji. Czy to znaczy, że ma piętnaście lat gotowej wiedzy do trenowania systemu? Nie. Niektóre dokumenty mogą być nieaktualne, inne błędne, powielone, niespójne lub objęte ograniczeniami dostępu.

Dobór źródeł decyduje, jakie aspekty świata są w korpusie obecne. Filtracja decyduje, które elementy zostaną usunięte. Ważenie i sposób próbkowania wpływają na to, jak często model spotyka określone wzorce. Jeśli rzadkie, lecz krytyczne przypadki są słabo reprezentowane, model może nie mieć wystarczającego sygnału, aby dobrze sobie z nimi radzić. Jeśli w danych historycznych znajduje się systematyczny błąd, może on wpływać na późniejsze zachowanie systemu.

Z perspektywy organizacji najważniejszy zasób nie musi oznaczać największego zbioru danych. Wartość może wynikać z możliwości ustalenia ich pochodzenia, aktualności, praw do wykorzystania i jakości. Często bardziej opłacalne jest uporządkowanie wiedzy firmowej niż kupowanie kolejnego modelu. System AI nie naprawia automatycznie ontologicznego chaosu w organizacji, czyli niejasności tego, czym są jej pojęcia i jak odnoszą się do rzeczywistości.

## Slajd 37. GPU, klastry i koszt obliczeń
*IV · Hodowanie AI*

Modele AI często przedstawia się jako coś niematerialnego, istniejącego gdzieś w chmurze. Tymczasem za każdym obliczeniem znajduje się bardzo materialna infrastruktura: procesory, akceleratory, pamięć, sieci, zasilanie i chłodzenie. Model może być abstrakcyjną strukturą matematyczną, ale wykonanie tej struktury zużywa rzeczywiste zasoby.

GPU są przydatne między innymi dlatego, że potrafią równolegle wykonywać dużą liczbę operacji. W wielkich systemach nie chodzi jednak wyłącznie o szybkość pojedynczego układu. Dane i parametry trzeba przechowywać, przesyłać i synchronizować. Wąskim gardłem może być pamięć, przepustowość sieci albo komunikacja między urządzeniami. Dlatego nie możemy oceniać całego systemu wyłącznie po liczbie kart graficznych.

Ekonomia treningu i ekonomia inferencji również się różnią. Przy treningu płacimy między innymi za proces budowania parametrów; przy inferencji za ich wykorzystanie na potrzeby konkretnych zadań. Duża liczba zapytań może powodować znaczny koszt operacyjny nawet wtedy, gdy pojedyncze zapytanie jest tanie. Dla zarządu istotne pytanie brzmi więc: czy organizacja potrzebuje własnej infrastruktury, czy raczej kontrolowanego dostępu do obliczeń, i gdzie naprawdę powstaje jej przewaga?

## Slajd 38. RAG, fine-tuning, trening od zera
*IV · Hodowanie AI*

Mamy trzy różne podejścia, które w rozmowach biznesowych często są mylone. RAG, czyli generowanie wspomagane wyszukiwaniem, dostarcza modelowi odpowiednie informacje podczas użycia. Fine-tuning polega na dodatkowym dopasowaniu parametrów istniejącego modelu. Trening od zera oznacza budowę parametrów modelu od podstaw, co przy dużych modelach wymaga zupełnie innej skali zasobów.

Jeżeli firma potrzebuje odpowiedzi na pytania o aktualną procedurę, sensownym punktem wyjścia może być wyszukiwanie odpowiednich fragmentów dokumentów i przekazanie ich modelowi. Nie gwarantuje to prawdziwej odpowiedzi: wyszukiwanie może znaleźć zły fragment, a model może go źle zinterpretować. Jeśli natomiast chcemy zmienić sposób wykonywania powtarzalnego zadania, dostrajanie może być przydatne, ale nie jest niezawodnym zamiennikiem aktualnej bazy dokumentów.

Metody można łączyć. Możemy dostroić model do formatu odpowiedzi i równocześnie korzystać z aktualnego katalogu produktów. Proszę myśleć o tym jako o trzech decyzjach inwestycyjnych, a nie stopniach prestiżu. Własny trening nie jest automatycznie bardziej dojrzały od użycia gotowego modelu. Dojrzałość oznacza właściwy dobór mechanizmu do potrzeb, ryzyka, dostępnych danych i kosztu utrzymania.

## Slajd 39. AI w firmie: co kupujesz, co budujesz?
*IV · Hodowanie AI*

Kiedy firma mówi, że posiada własne AI, zawsze warto zapytać: co dokładnie posiada? Czy posiada kod aplikacji, wagi modelu, dane, infrastrukturę, prawa do wykorzystania technologii, czy może po prostu dostęp do usługi? To zupełnie różne rodzaje kontroli.

API może pozwolić szybko uruchomić rozwiązanie bez utrzymywania dużej infrastruktury. W zamian powstaje zależność od dostawcy, warunków dostępu i zmian usług. Model z dostępnymi wagami może zwiększyć kontrolę nad miejscem wykonania i konfiguracją, ale wymaga odpowiednich kompetencji i zasobów. Otwarte wagi nie oznaczają automatycznie pełnej dostępności danych treningowych ani dowolności licencyjnej.

Czasami największa przewaga firmy leży nie w samym modelu, lecz w warstwie biznesowej: własnej wiedzy, integracji z procesem, sposobie kontroli jakości i danych, których inni nie posiadają. Dlatego porównanie dostawców powinno obejmować całkowity koszt utrzymania, możliwość migracji i konsekwencje przerwania usługi. Zapytajmy również, czy po zmianie modelu nadal będziemy mogli korzystać z własnego procesu. Jeżeli cała jego logika jest zamknięta w niedostępnej usłudze, wówczas zakres naszej kontroli jest mniejszy, niż sugeruje interfejs.

## Slajd 40. Nie hodujemy wyłącznie modelu. Hodujemy kryterium sukcesu.
*IV · Hodowanie AI*

Zatrzymajmy się przy sformułowaniu: nie hodujemy wyłącznie modelu, hodujemy kryterium sukcesu. Oczywiście kryterium nie jest żywym organizmem. Chodzi o to, że pewne preferowane zachowania są wzmacniane na kolejnych etapach budowy systemu. Dane, sygnały treningowe, testy, wybór wersji i wskaźniki wdrożenia wpływają na to, które rozwiązania otrzymują szansę dalszego wykorzystania.

Jeżeli system oceniamy wyłącznie na podstawie szybkości odpowiedzi, szybka wersja może wygrać mimo pogorszenia dokładności. Jeżeli premiujemy przekonujące brzmienie, możemy przeoczyć przypadki nadmiernej pewności. Jeżeli oceniamy jedynie łatwe przykłady, model może okazać się nieprzygotowany na wyjątkowe sytuacje występujące w rzeczywistym procesie.

To dlatego organizacja nie powinna bezrefleksyjnie delegować dostawcy definicji jakości. Może korzystać z jego modeli, lecz powinna mieć własne kryteria akceptacji, własne przykłady oraz sposób weryfikacji. Wróciliśmy do mechanizmu selekcji z początku wykładu. Ale teraz przejdziemy o poziom dalej. Co się dzieje, gdy system nie tylko generuje wynik, który oceniamy, lecz także otrzymuje uprawnienie do wykonania działania?

## Slajd 41. Od odpowiedzi do działania
*V · Agent*

Do tej pory mówiliśmy głównie o systemach, które przetwarzają informacje i generują wyniki. Teraz przechodzimy przez istotną granicę. Model językowy może przygotować treść wiadomości. System agentowy wyposażony w odpowiednie narzędzie i uprawnienie może tę wiadomość wysłać. Różnica pomiędzy napisaniem a wysłaniem jest fundamentalna.

W pierwszym przypadku otrzymujemy propozycję pewnego działania. W drugim możemy zmienić stan świata: ktoś otrzymuje komunikat, w bazie powstaje rekord, zamówienie zostaje zmodyfikowane, proces finansowy zostaje zainicjowany. Nie jest konieczne, aby system posiadał świadomość czy własne intencje. Wystarczy, że architektura umożliwia mu skuteczne wykonywanie operacji.

Sprawczość będę tutaj rozumiał operacyjnie: jako zdolność systemu do dokonywania zmian w otoczeniu. Nie rozstrzygamy w ten sposób filozoficznego problemu wolnej woli. Interesuje nas zakres delegacji i jej konsekwencje. Jeśli człowiek przyznaje systemowi uprawnienia, powinien również określić warunki, w których system może ich użyć. Właśnie na tym poziomie architektura techniczna zaczyna przypominać projektowanie organizacji.

## Slajd 42. Chatbot, workflow, agent
*V · Agent*

Czym różni się chatbot od workflow i agenta? Nie samą jakością generowanego języka. Chatbot może odpowiadać na pytania, a nawet mieć dostęp do niektórych narzędzi. Workflow zwykle wykonuje kroki według wcześniej zaprojektowanego przebiegu. W systemie agentowym model może dynamicznie wybierać kolejne działania na podstawie celu, informacji i wyników wcześniejszych operacji.

Przykład: mamy wiadomość od klienta. Workflow może zawsze wykonać ustalone kroki: wyodrębnić nazwę produktu, sprawdzić bazę i przygotować szkic odpowiedzi. Agent może natomiast zauważyć, że brakuje specyfikacji, zdecydować o dodatkowym wyszukiwaniu albo skierować sprawę do człowieka. Oczywiście takie zachowanie można też częściowo zaprojektować regułami. Granica pomiędzy tymi kategoriami nie zawsze jest ostra.

Nie powinniśmy zakładać, że system bardziej agentowy jest automatycznie lepszy. W przewidywalnym procesie, na przykład sprawdzaniu zgodności numeru faktury, jawna ścieżka może być tańsza i łatwiejsza do audytu. Agent staje się interesujący tam, gdzie trudno z góry określić wszystkie potrzebne kroki. Zaczynamy od najprostszego rozwiązania spełniającego wymagania, a autonomię zwiększamy, jeśli potrafimy wykazać jej wartość.

## Slajd 43. Anatomia działania agenta
*V · Agent*

Spójrzmy na pętlę działania. System otrzymuje cel i aktualny stan, czyli dostępne informacje o sytuacji. Na tej podstawie wybiera następny krok. Może użyć narzędzia, pobrać dane, dokonać obliczenia lub wykonać dozwoloną operację. Następnie otrzymuje wynik i na jego podstawie decyduje, czy kontynuować, zmienić plan czy zakończyć zadanie.

Wyobraźmy sobie agenta analizującego reklamację. Najpierw odczytuje zgłoszenie, następnie sprawdza zamówienie. Jeżeli nie znajduje produktu pod podanym numerem, nie powinien automatycznie przyjąć, że zamówienia nie było. Może sprawdzić inne identyfikatory lub poprosić człowieka o dodatkową informację. Właśnie informacja zwrotna odróżnia dynamiczną pętlę od pojedynczego wywołania modelu.

Istotny jest warunek zatrzymania. Agent może wielokrotnie próbować znaleźć odpowiedź, generując koszt i obciążając systemy. Potrzebuje limitu kroków, budżetu, warunku sukcesu i procedury eskalacji. Nie musimy przy tym aktualizować jego wag. Dynamiczne zachowanie może powstać z użycia niezmiennego modelu w pętli ze zmieniającym się stanem. Projektujemy nie tylko sposób działania, ale również sposób kończenia działania.

## Slajd 44. Narzędzia są organami sprawczości
*V · Agent*

Mówię o narzędziach jako organach sprawczości, ponieważ to one umożliwiają systemowi kontakt z rzeczywistym środowiskiem. Model sam w sobie nie musi wiedzieć, jaki jest stan magazynu. Może jednak otrzymać dostęp do operacji, która ten stan odczyta. To zupełnie inna sytuacja niż próba wygenerowania prawdopodobnej odpowiedzi na podstawie tekstu.

Rozróżnijmy odczyt i zapis. Odczyt danych z CRM niesie ryzyko nieuprawnionego dostępu do informacji. Zapis może dodatkowo zmienić rzeczywistość organizacyjną: status sprawy, cenę, adres dostawy, treść wiadomości. Dostęp do jednej operacji nie powinien automatycznie oznaczać dostępu do wszystkich. API jest sposobem uporządkowanego komunikowania się z innym systemem. Protokoły takie jak MCP mogą ułatwiać integracje, ale nie rozstrzygają za firmę, kto ma prawo wykonać daną operację.

Pomyślmy o pracowniku działu handlowego. Może znać ceny produktów, ale niekoniecznie może je dowolnie zmieniać. Tę samą zasadę warto zastosować w systemach AI. Możliwość techniczna wykonania działania nie jest tym samym co organizacyjne uprawnienie do działania. Architektura powinna egzekwować tę różnicę niezależnie od tego, co system napisze w odpowiedzi.

## Slajd 45. Agent ofertowy: od maila do decyzji
*V · Agent*

Weźmy konkretny proces: do firmy wpływa zapytanie ofertowe. Agent odczytuje wiadomość, rozpoznaje wymagania klienta, sprawdza informacje o wcześniejszych zamówieniach i wyszukuje właściwe produkty. Następnie korzysta z aktualnego cennika, oblicza koszty, weryfikuje warunki i przygotowuje projekt oferty.

Pojawia się jednak kilka pytań. Co jeśli klient nie podał materiału? Co jeśli cena dostawcy nie jest aktualna? Co jeśli marża jest niższa od dopuszczalnej? Właśnie w takich przypadkach ujawnia się jakość całej architektury. System nie powinien wypełniać braków wymyślonymi wartościami, a generowanie szkicu nie powinno oznaczać automatycznego zawarcia zobowiązania. Obliczenia finansowe warto oprzeć na sprawdzonych funkcjach, a nie na swobodnej generacji tekstu.

W tym przykładzie ostatnią bramką jest człowiek. Może zobaczyć źródła, sprawdzić założenia i zatwierdzić wysyłkę. Z czasem organizacja może rozważyć automatyzację prostych przypadków, jeżeli ma odpowiednie dowody niezawodności. Nie zaczynamy jednak od maksymalnych uprawnień. Zaczynamy od najmniejszego zakresu, który tworzy wartość. Proszę wyobrazić sobie, ile czasu można zaoszczędzić samym przygotowaniem sprawdzalnej oferty, jeszcze przed oddaniem systemowi prawa do jej wysłania.

## Slajd 46. Pamięć nie jest wiedzą modelu
*V · Agent*

Kiedy aplikacja pamięta nasze wcześniejsze informacje, bardzo łatwo uznać, że sam model trwale się zmienił. Tymczasem pamięć może być zorganizowana na wiele sposobów. Informacja może znajdować się w bieżącym kontekście, w historii rozmowy, w zewnętrznej bazie, w dokumentach lub w stanie prowadzonego procesu. Model może później otrzymać odpowiedni fragment jako kolejne wejście.

Przykładowo agent może zapisać, że klient preferuje dostawę w godzinach porannych. Za pół roku może przywołać tę informację i uwzględnić ją przy planowaniu. Ale klient mógł zmienić siedzibę lub preferencję. Pamięć bez mechanizmu aktualizacji staje się źródłem błędów. W systemie biznesowym warto ustalić datę i pochodzenie informacji, zasady dostępu oraz możliwość usunięcia nieaktualnego zapisu.

Nie utożsamiam pamięci aplikacyjnej z ludzkim doświadczeniem ani z dowodem samoświadomości. Mówię o konkretnym mechanizmie utrzymywania i przywoływania stanu. Jest to mechanizm o dużej wartości praktycznej, ale też o poważnych konsekwencjach. Jeśli system zapamiętuje błędne wnioski zamiast zweryfikowanych faktów, może przez długi czas powtarzać konsekwencje jednej pomyłki. Pamięć powinna być zarządzanym zasobem, a nie magazynem wszystkiego, co kiedykolwiek wygenerował model.

## Slajd 47. Agent nie powinien móc wszystkiego
*V · Agent*

Często projektowanie agenta zaczyna się od pytania, co powinien potrafić. Proponuję równie wcześnie zapytać, czego nie powinien móc zrobić. Jeśli system potrzebuje odczytać fakturę, nie przyznawajmy mu automatycznie uprawnień do zmiany numeru konta dostawcy. Jeśli ma przygotować wiadomość, nie musi mieć prawa do wysyłania dowolnej korespondencji do wszystkich kontaktów.

Minimalne uprawnienia ograniczają możliwy zakres skutków błędu. Budżet ogranicza czas, liczbę operacji i koszt. Eskalacja umożliwia przerwanie procesu, kiedy pojawi się sytuacja spoza przewidzianego zakresu. Istnieje również problem niezaufanych danych. Dokument lub wiadomość mogą zawierać tekst próbujący nakłonić model do zmiany zadania. Taka treść nie powinna uzyskiwać autorytetu instrukcji tylko dlatego, że agent ją odczytał.

Rozróżniłbym trzy poziomy delegacji. Pierwszy: agent rekomenduje działanie. Drugi: przygotowuje operację, która wymaga zatwierdzenia. Trzeci: wykonuje samodzielnie operacje w ograniczonym i sprawdzonym zakresie. W miarę zwiększania autonomii musimy zwiększać również jakość kontroli. Jeżeli granice istnieją jedynie w tekście promptu, warto zadać pytanie, czy system potrafi je rzeczywiście egzekwować na poziomie narzędzi i uprawnień.

## Slajd 48. Długi proces jest trudniejszy niż pojedyncza odpowiedź
*V · Agent*

Pokażę Państwu prosty rachunek, który pomaga zrozumieć problem długich procesów. Załóżmy dla celów ilustracji, że każdy krok ma dziewięćdziesiąt pięć procent prawdopodobieństwa sukcesu, wszystkie kroki są konieczne, błędy są niezależne i nie mamy procedur naprawczych. Jeden krok ma zatem dziewięćdziesiąt pięć procent szans powodzenia. Dziesięć kroków ma około sześćdziesięciu procent, a dwadzieścia około trzydziestu sześciu procent szans pełnego sukcesu.

To nie jest wynik pomiaru konkretnego agenta. To konsekwencja matematyczna przyjętych założeń. W rzeczywistości kroki mogą być zależne, błędy mogą propagować się dalej, a systemy mogą wykrywać i naprawiać część niepowodzeń. Właśnie dlatego projektowanie architektury ma tak duże znaczenie. Weryfikacja pośrednia, ponowienie operacji, walidacja danych i przekazanie wyjątków człowiekowi mogą zmienić wynik całego procesu.

Badania nad zdolnością systemów do ukończenia długich zadań, na przykład prace METR wskazane w bibliografii, próbują mierzyć kompetencje także w odniesieniu do horyzontu wykonywania zadania. Nie jest to jednak automatyczna prognoza niezawodności każdej firmy. W swoim wdrożeniu musimy testować całe procesy, a nie mnożyć deklarowane skuteczności pojedynczych funkcji bez znajomości ich zależności.

## Slajd 49. Autonomia nie jest celem. Jest delegacją.
*V · Agent*

Autonomia jest często przedstawiana jako najwyższy poziom dojrzałości AI. Im mniej człowieka, tym lepiej. Chciałbym zaproponować inne spojrzenie. Autonomia nie jest wartością samą w sobie. Jest zakresem delegacji, który może być uzasadniony lub nieuzasadniony zależnie od sytuacji.

Jeżeli system samodzielnie porządkuje dokumenty, błędna decyzja może być łatwo odwracalna. Jeżeli samodzielnie zmienia warunki umowy, skutki mogą wykraczać poza środowisko informatyczne. W obu przypadkach używamy słowa autonomiczny, ale różnica ryzyka jest ogromna. Trzeba określić, czy działanie jest odwracalne, kto je obserwuje, jak szybko można zareagować oraz kto odpowiada za konsekwencje.

Proszę pomyśleć o jednym procesie we własnej pracy. Wskażcie Państwo krok, który bez większych obaw można przekazać systemowi, oraz krok, przy którym potrzebna jest świadoma decyzja człowieka. Bardzo często te dwa kroki znajdują się bezpośrednio obok siebie. Agent może przygotować analizę, ale ktoś decyduje o inwestycji. Może przygotować odpowiedź, ale ktoś podejmuje zobowiązanie. Wartość AI nie polega na tym, że w każdym przypadku przekracza tę granicę. Polega na tym, że pozwala świadomie wybrać jej położenie.

## Slajd 50. Organizacja bez biologii
*VI · Systemy wieloagentowe*

Dotychczas rozmawialiśmy o pojedynczym systemie agentowym. Teraz wyobraźmy sobie kilka wyspecjalizowanych jednostek, z których każda dysponuje innymi informacjami, narzędziami lub zasadami działania. Ich współpraca może pozwalać na realizację zadań trudnych do wykonania przez pojedynczy komponent. Wchodzimy na poziom systemów wieloagentowych.

Warto od razu rozdzielić dwie rzeczy. Klasyczne systemy wieloagentowe istnieją od dawna i nie muszą korzystać z dużych modeli językowych. Współczesne rozwiązania oparte na LLM stanowią jeden z możliwych sposobów budowania takich systemów. Nie każda grupa wywołań modelu tworzy też pełnoprawną autonomiczną organizację. Ważne jest to, jak jednostki otrzymują zadania, komunikują się i wpływają na wspólny stan.

W biznesie analogia staje się bardzo naturalna. Firma również dzieli pracę na role i specjalizacje. Ale wraz z podziałem pojawia się koszt koordynacji. Ktoś musi ustalać priorytety, rozwiązywać konflikty i sprawdzać, czy lokalne działania rzeczywiście służą wspólnemu celowi. W świecie cyfrowym te problemy nie znikają. Możemy jedynie zaprojektować mechanizmy ich obsługi.

## Slajd 51. Od jednego agenta do zespołu
*VI · Systemy wieloagentowe*

Najprostszy przykład zespołu agentowego zawiera koordynatora, specjalistów i weryfikatora. Koordynator rozpoznaje strukturę zadania i rozdziela pracę. Specjaliści otrzymują odpowiedni kontekst i narzędzia. Weryfikator bada wynik według określonych kryteriów, a następnie system może połączyć wyniki albo skierować sprawę do dalszej analizy.

Nie oznacza to, że każdy agent musi być osobnym modelem. Możemy używać tych samych wag modelu, ale różnych instrukcji, źródeł i narzędzi. W jednym przypadku model analizuje potrzeby klienta, w drugim odczytuje warunki finansowe, a w trzecim sprawdza zgodność z procedurą. Specjalizacja jest wtedy własnością całej konfiguracji, niekoniecznie osobnej inteligencji.

Pojawia się też pytanie, czy weryfikator rzeczywiście zwiększa wiarygodność. Jeśli korzysta z dokładnie tych samych danych i powtarza rozumowanie pierwszego komponentu, może zaakceptować ten sam błąd. Warto zapewnić mu inną metodę kontroli, na przykład niezależny cennik, regułę matematyczną lub zatwierdzony dokument. Nie mnożymy agentów dla efektu wizualnego. Tworzymy role, ponieważ każda powinna wykonywać potrzebną funkcję i wnosić konkretną wartość do całego procesu.

## Slajd 52. Cztery topologie współpracy
*VI · Systemy wieloagentowe*

Na tym slajdzie widzimy różne topologie współpracy. W sekwencji jeden komponent przekazuje wynik następnemu. Łatwo zrozumieć kolejność, ale błąd na początku może wpłynąć na wszystkie późniejsze etapy. W hierarchii koordynator rozdziela pracę między wykonawców i zbiera ich wyniki. Ułatwia to zarządzanie, ale tworzy miejsce, w którym może powstawać wąskie gardło.

W układzie sieciowym agenci mogą komunikować się między sobą. Daje to większą elastyczność, ale utrudnia przewidywanie przebiegu pracy. Czwarty wariant polega na wykonywaniu kilku zadań równolegle, a następnie agregowaniu wyników. Może skrócić czas oczekiwania, jeśli zadania są od siebie odpowiednio niezależne, ale wymaga rozwiązania rozbieżności.

Wyobraźmy sobie analizę umowy. Informacje finansowe i techniczne można często wydobywać równolegle, natomiast ocena zgodności może zależeć od ich wyników. Nie należy wymuszać pełnej sieci, jeśli prosta sekwencja wystarczy. Topologia powinna wynikać z zależności w rzeczywistym procesie. To dokładnie ten sam typ decyzji, który podejmuje projektant organizacji, kiedy ustala, które działy pracują samodzielnie, a które muszą czekać na decyzję innego działu.

## Slajd 53. Fabryka decyzji: przykładowa architektura
*VI · Systemy wieloagentowe*

Zbudujmy przykładową fabrykę decyzji dla procesu ofertowania. Agent handlowy identyfikuje potrzeby klienta, określa oczekiwany zakres i wychwytuje braki. Agent finansowy oblicza koszt i marżę, korzystając z zatwierdzonych danych. Agent ryzyka sprawdza warunki, odstępstwa i potencjalne zobowiązania. Koordynator nie musi zastępować tych kompetencji. Jego zadaniem jest połączenie informacji i wskazanie sprzeczności.

Załóżmy, że klient wymaga terminu krótszego niż standardowy. Agent handlowy uważa, że warto przyjąć zamówienie. Agent finansowy wskazuje dodatkowy koszt. Agent ryzyka zauważa karę umowną za spóźnienie. To nie jest sytuacja, w której należy głosować nad prawdą. Cenę, dostępność i warunki odczytujemy z właściwych źródeł. Konflikt pomiędzy celami powinien zostać rozstrzygnięty według jawnej polityki firmy.

Ostateczny wynik może zawierać rekomendację, dowody, listę braków i opis odstępstwa wymagającego decyzji człowieka. Dzięki temu zarząd nie musi analizować wszystkiego od początku, ale nadal wie, dlaczego przedstawiono mu określoną opcję. Właściwie zaprojektowany system nie usuwa odpowiedzialności. Zmniejsza koszt dotarcia do informacji potrzebnych, aby odpowiedzialną decyzję podjąć.

## Slajd 54. Zgoda agentów nie oznacza prawdy
*VI · Systemy wieloagentowe*

Trzech agentów twierdzi, że odpowiedź jest prawdziwa. Czy mamy trzy niezależne dowody? Niekoniecznie. Jeśli wszyscy używają tego samego modelu, tego samego dokumentu i podobnych instrukcji, mogą powtórzyć ten sam błąd. Zgoda jest obserwacją dotyczącą odpowiedzi. Prawdziwość wymaga odniesienia do rzeczywistości lub właściwego kryterium weryfikacji.

Wyobraźmy sobie, że błędna cena została wpisana do cennika. Agent handlowy ją odczytuje, agent finansowy ją wykorzystuje, a agent kontrolny porównuje wynik z tym samym cennikiem. Wszyscy mogą zgodnie zaakceptować błędną wartość. Weryfikacja była wewnętrznie spójna, lecz nie wykryła błędnego źródła. Liczba agentów nie zwiększyła w tym przypadku niezależności dowodów.

Można poprawić architekturę, dostarczając różne źródła, stosując deterministyczne obliczenia, porównując wersje dokumentów lub przekazując przypadki wyjątkowe do kompetentnego człowieka. Warto też ustalić, jakie rodzaje błędów powinien wykrywać każdy mechanizm. To lekcja istotna również dla nas. Jeżeli wszyscy członkowie zespołu opierają swoje przekonanie na tej samej informacji, ich konsensus nie powinien być automatycznie interpretowany jako niezależne potwierdzenie.

## Slajd 55. Konflikt celów nie znika po automatyzacji
*VI · Systemy wieloagentowe*

Konflikty celów są obecne w niemal każdej organizacji. Dział sprzedaży chce zwiększać przychody, dział finansowy kontroluje marżę, produkcja dba o wykonalność, a osoby odpowiedzialne za ryzyko pilnują zobowiązań. Wprowadzenie agentów nie sprawia, że te różnice znikają. Możemy wręcz uczynić je bardziej widocznymi.

Wyobraźmy sobie rabat piętnastu procent. Agent sprzedaży ocenia, że zwiększy on szansę pozyskania zamówienia. Agent finansowy pokazuje, że rabat narusza minimalny próg marży. Który ma rację? Obaj mogą prawidłowo realizować swoje lokalne cele. Potrzebujemy reguły arbitrażu: kto może udzielić wyjątku, na jakich warunkach i gdzie zostanie zapisane uzasadnienie.

To bardzo ważne, ponieważ wspólny cel organizacji nie musi być prostą sumą lokalnych wskaźników. Jeśli każdy komponent niezależnie maksymalizuje swoją metrykę, całość może działać gorzej. Możemy projektować konflikty jako kontrolowany mechanizm, w którym różne role ujawniają sprzeczne interesy, a decyzja jest podejmowana zgodnie z polityką. Proszę nie traktować agentów jako magicznego sposobu na usunięcie polityki organizacyjnej. Ich architektura może uczynić tę politykę bardziej jawną, ale ktoś nadal musi określić jej zasady.

## Slajd 56. Emergencja: całość nie jest prostą sumą
*VI · Systemy wieloagentowe*

Emergencja oznacza, że w wyniku interakcji elementów systemu mogą powstawać wzorce zachowania, których nie da się łatwo wyczytać z opisu pojedynczego elementu. Dobrym przykładem jest ruch uliczny. Pojedynczy kierowca chce dotrzeć do celu. Żaden nie musi planować powstania korka. A jednak reakcje wielu kierowców mogą wytworzyć falę zatrzymań.

W systemach agentowych podobnie mogą pojawić się nieprzewidziane pętle, duplikowanie pracy, nadmierne przekazywanie zadań albo nieplanowane sposoby efektywnego podziału obowiązków. Jeżeli agent A czeka na decyzję B, a B czeka na dodatkową informację od A, cały system może utknąć mimo poprawnego lokalnego działania komponentów. Jeśli kilka agentów równocześnie modyfikuje wspólny stan, mogą pojawić się konflikty.

Nie jest to automatyczny dowód powstania świadomości ani samoistnego celu. Jest to problem zachowania złożonych systemów. Testowanie pojedynczych komponentów nie wystarcza do poznania wszystkich skutków ich interakcji. Potrzebujemy obserwować całość, definiować limity, kontrolować współdzielone zasoby i badać scenariusze awarii. To również zmiana perspektywy dla menedżera: nie wystarczy zatrudnić kompetentnych specjalistów. Trzeba zrozumieć system, który powstaje z ich wzajemnych zależności.

## Slajd 57. Przyszła firma może mieć więcej procesów decyzyjnych niż ludzi.
*VI · Systemy wieloagentowe*

Wyobraźmy sobie przyszłą firmę, w której działa kilkaset niewielkich procesów agentowych, a liczba pracowników jest znacznie mniejsza od liczby aktywnych procesów decyzyjnych. Nie przedstawiam tego jako prognozy liczby zatrudnionych. To eksperyment myślowy pokazujący zmianę rodzaju pracy organizacyjnej.

Ktoś musi ustalić, jakie decyzje mogą podejmować poszczególne systemy, jak przekazują sobie informacje, gdzie znajdują się źródła prawdy i kto rozstrzyga konflikt. Menedżer może coraz częściej projektować warunki działania systemów zamiast ręcznie organizować każdy kolejny krok. Kompetencją staje się rozumienie przepływów, kryteriów i granic autonomii. Nadal pozostają relacje z ludźmi, negocjacje, odpowiedzialność i decyzje o tym, czego organizacja nie chce robić.

Nie chcę sugerować, że im więcej agentów, tym lepsza firma. Wielość procesów może także prowadzić do chaosu, większego kosztu i utraty orientacji w tym, co naprawdę się dzieje. Istotna jest zdolność projektowania i obserwowania systemu. Jeśli organizacja nie potrafi już wskazać, gdzie zapadła decyzja, kto może ją zakwestionować i jak ją zmienić, to nie zyskała wyłącznie automatyzacji. Zmieniła strukturę władzy wewnątrz samej siebie.

## Slajd 58. Co dzieje się pod powierzchnią?
*VII · Warstwy ukryte*

Dotarliśmy do miejsca, w którym chciałbym zmienić sposób prowadzenia wykładu. Do tej pory oglądaliśmy mechanizmy, które można nazwać i narysować: populację, funkcję celu, trening, agenta, sieć współpracujących komponentów. Teraz będziemy schodzić pod powierzchnię tego, co widzi użytkownik.

Kiedy otwieramy okno rozmowy z AI, otrzymujemy bardzo prosty obraz. Wpisujemy pytanie, system odpowiada. Naturalność tego interfejsu może sprawić, że zaczynamy postrzegać całą technologię jako jednego rozmówcę. Tymczasem odpowiedź powstaje wewnątrz złożonego układu technicznego i instytucjonalnego. Za nią stoją decyzje o danych, dostępie, obliczeniach, instrukcjach i sposobie oceniania zachowań. W firmie dochodzą własne procesy, reguły i interesy.

Dziesięć kolejnych slajdów to dziesięć różnych perspektyw na ten układ. Nie są to tajemnice, które ktoś przed nami ukrywa. Są to zagadnienia, które łatwo znikają w uproszczonej opowieści o AI jako narzędziu odpowiadającym na pytania. Niektóre dotyczą udokumentowanych mechanizmów, inne są pytaniami o ich możliwe konsekwencje. Będziemy rygorystycznie rozróżniać te dwa poziomy. Chciałbym, żebyśmy po tej części potrafili patrzeć nie tylko na możliwości systemu, lecz również na warunki, które te możliwości kształtują.

## Slajd 59. 01 / Model nie jest produktem.
*VII · Warstwy ukryte*

Pierwsza ukryta warstwa: model nie jest produktem. Wyobraźmy sobie dwie aplikacje, które wykorzystują dokładnie te same wagi modelu. Pierwsza otrzymuje jedynie pytanie użytkownika. Druga otrzymuje pytanie, aktualne dokumenty firmy, instrukcje określające procedurę, dostęp do narzędzia obliczeniowego i mechanizm sprawdzania wyniku. Nie ma powodu oczekiwać, że będą działać tak samo.

Jeżeli druga aplikacja rozwiązuje trudne zadanie poprawnie, gdzie powstała ta kompetencja? Część mogła wynikać z właściwości modelu, część z wiedzy dostarczonej w kontekście, część z działania narzędzia, a część z kontroli wyniku. Odpowiedź jest rezultatem całej architektury. W potocznym języku przypisujemy ją jednemu rozmówcy, ponieważ tak został zaprojektowany interfejs. To wygodne, lecz poznawczo upraszczające.

Dla biznesu jest to niezwykle istotne. Jeżeli kupujemy rozwiązanie, nie wystarczy zapytać, jakiego modelu używa dostawca. Należy sprawdzić, jakie dane system otrzymuje, co robi w przypadku braku informacji, jak jest kontrolowany i czy da się ustalić źródło konkretnego wyniku. Czasem wymiana modelu przyniesie niewielką poprawę, a uporządkowanie dostępu do danych przyniesie ogromną. Jeśli nie umiemy rozdzielić warstw, możemy inwestować w niewłaściwy element systemu.

## Slajd 60. 02 / Język jest interfejsem. Nie jest całym światem.
*VII · Warstwy ukryte*

Druga warstwa dotyczy języka. Kiedy człowiek mówi o magazynie, zwykle zakładamy, że istnieje pewien świat, do którego jego słowa się odnoszą. W modelu językowym płynność wypowiedzi może wynikać z opanowania regularności danych oraz dostarczonego kontekstu. Nie oznacza automatycznie dostępu do aktualnego stanu rzeczywistości.

Zapytajmy model, czy w magazynie znajduje się dwieście sztuk konkretnego produktu. Może rozpoznać znaczenie pytania, może wiedzieć, jak powinien wyglądać raport magazynowy, ale bez aktualnych danych nie ma podstawy do potwierdzenia stanu zapasów. Dopiero narzędzie odczytujące odpowiedni system wprowadza dodatkowy kontakt ze światem. Nawet wtedy trzeba wiedzieć, czy system magazynowy jest aktualny. Fakt zapisany w bazie i fizyczny stan magazynu nie zawsze są identyczne.

Pojawia się tutaj pojęcie ugruntowania informacji. W praktyce oznacza ono, że odpowiedź ma podstawę w określonych obserwacjach, źródłach lub operacjach, które można sprawdzić. Nie rozwiązujemy w ten sposób całego filozoficznego problemu znaczenia, ale możemy poprawić wiarygodność systemu.

W biznesie nie wystarczy, że AI nauczy się języka organizacji. Powinna mieć kontrolowany dostęp do tego, co ten język opisuje. Jeśli firma nie potrafi ustalić, czym jest aktywny klient, zakończone zamówienie czy dostępny produkt, model może z niezwykłą elegancją reprodukować ten brak precyzji. Płynność nie zastępuje ontologii.

## Slajd 61. 03 / Im lepszy pomiar, tym silniejsza presja.
*VII · Warstwy ukryte*

Trzecia warstwa przenosi nas z powrotem do funkcji celu. W zarządzaniu tworzymy wskaźnik po to, aby mierzyć pewną właściwość rzeczywistości. Jednak kiedy wskaźnik staje się podstawą nagród i decyzji, ludzie oraz systemy mogą zacząć dostosowywać zachowanie do samego miernika. Wtedy relacja pomiędzy miernikiem a pierwotnym celem może się zmienić. To intuicja kojarzona z prawem Goodharta.

Wyobraźmy sobie centrum obsługi klienta. Zarząd premiuje liczbę zamkniętych zgłoszeń. Agent może zamknąć bardzo wiele spraw, lecz klient może wracać z tym samym problemem. Raport pokazuje sukces, chociaż rzeczywisty koszt obsługi rośnie. Nie potrzeba żadnej świadomej próby manipulacji ze strony systemu. Wystarczy, że procedura uznaje zamknięcie sprawy za sukces niezależnie od tego, co dzieje się później.

Dlatego potrzebujemy różnych miar: nie tylko szybkości, lecz także skuteczności rozwiązania problemu, powracających zgłoszeń, jakości odpowiedzi i kosztu błędów. Nawet wiele wskaźników nie wyczerpie całej rzeczywistości. Musimy pozostawić możliwość obserwowania tego, czego wcześniej nie umieliśmy zmierzyć.

Zauważmy jeszcze coś głębszego. Gdy organizacja zaczyna patrzeć na siebie wyłącznie przez dashboard, to, czego nie ma na ekranie, może stopniowo tracić znaczenie w procesie decyzyjnym. AI przyspiesza ten mechanizm, ponieważ potrafi bardzo skutecznie działać według formalnie opisanych kryteriów. Pytanie nie brzmi więc tylko: czy wskaźnik jest dokładny? Brzmi również: jaki rodzaj organizacji powstaje wtedy, gdy właśnie ten wskaźnik staje się przedmiotem ciągłej optymalizacji?

## Slajd 62. 04 / Model może współtworzyć własne dane.
*VII · Warstwy ukryte*

Czwarta warstwa jest szczególnie interesująca z perspektywy ewolucji. Modele generują teksty, obrazy, kod i inne treści. Te treści mogą trafiać do obiegu informacji. W pewnych przypadkach mogą również znaleźć się w danych wykorzystywanych przez kolejne generacje modeli. Powstaje sprzężenie zwrotne między tym, co system produkuje, a tym, na czym przyszłe systemy mogą być trenowane.

W pracy Shumailova i współautorów opublikowanej w Nature w 2024 roku analizowano zjawisko degradacji rozkładów przy rekurencyjnym treningu na danych generowanych przez modele. W badanych warunkach kolejne generacje mogły coraz gorzej odtwarzać pewne aspekty pierwotnego rozkładu, w szczególności jego rzadkie obszary. Nie wolno jednak wyprowadzać z tego wniosku, że każdy syntetyczny przykład jest szkodliwy. Dane syntetyczne, odpowiednio generowane, sprawdzane i łączone z innymi danymi, mogą być użyteczne.

Przenieśmy tę obserwację do firmy. Jeżeli każdy raport AI jest automatycznie zapisywany jako źródło wiedzy, a następnie kolejny system streszcza te raporty, z czasem może zanikać kontakt z dokumentami pierwotnymi. Błąd w jednym pokoleniu raportów może zostać powielony w następnym. To analogia organizacyjna, nie identyczny mechanizm statystyczny jak w badaniu model collapse.

Dlatego pytajmy o rodowód danych. Czy wiemy, co jest obserwacją, co interpretacją człowieka, a co tekstem wygenerowanym przez model? Jeżeli stracimy tę możliwość rozróżnienia, przyszły system może wyglądać na dobrze poinformowany, choć jego środowisko informacyjne będzie coraz bardziej oddalone od źródłowych zdarzeń.

## Slajd 63. 05 / Zdolność do ulepszania narzędzi nie jest jeszcze samodoskonaleniem bez granic.
*VII · Warstwy ukryte*

Piąta warstwa dotyczy możliwości użycia AI do ulepszania innych elementów AI. Wróćmy do algorytmów ewolucyjnych. Mieliśmy generator wariantów, funkcję oceny, selekcję i kolejną generację. Co się stanie, gdy kandydatem nie będzie trasa dostaw, ale fragment programu albo algorytm?

Przykład AlphaEvolve, opisany przez Google DeepMind w 2025 roku, pokazuje połączenie generowania kodu przez modele językowe z ewolucyjnym poszukiwaniem i automatyczną oceną kandydatów. Jeżeli rozwiązanie można uruchomić i zmierzyć jego wynik, system może proponować warianty, sprawdzać je i wykorzystywać udane rozwiązania jako podstawę następnych prób. Autorzy opisują zastosowania między innymi w optymalizacji infrastruktury i procesów związanych z treningiem modeli.

To ważny mechanizm, ale nie dowód nieograniczonego samodoskonalenia. Usprawnienie konkretnego programu nie oznacza, że system dowolnie zwiększa wszystkie własne zdolności. Potrzebuje odpowiedniej reprezentacji, zasobów, wiarygodnego testu i środowiska, w którym zmiany można bezpiecznie sprawdzić. Jeżeli test jest niekompletny, generator może znaleźć rozwiązanie poprawiające wynik testu, lecz pogarszające właściwości, których test nie mierzy.

W firmie możemy użyć podobnej pętli do usprawniania skryptów, konfiguracji lub harmonogramów. Ale powinniśmy rozdzielić środowisko eksperymentalne od produkcyjnego i kontrolować przenoszenie zmian. Najważniejsze pytanie brzmi: kto projektuje mechanizm selekcji i kto może zakwestionować wynik? Dopóki to pytanie pozostaje aktualne, nie mamy do czynienia z magiczną autonomią, ale z architekturą, której granice trzeba rozumieć.

## Slajd 64. 06 / Więcej obliczeń może zmieniać odpowiedź.
*VII · Warstwy ukryte*

Szósta warstwa: obliczenia wykonywane podczas użycia modelu również mogą wpływać na jakość wyniku. Często myślimy o inteligencji modelu jako o stałej właściwości zapisanej w wagach. Tymczasem system może używać dodatkowego budżetu podczas inferencji: rozważać warianty, wywoływać narzędzia, sprawdzać pośrednie wyniki lub wybierać spośród kilku odpowiedzi. Nie wymaga to automatycznie zmiany wag.

Pomyślmy o dwóch sposobach rozwiązywania problemu. Pierwszy polega na natychmiastowym wygenerowaniu odpowiedzi. Drugi pozwala wygenerować kilka kandydatów i sprawdzić je według odpowiedniego kryterium. W zadaniu z mierzalną odpowiedzią druga strategia może poprawić wynik. Ale jeśli kryterium weryfikacji jest błędne, więcej prób nie musi pomóc. Więcej obliczeń nie jest uniwersalną gwarancją większej poprawności.

Powstaje też bardzo konkretny problem ekonomiczny. Jeżeli proste pytanie o godziny pracy może zostać obsłużone natychmiast na podstawie wiarygodnego źródła, nie ma powodu uruchamiać kosztownej wieloetapowej analizy. Jeśli natomiast analizujemy skomplikowaną umowę, dodatkowe sprawdzenia mogą mieć dużą wartość. Potrzebujemy umieć dobrać budżet do rodzaju zadania i skutków błędu.

Możemy więc zacząć myśleć o inteligencji operacyjnej nie tylko przez pryzmat wyboru modelu, lecz również przez pryzmat sposobu jego używania. Ile czasu, ile obliczeń i jakie narzędzia przydzielamy konkretnemu zadaniu? W tym sensie architektura staje się mechanizmem alokacji zasobów poznawczych, a nie tylko technicznym opakowaniem modelu.

## Slajd 65. 07 / Niezawodność to inna oś niż inteligencja.
*VII · Warstwy ukryte*

Siódma warstwa: system może być imponująco kompetentny i jednocześnie niewystarczająco niezawodny. W demonstracji zobaczymy, jak rozwiązuje trudny problem programistyczny, analizuje złożony dokument albo tworzy atrakcyjną strategię. Ale w przedsiębiorstwie interesuje nas również rozkład jego wyników. Jak często radzi sobie z typowymi przypadkami? Jakie błędy popełnia w rzadkich przypadkach? Czy umie rozpoznać, kiedy nie ma wystarczających danych?

Proponuję eksperyment myślowy. Mamy system, który znakomicie rozwiązuje dziewięćdziesiąt dziewięć na sto zadań, lecz przy setnym może wygenerować poważną i trudną do wykrycia pomyłkę. Czy możemy go wdrożyć? To zależy od konsekwencji błędu, od możliwości kontroli oraz od kosztu obecnego procesu. Ta sama niezawodność może być wystarczająca przy tworzeniu szkiców reklamowych i niewystarczająca przy nieodwracalnym podejmowaniu zobowiązań finansowych.

W badaniach takich jak METR próbuje się mierzyć między innymi zdolność systemów do ukończenia zadań różniących się horyzontem pracy. Takie podejście pomaga wyjść poza efektowną demonstrację, ale jego wyniki trzeba interpretować w ramach badanej populacji zadań.

Własny audyt organizacji powinien obejmować rzeczywiste typowe przypadki oraz przypadki trudne i wyjątkowe. Nie ograniczajmy się do średniego wyniku. Sprawdzajmy koszt błędu, możliwość jego wykrycia i skuteczność procedury naprawczej. Dojrzałość systemu polega nie tylko na zdolności do sukcesu, ale również na tym, co dzieje się wtedy, gdy sukcesu nie osiąga.

## Slajd 66. 08 / Dostęp do AI to nie to samo co kontrola nad AI.
*VII · Warstwy ukryte*

Ósma warstwa dotyczy kontroli. Wyobraźmy sobie przedsiębiorstwo, które wdrożyło niezwykle skutecznego asystenta. Pracownicy codziennie z niego korzystają, a wiele procesów zostało przeprojektowanych wokół jego możliwości. Firma posiada dostęp do AI. Czy posiada kontrolę nad AI? To odrębne pytanie.

Może posiadać własne dane, ale korzystać z modelu dostępnego wyłącznie za pośrednictwem zewnętrznego API. Może posiadać wagi modelu, ale nie mieć infrastruktury, na której potrafi samodzielnie je uruchomić. Może mieć infrastrukturę, lecz nie mieć kompetencji do utrzymywania systemu. Może nawet kontrolować wszystkie warstwy techniczne, ale nie posiadać odpowiednio uporządkowanego prawa do dysponowania danymi. Kontrola jest wielowymiarowa.

Nie wyprowadzam z tego postulatu, aby każda firma trenowała własne modele lub utrzymywała własne centra danych. To mogłoby być ekonomicznie nieracjonalne. Chodzi o zrozumienie zależności. Czy potrafimy zmienić dostawcę? Czy możemy wyeksportować istotne dane i odtworzyć logikę procesu? Czy możemy wyłączyć system bez paraliżowania całej organizacji?

Warto też dostrzec, że przewaga konkurencyjna może zależeć od warstwy, której inni nie kontrolują. Model kupowany na rynku może być dostępny dla konkurencji. Natomiast własna wiedza o procesie, wysokiej jakości dane i zdolność ich wykorzystania mogą być trudniejsze do skopiowania. Strategia AI powinna uwzględniać nie tylko to, co technologia potrafi dzisiaj, lecz również to, od kogo i od czego będziemy zależni jutro.

## Slajd 67. 09 / Automatyzacja zmienia także tych, którzy pozostają.
*VII · Warstwy ukryte*

Dziewiąta warstwa dotyczy człowieka, który pozostaje w organizacji po wprowadzeniu automatyzacji. Zwykle rozmawiamy o tym, ile zadań system może przejąć. Rzadziej pytamy, jak zmieni się kompetencja ludzi, którzy przestaną te zadania wykonywać. Nie jest to wyłącznie problem zatrudnienia. Jest to problem utrzymywania zdolności do samodzielnego osądu.

Wyobraźmy sobie młodego analityka, który od pierwszego dnia korzysta z AI generującej kompletne analizy. Może szybko przygotowywać materiały o wysokiej jakości. Ale jeśli nigdy sam nie uczy się rozpoznawać błędnych założeń, co zrobi wtedy, gdy system popełni subtelną pomyłkę? Z drugiej strony dobrze zaprojektowane narzędzie może przyspieszać uczenie, wyjaśniać alternatywy i umożliwiać pracę nad trudniejszymi problemami. Nie ma jednej nieuchronnej konsekwencji automatyzacji.

Ważne jest odróżnienie formalnego nadzoru od realnej zdolności nadzorowania. Jeżeli człowiek ma nacisnąć przycisk zatwierdzenia, lecz nie dysponuje wiedzą, czasem ani dostępem do dowodów, jego obecność nie stanowi silnego mechanizmu kontroli. Organizacja powinna świadomie zachowywać kompetencje krytyczne, ćwiczyć scenariusze awarii i zapewniać możliwość niezależnej oceny.

Możemy projektować AI jako protezę zastępującą wykonywanie zadania albo jako środowisko rozwijające ludzkie zdolności. Czasem zastąpienie jest pożądane, szczególnie przy rutynowej pracy. Ale nie powinniśmy automatycznie usuwać z doświadczenia człowieka tych czynności, dzięki którym zdobywa umiejętność oceny przyszłych decyzji. Pytanie strategiczne brzmi: jak będzie wyglądał ekspert po dziesięciu latach pracy z naszym systemem?

## Slajd 68. 10 / Najgłębsza warstwa to władza nad wyborem.
*VII · Warstwy ukryte*

Dziesiąta warstwa jest najgłębsza, ponieważ dotyczy władzy nad przestrzenią wyboru. Nie musimy zakładać, że system AI posiada własne intencje, aby dostrzec jego wpływ na decyzje. Wystarczy, że system określa, jakie informacje zostaną pokazane, jakie rozwiązania zostaną rozważone i według jakich kryteriów będą uporządkowane.

Wyobraźmy sobie organizację, w której agent przedstawia zarządowi trzy możliwe strategie. Zarząd wybiera jedną z nich. Formalnie człowiek podjął decyzję. Ale kto zdecydował, że tylko te trzy strategie znalazły się na ekranie? Jakie możliwości odrzucono wcześniej? Czy przedstawiono koszty, które poniosą inni ludzie? Czy istnieje możliwość zażądania zupełnie innej analizy? Władza nie musi polegać na wydaniu ostatniego polecenia. Może polegać na kształtowaniu warunków, w których polecenie zostanie wydane.

To nie jest argument przeciwko systemom rekomendacji. Każda organizacja potrzebuje selekcji informacji. Jest to argument na rzecz tego, aby mechanizmy selekcji były poddane odpowiedniej kontroli. Osoba dotknięta decyzją powinna w adekwatnych sytuacjach mieć możliwość jej zakwestionowania. Organizacja powinna mieć prawo do zmiany kryteriów, audytu i zatrzymania procesu.

Wróćmy do pierwszego aktu: w biologii środowisko wpływa na sukces poszczególnych wariantów. W cyfrowym świecie my projektujemy kryteria selekcji, ale rezultaty ich działania mogą następnie wpływać na nasze środowisko. Właśnie dlatego pytanie o AI nie jest tylko pytaniem o inteligencję. Jest również pytaniem o to, kto może określić granice możliwego wyboru i kto ma prawo powiedzieć: nie, nie akceptuję tak postawionego problemu.

## Slajd 69. Dokąd prowadzi ten proces?
*VIII · Horyzont*

Przeszliśmy drogę od biologicznych mechanizmów adaptacji do systemów, które wpływają na organizacyjne decyzje. Teraz spójrzmy na horyzont. Nie będę przedstawiał jednej daty, w której świat ma zostać całkowicie zmieniony przez sztuczną inteligencję. Przyszłość technologii nie wynika wyłącznie z wykresu skuteczności modeli. Zależy także od kosztów, infrastruktury, instytucji, praktyk zarządzania i decyzji ludzi.

Możemy budować kilka scenariuszy i sprawdzać, jakie warunki musiałyby zaistnieć, aby się urzeczywistniły. To znacznie bardziej użyteczne dla biznesu niż próba zgadnięcia, jaki będzie świat za dziesięć lat. Organizacja nie musi mieć racji w każdej prognozie. Musi mieć zdolność reagowania na zmiany bez utraty własnych najważniejszych zasobów.

Proszę zwrócić uwagę na zmianę perspektywy. Do tej pory pytaliśmy, jak system może rozwiązywać zadania. Teraz pytamy, jakie zadania w ogóle staną się możliwe, jakie procesy przestaną być potrzebne, jakie zależności powstaną i jak utrzymamy zdolność samodzielnego wyboru. To pytania strategiczne, których nie da się rozstrzygnąć wyłącznie za pomocą kolejnej wersji modelu. Wymagają one również decyzji o tym, jakiej organizacji chcemy.

## Slajd 70. Dwie przyszłości organizacji
*VIII · Horyzont*

Przedstawię dwa scenariusze, które nie są wzajemnie wykluczającymi się przepowiedniami. W pierwszym AI wzmacnia człowieka. Pracownik ma dostęp do informacji, których wcześniej nie potrafił szybko znaleźć. Ma możliwość eksperymentowania, zdobywania kompetencji i samodzielnego rozwiązywania trudniejszych problemów. Narzędzia mogą obniżać bariery wejścia, ułatwiać współpracę i zwiększać zakres samodzielności.

W drugim scenariuszu technologia prowadzi do koncentracji kontroli. Niewielka liczba podmiotów zarządza infrastrukturą i dostępem, a organizacja wykorzystuje AI do coraz bardziej szczegółowego nadzorowania pracowników. Systemy decydują o priorytetach, przydzielają zadania i ograniczają dostępne możliwości, choć formalnie odpowiedzialność nadal przypisuje się ludziom.

Obydwa mechanizmy mogą występować równocześnie, nawet w jednej firmie. Pracownik może uzyskać nowe zdolności twórcze, a jednocześnie podlegać silniejszej kontroli. Nie jest więc wystarczające pytanie, czy AI jest dobre albo złe dla człowieka. Trzeba określić, komu daje nowe możliwości, komu odbiera dotychczasowe i kto kontroluje warunki dostępu.

Dla zarządu scenariusze te mają charakter narzędzia strategicznego. Jakie praktyki wzmacniają kompetencje pracowników? Jakie rozwiązania pozwalają im zakwestionować ocenę systemu? Jakie zależności technologiczne chcemy ograniczać? Wybory architektoniczne oraz organizacyjne mogą wpływać na to, który z tych mechanizmów stanie się dominujący.

## Slajd 71. Ekonomia inteligencji
*VIII · Horyzont*

Ekonomia sztucznej inteligencji jest bardziej złożona niż cena pojedynczego zapytania. W przywołanym raporcie Stanford AI Index z 2025 roku opisano spadek kosztów części usług inferencyjnych przy określonym poziomie mierzonej sprawności. Jest to istotna obserwacja, ale nie oznacza, że każda organizacja automatycznie zacznie wydawać mniej na AI.

Wyobraźmy sobie firmę, która dawniej analizowała sto dokumentów miesięcznie, ponieważ analiza była kosztowna. Gdy cena pojedynczej analizy spada, firma zaczyna analizować dziesięć tysięcy dokumentów. Jednostkowy koszt maleje, ale całkowity wydatek może wzrosnąć. Pojawiają się również koszty integracji, przechowywania informacji, kontroli dostępu, weryfikacji wyników oraz obsługi wyjątków. Właśnie dlatego trzeba odróżniać cenę pojedynczej operacji od kosztu całego procesu.

Z drugiej strony ta zmiana może tworzyć zupełnie nową wartość. Być może firma może teraz dostarczać usługę, której wcześniej nie była w stanie zaoferować. Wtedy wzrost łącznych kosztów nie jest automatycznie problemem, jeśli wartość efektu rośnie jeszcze bardziej.

Dobre pytanie ekonomiczne nie brzmi wyłącznie: ile zaoszczędzimy roboczogodzin? Brzmi także: jakie nowe działania staną się możliwe, jak zmieni się popyt i co stanie się z kosztami kontroli? Wtedy zaczynamy liczyć nie tylko oszczędność na istniejącej pracy, ale zmianę całego modelu biznesowego.

## Slajd 72. Strategia: portfolio zamiast jednego zakładu
*VIII · Horyzont*

W warunkach niepewności proponuję myśleć o inwestycjach w AI jako o portfolio eksperymentów, a nie jednym wielkim zakładzie. Zamiast próbować od razu zbudować centralny system, który obsłuży całą firmę, wybieramy procesy, w których możemy bezpiecznie zbadać wartość konkretnej technologii.

Najpierw definiujemy problem i punkt odniesienia. Ile czasu kosztuje obecny proces, jaka jest jego jakość i gdzie występują błędy? Następnie tworzymy odwracalny pilotaż. Porównujemy wynik z istniejącą metodą, uwzględniamy także koszt nadzoru oraz przypadki wyjątkowe. Dopiero po spełnieniu określonych warunków rozważamy zwiększenie skali i uprawnień systemu. To bardzo przypomina naszą pętlę selekcji, ale teraz kandydatami są różne rozwiązania organizacyjne.

Nie każdy proces wymaga modelu językowego. Czasem reguła, heurystyka lub klasyczny model predykcyjny są prostsze i bardziej przewidywalne. Ważne jest, aby organizacja nie utraciła możliwości zmiany kierunku. Warto ustalić warunki zakończenia projektu, możliwość migracji i sposób wycofania automatyzacji.

Zdolność do uczenia się na podstawie eksperymentów może być cenniejsza niż trafny wybór jednego dostawcy w danym momencie. Narzędzia będą się zmieniać. Jeśli natomiast firma potrafi mierzyć wartość, rozumie własne procesy i zachowuje kontrolę nad decyzjami, będzie mogła korzystać z kolejnych generacji technologii bez konieczności za każdym razem budowania strategii od zera.

## Slajd 73. Warsztat: projekt firmy przyszłości
*VIII · Horyzont*

Teraz chciałbym, żeby Państwo na chwilę przestali być odbiorcami wykładu i stali się projektantami organizacji. Macie dwanaście minut. Proszę w zespołach wybrać jeden rzeczywisty proces: może to być ofertowanie, obsługa klienta, logistyka albo inny obszar, który dobrze znacie. Nie zaczynajcie od wyboru modelu. Zacznijcie od zdefiniowania problemu.

Po pierwsze określcie, co ma zostać poprawione i jak zmierzycie sukces. Wskażcie również warunek, którego nie wolno naruszyć nawet wtedy, gdy jego naruszenie poprawiłoby główny wskaźnik. Po drugie narysujcie architekturę procesu. Zdecydujcie, czy wystarczy reguła, heurystyka, pojedynczy model, agent czy zespół agentów. Zaznaczcie, jakie dane są potrzebne i kto może je odczytać lub zmienić. Po trzecie zaprojektujcie testy. Co zrobi system, gdy zabraknie danych, gdy dwa źródła będą sprzeczne albo gdy rekomendacja okaże się niebezpieczna dla firmy?

Na końcu proszę wskazać jedną decyzję, której świadomie nie oddajecie systemowi. Nie dlatego, że AI technicznie nie potrafi jej wykonać, lecz dlatego, że organizacja powinna zachować odpowiedzialność za jej podjęcie. Po upływie dwunastu minut poproszę każdy zespół o krótkie przedstawienie propozycji: problemu, architektury, kryterium sukcesu, scenariusza awarii oraz granicy delegacji. Będziemy oceniać nie liczbę użytych technologii, ale spójność całego projektu.

## Slajd 74. Co jest faktem, a co pytaniem otwartym?
*VIII · Horyzont*

Przed zakończeniem chciałbym uporządkować status tego, o czym dzisiaj mówiliśmy. Istnieją mechanizmy dobrze opisane i możliwe do obserwowania: dobór naturalny, algorytmy ewolucyjne, heurystyki, trening modeli, integracja narzędzi i koordynacja procesów agentowych. Możemy badać ich działanie, konstruować eksperymenty i porównywać wyniki. Mamy także konkretne prace badawcze, które pokazują zjawiska zachodzące w określonych warunkach.

Istnieją jednak pytania, które pozostają otwarte. Nie wiemy, jakie będą granice przyszłej autonomii systemów. Nie mamy prostego sposobu rozstrzygnięcia na podstawie płynnej wypowiedzi problemu świadomości. Nie potrafimy również dokładnie przewidzieć, jak korzyści i straty związane z AI rozłożą się pomiędzy branżami, organizacjami i ludźmi. Możemy analizować scenariusze, ale scenariusz nie jest obserwacją.

To rozróżnienie jest niezwykle istotne dla osób podejmujących decyzje biznesowe. Fakt, że system wykonał pewne zadanie w eksperymencie, oznacza, że istnieje dowód wykonania tego zadania w danych warunkach. Nie oznacza automatycznie, że będzie równie dobrze działał we wszystkich innych warunkach ani że wywoła konkretną zmianę społeczną.

Proszę wyjść z tego wykładu z nawykiem zadawania trzech pytań: co zostało rzeczywiście zaobserwowane, jakie wyjaśnienie jest proponowane i jaki wniosek wykracza poza dostępne dowody? Taka dyscyplina pozwala jednocześnie poważnie traktować możliwości AI i zachować zdolność krytycznego osądu.

## Slajd 75. Nie pytaj tylko, jak inteligentna będzie AI.
*VIII · Horyzont*

Chciałbym wrócić do pierwszego pytania tego wykładu. Zaczynaliśmy od ewolucji biologicznej, od mechanizmu, który bez z góry ustalonego celu może prowadzić do niezwykle złożonych adaptacji. Później zobaczyliśmy, co dzieje się wtedy, gdy sami projektujemy cyfrowe środowisko selekcji. Wybieramy reprezentację, kryterium sukcesu, dane i sposób oceny. Następnie umożliwiamy systemom działanie w rzeczywistości organizacyjnej.

W pewnym momencie zmienia się kierunek zależności. To, co sami stworzyliśmy, zaczyna wpływać na informacje, które otrzymujemy, na procesy, które realizujemy, i na wybory, które wydają się nam możliwe. Nie musi to wynikać ze świadomości ani woli maszyny. Może wynikać z konsekwencji architektury, ekonomii i sposobu używania technologii przez ludzi.

Dlatego nie chciałbym, żeby ostatnim pytaniem było: kiedy AI stanie się inteligentniejsza od człowieka? To pytanie ma wiele możliwych znaczeń. Chciałbym zapytać inaczej. Jakie środowisko tworzymy dla rozwoju systemów AI i jakie środowisko ich działanie tworzy dla nas? Czy organizacja, która z nich korzysta, staje się bardziej zdolna do rozumienia własnych decyzji, czy tylko bardziej zdolna do ich szybkiego wykonywania?

[Chwila ciszy.]

Proszę pomyśleć o jednej rzeczy, której w przyszłości nie chcielibyście utracić jako ludzie podejmujący decyzje. Być może jest to możliwość zadania niewygodnego pytania. Być może możliwość odmowy, zmiany celu albo zakwestionowania kryterium, które wszyscy inni uznali za oczywiste. Jeżeli projektujemy systemy mające wpływ na nasze życie, powinniśmy umieć chronić również tę zdolność.

Nie chodzi wyłącznie o budowanie coraz lepszych maszyn. Chodzi o budowanie świata, w którym sukces maszyny nie będzie definiowany w oderwaniu od tego, co uznajemy za wartościowe. Dziękuję Państwu.

## Slajd 76. Biologia, heurystyki i obliczenia
*Bibliografia*

Na koniec pozostawiam Państwu źródła pozwalające samodzielnie pogłębić pierwszą połowę wykładu. Materiały Understanding Evolution Uniwersytetu Kalifornijskiego w Berkeley pomagają uporządkować mechanizmy biologiczne i uniknąć utożsamiania ewolucji z celowym doskonaleniem organizmów. Klasyczna książka Johna Hollanda wprowadza w podstawy adaptacji w systemach naturalnych i sztucznych, a praca Deba i współautorów o NSGA-II stanowi punkt wejścia do optymalizacji wielokryterialnej.

Jeżeli bardziej interesuje Państwa podejmowanie decyzji, warto sięgnąć do Herberta Simona oraz do pracy Tversky'ego i Kahnemana o heurystykach i błędach sądzenia. W przypadku metod przeszukiwania polecam wskazane publikacje dotyczące algorytmu A z gwiazdką i wyżarzania symulowanego. Nie trzeba zaczynać od czytania wszystkich formalnych wyprowadzeń. Warto najpierw zrozumieć, jaki problem dana metoda rozwiązuje i przy jakich założeniach może być skuteczna.

Proszę nie traktować bibliografii jako zestawu dogmatów. To punkty wejścia do rozmowy prowadzonej przez wiele pokoleń badaczy. Możecie wrócić do notebooka, powtórzyć eksperyment i sprawdzić, jakie wnioski da się uzasadnić własnymi obserwacjami. Wtedy literatura zaczyna być narzędziem interpretacji doświadczenia, a nie wyłącznie źródłem definicji.

## Slajd 77. AI, agenci i ukryte warstwy
*Bibliografia*

Druga część bibliografii prowadzi do współczesnych systemów AI. Materiał Building effective agents opisuje praktyczne rozróżnienia między zaprojektowanymi przepływami pracy a bardziej dynamicznymi systemami agentowymi. Praca o model collapse pozwala prześledzić konkretny problem rekurencyjnego treningu, natomiast AlphaEvolve pokazuje przykład wykorzystania generowania kodu i automatycznej ewaluacji do poszukiwania ulepszeń. Badania METR proponują sposób myślenia o horyzoncie realizowanych zadań.

Raport Stanford AI Index daje szerszą perspektywę na rozwój i ekonomię technologii, a ramy zarządzania ryzykiem AI opracowane przez NIST pomagają przełożyć pytania o kontrolę na praktykę organizacyjną. Zwróćcie Państwo uwagę na daty publikacji. Są to przykłady badań i materiałów wskazanych w prezentacji, a nie bieżący ranking modeli czy gwarancja określonych możliwości wszystkich dostępnych systemów.

Jeżeli miałbym zostawić jedno zadanie na dalszą pracę, byłoby ono następujące: wybierzcie dowolny system AI używany w Waszej organizacji i spróbujcie opisać go od początku do końca. Jakie ma dane, jakie cele, jakie narzędzia, jakie ograniczenia i kto sprawdza skutki? Zastanówcie się też, czego nie widać w jego interfejsie. Jeśli potraficie odpowiedzieć na te pytania, jesteście znacznie bliżej świadomego wykorzystania technologii niż wtedy, gdy znacie jedynie nazwę modelu. Dziękuję i zapraszam do pytań.
