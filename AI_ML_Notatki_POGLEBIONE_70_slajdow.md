# SZTUCZNA INTELIGENCJA: HISTORIA, ALGORYTMY ML, SIECI NEURONOWE

## Rozbudowane notatki prowadzącego do 70 slajdów

**Marcin Albiniak, Ph.D. • COMARCH • 23–26 listopada 2026**

**Cel dokumentu.** To scenariusz do opowiadania, a nie tekst do odczytywania ze slajdów. Każdy slajd ma rozwiniętą narrację, interpretację „głębszego dna”, przykład lub pytanie. Formuły służą zrozumieniu procesu, nie pokazowi rachunków dla samych rachunków.

**Prowadzenie.** Fragmenty „Scenariusz mówiony” można opowiadać niemal dosłownie. Fragmenty „Głębsze dno” służą wydobyciu założeń, konsekwencji i granic modeli. Pytania warto zadawać przed odkryciem pełnej odpowiedzi. Rozdziały I–IV odwzorowują moduły prezentacji. Slajdy 53 i 57 mają animację; instrukcja objaśnia, co ona ilustruje, a czego nie.

**Ważne rozróżnienia.** *Model* to formalna reprezentacja i mechanizm obliczeniowy; *system* to model wraz z danymi, narzędziami, regułami i ludźmi. *Predykcja* nie dowodzi przyczynowości. *Kompetencja zadaniowa* nie rozstrzyga świadomości. *Wynik testu* jest ograniczony warunkami pomiaru.

**Czas.** To materiał do pogłębionego wykładu i dyskusji. Przewiduj około 2–4 minut narracji na większość slajdów oraz więcej czasu na pytania, animacje i rachunek z przykładu 58. Nie jest to pełny warsztat praktyczny na cztery dni.

---

## BLOK I. OTWARCIE, HISTORIA I NATURA SZTUCZNEJ INTELIGENCJI

### 01. Od idei inteligencji do sieci neuronowych

**Scenariusz mówiony.** „Na tym szkoleniu spróbujemy zrobić coś trudniejszego niż pokazać, że AI działa. Spróbujemy zrozumieć, *dlaczego* działa, *co* tak naprawdę wykonuje i *kiedy* wynik jest wiarygodny. Proszę na chwilę odłożyć na bok chatboty. Sztuczna inteligencja ma historię znacznie dłuższą niż dzisiejsze modele językowe. Są w niej logika, teoria obliczeń, statystyka, psychologia poznawcza, neurobiologia, a w końcu geometria i optymalizacja”. Rozpocznij od trzech pytań: czy dobra decyzja jest tym samym co inteligencja; czy wytrenowanie modelu jest tym samym co nauczenie go rzeczywistości; czy system, który rozwiązuje zadanie, rozumie jego znaczenie?

Wyjaśnij mapę podróży. Najpierw geneza AI i spór o definicję, następnie mechanika uczenia, później konkretne rodziny algorytmów, wreszcie wielowarstwowe sieci: neuron, funkcje aktywacji, przepływ w przód, błąd, gradient i propagacja wsteczna. Nie zaczynamy od narzędzi, bo technologia zmienia się szybciej niż matematyczne zasady.

**Głębsze dno.** Najważniejsza teza wykładu: model nie jest światem. Jest zbudowaną w pewnym celu reprezentacją wybranych aspektów świata. Każdy wybór zmiennej, etykiety i metryki wycina część rzeczywistości. Dlatego w AI zawsze istnieją trzy pytania: ontologiczne, *co uznajemy za obiekt i relację*; epistemologiczne, *skąd wiemy, że model jest trafny*; i praktyczne, *kto oraz z jakimi konsekwencjami użyje wyniku*. Algorytmy będziemy oglądać w tej potrójnej perspektywie.

**Pytanie do grupy.** „Czy program może idealnie klasyfikować obrazy, a jednocześnie nie wiedzieć, czym jest przedmiot na obrazie?” Zbierz różne odpowiedzi, nie rozstrzygaj jeszcze. Wrócisz do nich na slajdzie 70.

### 02. AI nie jest jednym algorytmem

**Scenariusz mówiony.** „Wyobraźmy sobie trzy systemy: komputer szachowy, narzędzie wykrywania oszustw i asystenta tekstowego. Wszystkie mogą trafić pod etykietę AI, ale pierwszy może opierać się przede wszystkim na przeszukiwaniu, drugi na estymacji ryzyka, trzeci na wielkich sieciach neuronowych. Jeżeli będziemy mówić o nich jak o jednym mechanizmie, nie zrozumiemy żadnego”. Rozróżnij *zadanie*, *metodę* i *system*. Zadanie to np. wykrycie awarii. Metoda to np. Random Forest. System to cały proces: zbieranie danych, model, interfejs, człowiek, procedury i odpowiedzialność.

Pokaż trzy tradycje: symboliczną, statystyczną i neuronową. W systemie symbolicznym człowiek jawnie zapisuje przesłanki; w statystycznym algorytm dopasowuje zależność do obserwacji; w neuronowym model wytwarza reprezentacje przez złożenie wielu transformacji. Dziś systemy często są hybrydowe.

**Głębsze dno.** Krytykuj „AI” jako termin reklamowy. Etykieta niczego nie mówi o stopniu autonomii, poziomie błędu ani o sposobie dowodzenia jakości. Nie każda poprawna odpowiedź jest dowodem rozumienia, podobnie jak płynne zdanie nie jest dowodem prawdziwości. Z drugiej strony nie trzeba przypisywać modelowi ludzkiej świadomości, aby uznać, że wykonuje użyteczne operacje poznawcze. Pytanie nie brzmi tylko „czy jest AI?”, lecz „jakim mechanizmem przekształca wejście w wyjście i na jakiej podstawie temu ufamy?”.

**Przykład i pytanie.** System wykrywa dwa razy więcej podejrzanych transakcji, ale blokuje uczciwych klientów. Czy jest „inteligentniejszy”? Zależy od funkcji kosztu. Zapowiedz, że później policzycie dokładnie ten kompromis.

### 03. Agenda: cztery filary rozumienia AI

**Scenariusz mówiony.** Przedstaw cztery filary jako cztery różne poziomy pytań. Historia i natura AI odpowiada na „co chcemy zbudować i dlaczego?”. Mechanizm uczenia odpowiada na „co właściwie znaczy dopasowanie do doświadczenia?”. Algorytmy ML odpowiadają na „jakie hipotezy dopuszczamy, jakie ograniczenia narzucamy i jak optymalizujemy?”. Sieci neuronowe odpowiadają na „jak powstają złożone reprezentacje i skąd bierze się możliwość uczenia bardzo wielu parametrów?”. Nie traktuj agendy jako listy produktów; pokaż rosnący poziom abstrakcji.

Wyjaśnij organizację: w każdym module będą intuicja, model matematyczny, przykład porażki oraz pytanie o sens wyniku. Uczestnik nie musi znać od razu rachunku różniczkowego, by pojąć, że pochodna opisuje wrażliwość błędu na zmianę wagi. Formalizacja przyjdzie po intuicji. Nie omawiamy instalacji ani bibliotek: narzędzia są implementacją idei, nie ich wyjaśnieniem.

**Głębsze dno.** Porządek modułów ma przyczynę. Jeśli nie wiemy, *co* jest reprezentowane, wybór algorytmu staje się technicznym rytuałem. Jeśli nie rozumiemy *czego* minimalizuje funkcja straty, pojęcie „uczy się” jest metaforą bez treści. Jeśli nie potrafimy zbadać generalizacji, największa sieć pozostaje tylko kosztowną maszyną dopasowania. Cały wykład dotyczy przejścia od zachwytu efektem do rozumienia mechanizmu.

**Pytanie do sali.** „Który z czterech filarów jest waszym zdaniem najczęściej pomijany w projektach AI?” Zanotuj odpowiedzi, wróć do nich na końcu.

### 04. Pięć pytań, które będziemy zadawać modelom

**Scenariusz mówiony.** „Gdy ktoś pokazuje mi model o skuteczności 97%, nie pytam najpierw, czy jest nowoczesny. Pytam: 97% czego, na jakim zbiorze, w jakim czasie i wobec jakiego punktu odniesienia?”. Przejdź przez pięć pytań jako procedurę audytu. Po pierwsze problem: predykcja, opis, optymalizacja czy decyzja? Po drugie wejście i wyjście: co obserwujemy i co chcemy wiedzieć? Po trzecie reprezentacja i uczenie: jakie parametry lub struktura są dostosowywane? Po czwarte błąd: jak zdefiniowano stratę i metrykę? Po piąte generalizacja: co stanie się, gdy sytuacja przestanie przypominać trening?

Rozwiń przykład predykcji rezygnacji klienta. „Rezygnacja” może znaczyć brak zakupów przez miesiąc, rozwiązanie umowy lub spadek aktywności. Każda definicja tworzy inne etykiety. Model może być matematycznie znakomity dla źle nazwanego celu. Dalej rozróżnij estymowane prawdopodobieństwo od decyzji o telefonie do klienta: próg i koszty działania nie wynikają automatycznie z modelu.

**Głębsze dno.** To pięć pytań epistemologicznych ukrytych w metodzie inżynierskiej. Każda odpowiedź zakłada pewną teorię świata: co istnieje w danych, jak mierzymy rzeczywistość i jaki błąd jesteśmy gotowi uznać za dopuszczalny. Wysoki wynik bez kontekstu pomiaru może być iluzją. Będziemy rozróżniać *prawdę zadaniową* (czy trafiliśmy w etykietę) od *rzetelności zastosowania* (czy wynik jest adekwatny do celu i konsekwencji).

**Ćwiczenie ustne.** Poproś uczestnika, by przeszedł przez pięć pytań na przykładzie klasyfikacji e-maili jako spam. Każda odpowiedź jest krótkim testem zrozumienia.

### 05. Historia i natura AI: otwarcie modułu

**Scenariusz mówiony.** „Zanim powstały procesory graficzne i modele fundamentalne, pojawiło się znacznie starsze pytanie: czy wnioskowanie da się opisać regułami, które wykona maszyna? Nie jest to tylko pytanie o prędkość rachunku. Chodzi o to, czy takie działania jak rozpoznawanie wzoru, wyciąganie wniosku, uczenie i planowanie mają formalną strukturę”. Zarysuj trzy źródła AI: logikę i idee mechanizacji rozumowania; matematykę prawdopodobieństwa i uczenia z niepewnych danych; inspirację biologicznym przetwarzaniem sygnałów.

Historia AI nie jest prostą linią od „głupich” do „mądrych” algorytmów. To historia kilkukrotnego przesuwania kryterium sukcesu. Gdy komputer nauczył się liczyć, liczenie przestało imponować. Gdy zaczął wygrywać w gry, pojawiło się pytanie o obraz, język i zdrowy rozsądek. Gdy zaczął płynnie pisać, pytamy o niezawodność i sprawczość.

**Głębsze dno.** Każda epoka wyodrębniała inny fragment inteligencji. Dawniej akcent padał na logiczny dowód, później na rozwiązanie problemu, następnie na rozpoznanie statystyczne, a dziś na adaptację, generowanie i operowanie narzędziami. Nie oznacza to, że znaleźliśmy jedną definicję obejmującą wszystkie zjawiska. W nauce brak jednego pomiaru inteligencji nie jest porażką; bywa sygnałem, że badamy rodzinę kompetencji.

**Przejście.** „Najpierw zatem ustalmy, czego dotyczy samo słowo AI”.

### 06. Co właściwie znaczy „sztuczna inteligencja”?

**Scenariusz mówiony.** Przedstaw definicję operacyjną: system maszynowy, który dla celów jawnych lub dorozumianych wyprowadza z wejść sposób tworzenia predykcji, treści, rekomendacji lub decyzji, z różnym stopniem autonomii i ewentualnej adaptacyjności. Podkreśl, że definicje regulacyjne, np. OECD i AI Act, są użyteczne do określania zakresu obowiązków, ale nie stanowią filozoficznej teorii świadomości. „Słowo *inferencja* oznacza tu proces wyprowadzania wyniku z modelu lub reguł; nie trzeba zakładać ludzkiego namysłu”.

Porównaj trzy rzeczy: **model** jest funkcją lub konstrukcją matematyczną; **system** otacza model danymi i procedurą użycia; **agent** może dodatkowo wybierać i wykonywać działania w otoczeniu. Wszystkie mają inną powierzchnię ryzyka. Model diagnozujący chorobę nie jest tym samym co cały proces kliniczny, w którym lekarz zatwierdza wniosek.

**Głębsze dno.** Definicja operacyjna płaci pewną cenę: mierzy zewnętrzne zachowanie i mechanizmy działania, nie rozwiązuje pytania o wewnętrzne przeżycie, intencję czy sens. Termin „inteligentny” staje się wtedy relacyjny: inteligentny *wobec zadania, środowiska i kryterium*. Dla inżyniera to zaleta, bo pozwala testować. Dla filozofa to punkt startowy, nie koniec sporu.

**Pytanie.** „Czy system, który bezbłędnie oblicza podatek, ale nie potrafi wyjaśnić przepisu, jest inteligentny?” Zachęć do odpowiedzi zależnej od zakresu zadania.

### 07. Od percepcji do działania: pięć funkcji inteligencji

**Scenariusz mówiony.** „Zamiast antropomorfizować model, potraktujmy inteligencję jako zestaw funkcji”. Percepcja zamienia sygnały w dane, reprezentacja organizuje je w cechy i relacje, wnioskowanie wyprowadza przewidywania lub konsekwencje, decyzja wybiera działanie przy ograniczeniach, uczenie poprawia przyszłe działanie na podstawie informacji zwrotnej. Poproś uczestników o podanie, gdzie kończy się model, a zaczyna system. W kamerze przemysłowej obraz to wejście; wykryte uszkodzenie to wynik modelu; zatrzymanie linii to decyzja systemowa, wymagająca osobnej polityki bezpieczeństwa.

Wyjaśnij, że te funkcje mogą być rozdzielone albo sklejone. Jeden model może zarazem reprezentować obraz i klasyfikować obiekty. Inny system używa jawnego grafu pojęć do wnioskowania. Model nie musi uczyć się w czasie rzeczywistym, aby należeć do AI; często adaptacja zachodzi wyłącznie podczas zaplanowanych etapów treningu.

**Głębsze dno.** Mamy do czynienia z architekturą przejścia od obserwacji do działania, a nie z kompletną teorią ludzkiej świadomości. Najbardziej krytyczny moment to przejście od „jest prawdopodobne, że...” do „należy zrobić...”. Predykcja i normatywna decyzja są różnymi kategoriami. Model może przewidywać opóźnienie dostawy, ale to człowiek lub jawna polityka określa, kiedy zmienić harmonogram i jakie ryzyko podjąć.

**Przykład.** Kontrola jakości: kamera, wykrycie rysy, klasyfikacja wady, odrzucenie elementu. Zapytaj, które elementy można zweryfikować metryką, a które wymagają zasad biznesowych.

### 08. AI a zwykła automatyzacja

**Scenariusz mówiony.** „Reguła: jeśli faktura ma termin płatności dziś, wyślij przypomnienie. Jest automatyzacją. Model: oszacuj, które faktury najprawdopodobniej nie zostaną opłacone w terminie. To predykcja. System: wybierz sposób kontaktu na podstawie predykcji i zasad obsługi. To dopiero rozwiązanie biznesowe”. Wyjaśnij różnicę między deterministycznie zapisaną procedurą a mechanizmem, który wyprowadza wynik z reguł wiedzy lub parametrów wyuczonych na danych. Zaznacz, że granice nie są absolutnie ostre: program oparty na regułach może być przykładem klasycznej AI, jeśli wykonuje nietrywialne wnioskowanie.

Pokaż dwa rodzaje niepewności. Automatyzacja może być deterministyczna i mimo tego popełniać błędy wynikające z niewłaściwej reguły. ML może zwracać prawdopodobieństwo, lecz po ustawieniu progu podejmować deterministyczną decyzję. Nie myl probabilistycznego mechanizmu z niestabilnością każdego wyniku.

**Głębsze dno.** Granica AI i automatyzacji jest również granicą *źródła wiedzy*: kto i gdzie zapisał zależności między światem a działaniem? Czasem w kodzie jawnie. Czasem w przykładach i ich statystycznej strukturze. Czasem częściowo w jednym, częściowo w drugim. To podpowiada strategię audytu: w systemie regułowym sprawdzamy kompletność reguł; w uczonym sprawdzamy dane, reprezentację, stratę i generalizację.

**Pytanie.** „Jeśli model sugeruje decyzję, lecz reguła biznesowa ją zawsze nadpisuje, gdzie znajduje się faktyczna sprawczość?”.

### 09. Trzy wielkie tradycje sztucznej inteligencji

**Scenariusz mówiony.** Najpierw logika symboliczna: pojęcia, relacje, ontologie, reguły typu „jeżeli X i Y, to Z”. Siłą jest jawność struktury i możliwość śledzenia reguły, słabością koszt modelowania świata. Następnie statystyka: model o pewnej rodzinie funkcji, parametrach i rozkładzie danych. Siłą jest uczenie z przykładów, słabością zależność od reprezentatywności próbek oraz często słabsza intuicyjna interpretacja. Następnie podejście neuronowe: struktura uczy się reprezentacji poprzez złożenie transformacji. Siłą jest adaptacja do obrazów, tekstu i dźwięku, kosztem obliczeń i trudniejszej analizy wewnętrznej.

Przedstaw hybrydę: system rozumie dokument dzięki modelowi neuronowemu, odczytuje zapisane relacje z grafu wiedzy i wykonuje działanie dopiero po zastosowaniu reguły dostępu. To nie kompromis z braku odwagi, lecz architektura odpowiadająca różnym wymaganiom.

**Głębsze dno.** Trzy tradycje to trzy odpowiedzi na pytanie „gdzie jest wiedza?”. W symbolach: jawnie w zdaniach i relacjach. W statystyce: w oszacowanej zależności i parametrach. W sieci: rozproszona w wagach i aktywacjach. Nie są to trzy niezgodne ontologie świata, ale trzy sposoby konstruowania reprezentacji. Model rzeczywistości może być zarazem logicznie ograniczony, statystycznie uczony i neuronowo wykonywany.

**Pytanie.** „Gdzie umieścilibyście zasady bezpieczeństwa: w wagach modelu, w bazie reguł czy w obu?” Odpowiedź powinna uwzględniać weryfikowalność i konsekwencje błędu.

### 10. AI, Machine Learning, Deep Learning, generatywność

**Scenariusz mówiony.** „AI to szeroka dziedzina tworzenia systemów, które wykonują czynności związane z wnioskowaniem, predykcją czy działaniem. Machine Learning to grupa metod, w których zdolność rozwiązywania zadania kształtuje się dzięki danym lub doświadczeniu. Deep Learning to część uczenia maszynowego oparta na wielowarstwowych sieciach uczących reprezentacji. Generatywność nie jest kolejnym kołem w środku wszystkich pozostałych. Jest charakterem zadania: tworzeniem nowych próbek lub treści zgodnie z wyuczonym modelem”.

Podaj kontrprzykłady. Drzewo klasyfikujące reklamacje jest ML, ale nie DL. CNN rozpoznający wady jest DL, lecz nie generuje obrazu. Model dyfuzyjny generujący obraz jest generatywny i oparty na DL. Starsze modele probabilistyczne również mogły generować próbki, choć nie były głębokimi sieciami.

**Głębsze dno.** Klasyfikacja terminów nie jest pedanterią, bo nazwy sugerują inne metody weryfikacji. Rozpoznawanie klasy oceniamy trafnością i kalibracją. Generowanie wymaga dodatkowo oceny wierności, różnorodności, spójności, bezpieczeństwa i możliwości potwierdzenia faktów. Algorytm może być znakomity w generowaniu płynnego tekstu i słaby w rozwiązywaniu zadania wymagającego ścisłej zgodności z dokumentem.

**Pytanie.** „Czy system, który generuje idealnie brzmiącą, lecz fałszywą odpowiedź, odniósł sukces?” Zależy od celu: językowo, być może; epistemicznie i użytkowo, nie.

### 11. Czy zachowanie inteligentne oznacza rozumienie?

**Scenariusz mówiony.** „W tym miejscu trzeba oddzielić trzy sprawy. Kompetencja: czy system daje poprawną odpowiedź? Mechanizm poznawczy: jak przetwarza informację i wykorzystuje reprezentacje? Świadomość fenomenalna: czy coś jest dla tego systemu przeżyciem? Sukces w pierwszej kategorii nie jest automatycznym dowodem dwóch pozostałych”. Przywołaj debatę o Turingu, chińskim pokoju i funkcjonalizmie jako różne stanowiska, nie jako ostateczne rozstrzygnięcia. Unikaj stanowczego orzekania, że każdy obecny lub przyszły system AI na pewno ma albo na pewno nie ma subiektywnego doświadczenia; nie ma uzgodnionego testu takiego rozstrzygnięcia.

Rozwiń analogię lotu: samolot potrafi latać bez biologicznego mechanizmu ptasiego skrzydła. Możemy badać kompetencję niezależnie od materiału, z którego wykonano maszynę. Analogia ma jednak limit: w przypadku lotu dysponujemy precyzyjnymi wielkościami fizycznymi, a w przypadku „rozumienia” stosujemy niejednorodne kryteria.

**Głębsze dno.** Najciekawsze pytanie nie brzmi „czy model jest człowiekiem?”, ale „co trzeba by wykazać, aby uczciwie mówić o rozumieniu?”. Można mówić o rozumieniu operacyjnym: zdolności do poprawnego uogólniania, tworzenia spójnych modeli przyczynowych lub aktualizowania przekonań po kontrprzykładzie. Nie należy automatycznie utożsamiać tego z doświadczeniem wewnętrznym. Warto rozróżniać sukces testu, teorię mechanizmu i metafizyczne twierdzenie.

**Dyskusja.** „Czy zachowanie, którego przyczyny nie umiemy wytłumaczyć, może zasługiwać na zaufanie?” Pokaż różnicę między interpretowalnością a empiryczną walidacją.

### 12. 1943: neuron jako układ logiczny

**Scenariusz mówiony.** McCulloch i Pitts formalizowali ideę neuronu jako uproszczonej jednostki wykonującej operację logiczną na wejściach. Neuron może aktywować się, gdy odpowiednia kombinacja sygnałów spełnia warunek progowy. Proste elementy składają się w sieci wykonujące bardziej złożone obliczenia. Jest to fascynujący moment: do badania „procesów mózgowych” użyto języka logiki i obliczalności. Nie był to jeszcze system uczony gradientem ze współczesnych danych.

Wprowadź równanie intuicyjne: $z=\sum_i w_i x_i+b$, a następnie próg: aktywacja równa 1, gdy $z$ przekracza zadany poziom, inaczej 0. Dla dwóch binarnych wejść można zbudować logiczne AND. Pokaż przykład: dodatnie wagi obu wejść, próg wymagający ich jednoczesnej aktywności. Na późniejszych slajdach zastąpimy ostrą progową funkcję aktywacji funkcjami ułatwiającymi trening gradientowy.

**Głębsze dno.** To historyczne odkrycie ma znaczenie filozoficzne: zachowania przypominające obliczenie mogą wynikać z połączenia elementów lokalnie bardzo prostych. Złożoność nie musi znajdować się w jednym „centrum rozumowania”. Nie jest to jednak dowód, że formalny neuron odtwarza neurobiologię, ani że świadomość redukuje się do bramek logicznych. Formalizacja pokazuje możliwość pewnych obliczeń, nie pełnię biologicznego wyjaśnienia.

**Pytanie.** „Czy prostota komponentu wyklucza złożoność zachowania całego systemu?” Przygotuj przejście do sieci wielowarstwowych.

### 13. 1950: Alan Turing zmienia pytanie

**Scenariusz mówiony.** W artykule „Computing Machinery and Intelligence” Turing zaproponował zastąpienie trudnego do zdefiniowania pytania „czy maszyny myślą?” grą w naśladownictwo. W tej koncepcji badamy zachowanie widziane przez rozmówcę w określonych warunkach komunikacji. Zwróć uwagę, że późniejsza potoczna nazwa „test Turinga” przykrywa bardziej złożony oryginalny tekst i jego argumentację. Turing nie przedstawił laboratoryjnego miernika świadomości.

Powiedz: „To przesunięcie z wnętrza na zjawiska dostępne obserwacji było metodologicznie niezwykle skuteczne. Zadajemy pytanie, które można próbować testować, zamiast spierać się wyłącznie o znaczenie jednego słowa”. Współczesne systemy przechodzą rozmaite testy rozmowy, lecz wymagają także osobnych testów wiedzy, rozumowania, bezpieczeństwa, stabilności i skuteczności zadaniowej.

**Głębsze dno.** Test zachowania operacjonalizuje fragment inteligencji, ale w badaniu pojawia się ryzyko „ucieczki kryterium”: jeśli algorytm spełni test, zaczynamy uznawać go za zbyt łatwy. Z drugiej strony jeden test nie rozstrzyga filozofii umysłu. Sukces epistemologiczny polega nie na znalezieniu absolutnej definicji, lecz na zbudowaniu procedury, która dostarcza dowodów ograniczonych, ale sprawdzalnych.

**Pytanie.** „Czy zdolność przekonania człowieka, że rozmawia z człowiekiem, musi iść w parze z umiejętnością podejmowania bezpiecznych decyzji?” Odpowiedź prowadzi do wielowymiarowej ewaluacji.

### 14. 1956: Dartmouth i narodziny nazwy „AI”

**Scenariusz mówiony.** Propozycja warsztatów w Dartmouth została przygotowana w 1955 roku, a wydarzenie odbyło się latem 1956. John McCarthy wraz z innymi badaczami sformułował ambitny program: aspekty uczenia i inteligencji mają być na tyle precyzyjnie opisane, by można je symulować maszynowo. Powiedzenie „narodziny AI w 1956” oznacza więc raczej powstanie nazwy i programu badawczego niż początek wszelkiego myślenia o inteligentnych maszynach.

Przedstaw przełom intelektualny: uznano, że język, abstrakcja, rozwiązywanie problemów i twórczość mogą być tematem obliczeń. Wczesny optymizm był ogromny. Z czasem okazało się, że problemy łatwe dla człowieka, takie jak rozpoznawanie przedmiotu w nieidealnym świetle czy rozumienie kontekstu, nie redukują się do kilku jawnych reguł.

**Głębsze dno.** Dartmouth jest symbolem śmiałej hipotezy badawczej: w inteligencji istnieje część opisywalna formalnie. Z tego nie wynika, że cała inteligencja ma już formalną teorię. Historia nauki często zaczyna się od ambitnej deklaracji, po której następują dziesięciolecia precyzowania tego, co deklaracja naprawdę znaczy. Słowo „inteligencja” stało się obietnicą, ale również źródłem wygórowanych oczekiwań.

**Przejście.** „A teraz zobaczymy, jak model zainspirowany neuronem zaczął rzeczywiście dopasowywać swoje parametry”.

### 15. 1958–1986: perceptron, kryzys i powrót uczenia

**Scenariusz mówiony.** Frank Rosenblatt rozwijał perceptron jako prosty model uczący liniowej granicy decyzyjnej. Reguła aktualizacji wagi koryguje ją, gdy klasyfikacja jest błędna. Jeśli dane są liniowo separowalne, perceptron ma własności zbieżności przy odpowiednich warunkach. Klasycznym problemem jest XOR: cztery punkty, których etykiet nie da się oddzielić jedną linią w oryginalnej przestrzeni wejść. To nie oznacza, że „sieci neuronowe nie mogą nauczyć się XOR”; oznacza, że pojedyncza jednostka liniowa jest ograniczona.

Wielowarstwowe sieci pozwalają przekształcić reprezentację tak, aby dalsza warstwa rozdzieliła klasy. Backpropagation, spopularyzowana w latach 80. dzięki pracom Rumelharta, Hintona i Williamsa, umożliwiła wydajne wyznaczanie gradientów wielu warstw. Podkreśl precyzję historyczną: obliczanie pochodnych metodą wstecznego różniczkowania ma starsze korzenie; rok 1986 to ważny punkt upowszechnienia w sieciach, nie absolutny wynalazek całej idei.

**Głębsze dno.** Historia perceptronu pokazuje naukową wartość ograniczenia. Dowód, że model nie potrafi rozwiązać określonego zadania, nie unicestwia całej rodziny metod, lecz wskazuje, czego brakuje w architekturze lub reprezentacji. W ML „nie potrafi” zawsze znaczy „nie potrafi przy tych założeniach, tej reprezentacji i tej klasie funkcji”. Właśnie dlatego przed wyborem algorytmu badamy geometrię zadania.

**Pytanie.** „Czy rozwiązanie XOR wymaga więcej danych, czy zmiany klasy modelu?” Przy tym problemie kluczowa jest reprezentacja/nieliniowość, nie tylko liczebność zbioru.

### 16. Systemy eksperckie i zimy AI

**Scenariusz mówiony.** W latach 70. i 80. dużą rolę odegrały systemy eksperckie: baza wiedzy plus silnik wnioskowania. W wybranych dziedzinach, takich jak diagnostyka i konfiguracja, reguły typu IF–THEN okazywały się efektywne. Problem nie polegał na tym, że logika jest bezużyteczna. Problemem były koszty wydobycia wiedzy od ekspertów, utrzymania wyjątków, konfliktów reguł i zmian w rzeczywistym świecie. Im bardziej otwarta domena, tym trudniej opisać ją kompletnie ręcznie.

Pojęcie „zimy AI” odnosi się do okresów spadku finansowania i entuzjazmu po niespełnieniu nadmiernych prognoz; historia zna więcej niż jedną taką falę. Rozróżnij spadek oczekiwań od ustania badań. Nawet w kryzysie powstawały prace rozwijające statystykę, sieci, optymalizację i systemy wiedzy.

**Głębsze dno.** System ekspercki zmusza do pytania, czy wiedza istnieje jako skończona lista zdań. W wielu zadaniach jest częściowo jawna, częściowo nieformalna, kontekstowa, a czasem sprzeczna. Formalna ontologia porządkuje pojęcia, lecz nie gwarantuje pełnego pokrycia rzeczywistości. ML przesuwa wysiłek z ręcznego zapisywania wszystkich reguł na zbieranie danych i ocenę statystyczną. Nie usuwa problemu wiedzy; zmienia miejsce, w którym go napotykamy.

**Przykład.** Przepisy księgowe dają się częściowo opisać regułami. Wykrywanie nietypowych schematów nadużyć wymaga często analizy wzorców. Dobrze zaprojektowany system łączy oba podejścia.

### 17. 1997–2012: od wyszukiwania do głębokiego rozpoznawania

**Scenariusz mówiony.** W 1997 Deep Blue pokonał Garry'ego Kasparowa w meczu. Nie był prekursorem współczesnego chatbota; korzystał z zaawansowanego przeszukiwania pozycji szachowych, funkcji oceny i specjalizowanego sprzętu. Rok 2012 to odmienny przełom: AlexNet uzyskał bardzo dobry wynik w klasyfikacji obrazów ImageNet, pokazując praktyczną siłę głębokich sieci konwolucyjnych trenowanych na dużych danych przy użyciu GPU. Zwróć uwagę na różnicę: system szachowy eksploruje przestrzeń możliwych posunięć, CNN uczy się reprezentacji obrazu.

Wyjaśnij trzy składniki sukcesu uczenia głębokiego: architektura odpowiednia do struktury danych, duża liczba przykładów i moc obliczeniowa, plus techniki treningu. Rewolucja nie polegała na pojedynczym magicznym równaniu. Nastąpiło jednoczesne dojrzewanie kilku warunków.

**Głębsze dno.** Deep Blue i AlexNet ilustrują dwa różne znaczenia „inteligentnego rozwiązania”: wyszukiwanie w dobrze zdefiniowanej przestrzeni oraz statystyczne uogólnianie z obrazów. Ich sukces jest spektakularny, ale nie dowodzi posiadania ogólnej kompetencji życiowej. AI nie rozwija się według jednego uniwersalnego wskaźnika. Różne zadania wymagają różnych reprezentacji świata i odmiennych kryteriów sukcesu.

**Pytanie.** „Dlaczego nie rozwiązujemy rozpoznawania zdjęć, przeszukując wszystkie możliwe obrazy tak, jak ruchy szachowe?” Wprowadź problem przestrzeni kombinatorycznej i reprezentacji.

### 18. 2016–2017: AlphaGo i Transformer

**Scenariusz mówiony.** AlphaGo, znany z meczu z Lee Sedolem w 2016 roku, połączył kilka idei: sieci neuronowe szacujące ruchy i wartości pozycji, uczenie oraz wyszukiwanie Monte Carlo w drzewie. To ważny przykład, że model i search wzajemnie się wspierają: sieć podpowiada obiecujące kierunki, przeszukiwanie testuje konsekwencje. Następnie w 2017 roku publikacja „Attention Is All You Need” wprowadziła architekturę Transformera, opartą na mechanizmie uwagi zamiast dominującej wcześniej sekwencyjnej rekurencji.

Zarysuj intuition attention: token pyta inne tokeny o informację przydatną do aktualnej reprezentacji; powstają wagi zależne od kontekstu. Transformery umożliwiły efektywne równoległe trenowanie i rozwój modeli pracujących na ogromnych korpusach. Zaznacz, że model uwagi nie jest ludzkim aktem świadomości czy „zauważania”.

**Głębsze dno.** W AlphaGo inteligentne działanie jest wynikiem *architektury systemowej*: żadna pojedyncza część nie odpowiada za cały sukces. W Transformerze pojawia się zmiana w tym, jak model wyznacza istotność relacji. Otrzymujemy ważną lekcję: postęp AI nie musi oznaczać coraz wierniejszej imitacji mózgu; często polega na znalezieniu skuteczniejszej struktury obliczeń dla konkretnego zadania.

**Przejście.** „Teraz skala tych mechanizmów przechodzi z laboratoriów do powszechnego użycia”.

### 19. Od 2022: modele fundamentalne, multimodalność i agenci

**Scenariusz mówiony.** „Współczesna fala AI nie zaczęła całej dziedziny. Zmieniła jej dostępność i skalę zastosowań”. Wyjaśnij, czym jest model fundamentalny: model trenowany szeroko, możliwy do adaptacji do wielu zastosowań. Multimodalność oznacza łączenie różnych typów danych, np. tekstu, obrazu czy dźwięku. Agent to system, który może wykorzystywać model do planowania kroków i korzystania z narzędzi; jego rzeczywiste działanie zależy jednak od uprawnień, procedur i jakości integracji.

Podaj kontrast: chatbot generujący poradę ma inne ryzyko niż agent, który samodzielnie wysyła wiadomości lub dokonuje zmian w bazie. Tam, gdzie odpowiedź przechodzi w działanie, rośnie znaczenie granic uprawnień, kontroli stanu, testowania, audytu i możliwości przerwania procesu.

**Głębsze dno.** Wzrost skali modelu nie usuwa problemu prawdy. Model językowy uczy się zależności statystycznych na ogromnej liczbie przykładów, ale nie ma automatycznie gwarancji zgodności odpowiedzi z bieżącym światem. Dodatkowo „inteligencja systemu” nie jest wyłącznie własnością wag. Powstaje ze sprzężenia modelu, danych, narzędzi, pamięci roboczej, kontroli i ludzi. Im większa sprawczość systemu, tym istotniejsza staje się architektura odpowiedzialności.

**Pytanie.** „Co jest bardziej niebezpieczne: model, który raz się myli, czy agent, który ten błąd automatycznie realizuje w pięciu systemach?”

### 20. 80 lat AI: historia zmieniających się metod

**Scenariusz mówiony.** Przejdź przez oś czasu nie jako katalog dat, lecz jako historię kolejnych odpowiedzi na tę samą ambicję. 1943: formalny neuron; 1950: operacjonalizacja zachowania; 1956: wspólna nazwa projektu; 1958: ucząca się liniowa jednostka; 1986: praktyczne uczenie sieci wielowarstwowych; 1997: wyszukiwanie pokonujące mistrza szachowego; 2012: reprezentacje obrazowe; 2016: połączenie sieci i search; 2017: attention; od 2022: masowe użycie modeli generatywnych; 2026: silne zainteresowanie systemami agentowymi. Ostatni punkt traktuj jako obraz trendu wdrożeniowego, nie jako jednorazowy naukowy „wynalazek roku”.

Porównaj problem z każdej epoki. Czy trudność była w obliczeniu ruchu, opisaniu reguł, znalezieniu cech, treningu wielkiej sieci, czy w bezpiecznej integracji wyniku z działaniem? Pokaż ciągłość: stare metody nie znikają, bo często są bardziej adekwatne do danych i kosztu.

**Głębsze dno.** Oś czasu nie przedstawia ewolucji „stopnia świadomości” maszyn. Przedstawia rosnące możliwości rozwiązywania problemów i zmieniające się paradygmaty reprezentacji. Historia AI jest także historią definicji sukcesu. Problem, który w jednej dekadzie nazywano inteligencją, w kolejnej mógł stać się zwykłym elementem oprogramowania. To ważne ostrzeżenie przed utożsamianiem jednego benchmarku z definicją inteligencji.

**Przejście.** „Jakie pięć lekcji daje nam ta droga dla codziennej pracy z modelami?”.

### 21. Pięć lekcji historii AI

**Scenariusz mówiony.** Omów pięć lekcji z konkretnymi konsekwencjami. Po pierwsze, sukces w jednej domenie nie oznacza sprawności uniwersalnej: szachy, język, medycyna i planowanie to różne rodziny zadań. Po drugie, reprezentacja problemu potrafi być ważniejsza niż drobna różnica algorytmiczna. Po trzecie, dane, architektura i moc obliczeniowa rozwijają się razem. Po czwarte, hybrydy łączą mocne strony reguł i modeli uczonych. Po piąte, test w rzeczywistym użyciu jest równie istotny, jak wynik laboratoryjny.

Rozwiń przykład: model trenowany do oceny ryzyka w jednym banku może zawodzić w innej populacji, mimo że wykorzystuje identyczny algorytm. Problemem jest nie tylko „parametr”, ale zmiana warunków i znaczenia danych. Zachęć do myślenia o wdrożeniu jako eksperymencie rozciągniętym w czasie.

**Głębsze dno.** Historia nie prowadzi do wniosku „coraz większy model jest zawsze lepszy”. Prowadzi do bardziej niewygodnego pytania: jaka wiedza jest konieczna, by uzasadnić konkretną decyzję? W AI nie wystarcza zdolność do obliczenia odpowiedzi; liczy się także zakres jej prawomocności. Model matematyczny ma domenę zastosowania, granice założeń i koszt błędu. Dojrzałość AI zaczyna się od umiejętności powiedzenia: „ten wynik jest użyteczny tutaj, ale nie został dowiedziony poza tym przypadkiem”.

**Zamknięcie bloku.** „Skoro wiemy, dlaczego powstały różne typy AI, przejdźmy od historii do mechanizmu: co naprawdę oznacza, że maszyna się uczy?”.


## BLOK II. JAK MASZYNA SIĘ UCZY

### 22. Jak maszyna się uczy: otwarcie modułu

**Scenariusz mówiony.** „W języku potocznym nauka oznacza zrozumienie sensu. W uczeniu maszynowym ma definicję techniczną: algorytm zmienia parametry lub strukturę na podstawie danych lub informacji zwrotnej, aby poprawić określone kryterium”. Zacznij od przykładu: mamy dane o opóźnieniach przesyłek, ale nie znamy prostej reguły ich występowania. Budujemy model zależności między cechami zamówienia a opóźnieniem. W treningu algorytm ustala parametry. Prawdziwe wyzwanie zaczyna się dopiero wtedy, gdy pojawia się nowa przesyłka.

Zarysuj proces: zjawisko w świecie → sposób pomiaru → zbiór danych → hipoteza/model → funkcja straty → optymalizacja → walidacja → użycie. Przy każdym przejściu możliwy jest błąd. Nawet doskonała optymalizacja nie naprawi źle sformułowanego celu ani wadliwego pomiaru.

**Głębsze dno.** Uczenie nie jest „wchłanianiem świata”. Jest selektywnym dopasowaniem funkcji do dostępnego doświadczenia. To fundamentalne ograniczenie epistemiczne. Model uczy się tego, co da się wywnioskować z podanych danych przy danej architekturze i funkcji celu. Nie ma magicznego dostępu do faktów, których nie zakodowaliśmy lub których nie da się odzyskać statystycznie.

**Pytanie.** „Czy model może nauczyć się przyczyn opóźnień, jeśli widzi jedynie korelacje między typem przesyłki a wynikiem?” Zapowiedz rozróżnienie predykcji i wnioskowania przyczynowego.

### 23. Uczenie nie oznacza zapamiętywania odpowiedzi

**Scenariusz mówiony.** Rozróżnij interpolację i ekstrapolację. Interpolacja polega na wnioskowaniu między znanymi przykładami lub w ich podobnym sąsiedztwie. Ekstrapolacja dotyczy sytuacji wykraczających poza zakres treningu, zwykle trudniejszych. Jeśli model zapamięta tabelę identyfikatorów i etykiet, może osiągnąć 100% trafności na treningu, ale niczego sensownie nie przewidywać dla nowych identyfikatorów. Uczenie użytecznej reguły wymaga odkrycia stabilnej zależności, a nie tylko kompresji konkretnych odpowiedzi.

Użyj pojęcia funkcji hipotezy: $f_\theta(x)$. Dane ograniczają dopuszczalne wartości parametrów $\theta$, a algorytm szuka dopasowania. Generalizacja oznacza niski oczekiwany błąd na danych pochodzących z odpowiednio podobnego procesu, którego nie wykorzystano do strojenia. Zwróć uwagę, że także bardzo dobry model może częściowo zapamiętywać przykłady; istotne jest, czy to zjawisko prowadzi do zawodności poza treningiem i ewentualnie do ujawniania danych.

**Głębsze dno.** W centrum ML stoi problem indukcji: z ograniczonej liczby obserwacji chcemy wyciągnąć wniosek o przyszłości. Żaden skończony zbiór danych nie dowodzi, że reguła zadziała zawsze. Pomagają założenia o podobieństwie świata w czasie, strukturze danych i ograniczeniu złożoności modelu. Zaufanie do modelu jest więc uzasadnionym empirycznie oszacowaniem, nie logiczną pewnością.

**Pytanie.** „Czy jeden kontrprzykład obala model?” Nie zawsze; obala twierdzenie o bezwyjątkowości, ale jakość predykcji jest zwykle probabilistyczna.

### 24. Nadzorowane, nienadzorowane i uczenie ze wzmocnieniem

**Scenariusz mówiony.** W uczeniu nadzorowanym obserwujemy pary $(x,y)$. Przykład: cechy transakcji i informacja, czy była oszustwem. W nienadzorowanym mamy głównie $x$ i szukamy struktury: klastrów, kierunków zmienności, rozkładu. W uczeniu ze wzmocnieniem agent podejmuje akcje, otrzymuje nagrody i uczy się polityki maksymalizującej długoterminowy zwrot. W self-supervised learning zadanie treningowe tworzy się z danych samych w sobie, np. przewidując brakujący fragment sygnału lub kolejny token.

Wyraźnie odróżnij „brak etykiet” od „braku celu”. k-means minimalizuje określony błąd wewnątrz klastrów, chociaż nie zna gotowych klas. W RL nagroda nie musi być natychmiastowa; istnieje problem przypisania zasługi wielu wcześniejszym działaniom. W self-supervised model zna sygnał treningowy, choć nikt ręcznie nie opisuje go nazwami kategorii.

**Głębsze dno.** Typ uczenia mówi, *jakie źródło normy* dostaje model. Nadzór: wzorcowa odpowiedź. Nienadzór: kryterium struktury. RL: wartość konsekwencji działań. Self-supervision: przewidywalność lub spójność struktury danych. Ten sam system może łączyć te formy. Co ważne, nagroda nie jest moralnym dobrem, a etykieta nie jest automatycznie prawdą. To tylko sygnały, które przyjęliśmy za cel optymalizacji.

**Pytanie.** „Jeżeli bot uczy się maksymalizować czas spędzony w aplikacji, czy uczy się dobrostanu użytkownika?” To przykład błędnej specyfikacji nagrody.

### 25. Reprezentacja cech określa, czego model może się nauczyć

**Scenariusz mówiony.** Zacznij od dwóch obserwacji opisanych tylko surowymi identyfikatorami. Algorytm nie ma podstaw, by uznać je za podobne. Dodaj cechy opisujące kontekst, częstotliwość i czas, a zależność może stać się widoczna. Reprezentacja $\phi(x)$ zamienia obiekt świata na wektor lub strukturę używaną przez model. Istotne jest, by zachować informacje potrzebne do zadania, a ograniczyć te przypadkowe lub niedostępne podczas rzeczywistej predykcji.

Pokaż matematyczny trik: w danych wejściowych punkty mogą być nieliniowo separowalne, ale po transformacji, np. dodaniu cechy $x_1x_2$, rozdzielenie staje się łatwiejsze. Modele liniowe mogą stać się skuteczne po przekształceniu cech; sieci neuronowe uczą takich przekształceń przez warstwy. Nie oznacza to automatycznie, że nauczone cechy są semantycznie zrozumiałe.

**Głębsze dno.** Reprezentacja to ukryte założenie ontologiczne projektu. Kiedy mówię, że klient jest wektorem: wiek, liczba transakcji, średnia wartość koszyka, tworzę jedynie określony *opis* klienta. Pomijam jego motywacje, sytuację życiową, zamiar czy przyczyny działania. Algorytm nie „widzi człowieka”; widzi opis zbudowany dla zadania. Dlatego jakość pomiaru i sens cech są równie istotne, jak zdolność optymalizacji.

**Przykład.** Dwa miasta mają tę samą średnią temperaturę roczną, lecz zupełnie inny rozkład sezonowy. Jedna liczba nie zachowuje struktury potrzebnej do prognozowania zapotrzebowania na ogrzewanie.

### 26. Trening, walidacja, test: trzy role danych

**Scenariusz mówiony.** „Model widzi trening, projektant korzysta z walidacji, a test powinien sprawdzać obietnicę złożoną przed wdrożeniem”. W treningu dopasowujemy parametry. Na walidacji wybieramy modele, hiperparametry, transformacje i progi. Test odkładamy na końcową niezależną ocenę. Jeśli wielokrotnie zaglądamy do testu i poprawiamy decyzje, test de facto zamienia się w kolejny zbiór walidacyjny.

Wyjaśnij szczególne przypadki. W danych czasowych trenujemy na przeszłości, walidujemy na późniejszym okresie i testujemy na jeszcze późniejszym. Przy danych wielu pacjentów lub klientów unikamy obecności tej samej osoby w obu podzbiorach, jeśli wdrożenie ma przewidywać nowych ludzi. Gdy danych jest mało, stosuje się walidację krzyżową, ale trzeba zachować strukturę grup i czasów.

**Głębsze dno.** Test jest próbą odtworzenia sytuacji epistemicznej: model dostaje przypadek, o którym jeszcze nie wie. W praktyce test jest tylko przybliżeniem przyszłości, a nie gwarancją. Rozkład może się zmienić. Dlatego wynik 95% na danych historycznych nie jest niezmienną właściwością algorytmu; jest oszacowaniem w określonym protokole pomiarowym.

**Pytanie.** „Czy uczciwy test może wypaść słabo, mimo bardzo dobrego modelu?” Tak, przy trudnym przesunięciu rozkładu lub przy małej próbie i dużej niepewności estymacji.

### 27. Funkcja straty: jak model wie, że się pomylił?

**Scenariusz mówiony.** „Model nie ma poczucia porażki. Mamy funkcję, która zamienia rozbieżność między przewidywaniem a celem na liczbę”. Dla regresji można zdefiniować $L=\frac1n\sum (y_i-\hat y_i)^2$; kwadrat silniej karze duże pomyłki. Dla klasyfikacji prawdopodobieństw stosujemy cross-entropy, która dotkliwie karze nadmierną pewność co do błędnej klasy. Strata treningowa jest sposobem sterowania uczeniem, a metryka biznesowa może uwzględniać zupełnie inne konsekwencje.

Rozróżnij minimalizację ryzyka empirycznego od oczekiwanego: trenujemy na skończonej próbie, a chcemy dobrego wyniku na rozkładzie przyszłych obserwacji. Regularizacja dodaje karę za złożoność: $L_{total}=L_{data}+\lambda\Omega(\theta)$. Nie chodzi o moralne karanie „zbyt dużych” wag, lecz o narzucenie preferencji dla określonej rodziny rozwiązań.

**Głębsze dno.** Funkcja straty jest zapisanym matematycznie wyborem wartości. Jeśli mierzymy wyłącznie trafność, możemy ignorować asymetrię kosztu błędów. Jeśli premiujemy wyłącznie zaangażowanie, możemy uczyć system zachowań niepożądanych społecznie. Znane powiedzenie o prawie Goodharta przypomina: kiedy wskaźnik staje się jedynym celem, może przestać dobrze reprezentować pierwotną intencję. Model perfekcyjnie optymalizuje to, co zdefiniowaliśmy, nie to, co przemilczeliśmy.

**Pytanie.** „Czy funkcja straty musi być równa temu, na czym naprawdę zależy organizacji?” Nie; ale rozbieżność powinna być świadoma i mierzona.

### 28. Niedouczenie i przeuczenie

**Scenariusz mówiony.** Wyjaśnij niedouczenie jako model zbyt ubogi lub niedostatecznie nauczony, by uchwycić ważne prawidłowości. Przeuczenie występuje, gdy model dopasowuje również przypadkowe fluktuacje treningu, pogarszając wynik na nowych danych. Na wykresie błąd treningowy może stale spadać, podczas gdy walidacyjny najpierw maleje, a potem rośnie. Nie każde odejście od monotoniczności musi wyglądać identycznie w rzeczywistych dużych sieciach, ale schemat uczy właściwego pytania.

Połącz problem ze złożonością modelu. Drzewo o dwóch podziałach może nie uchwycić skomplikowanej granicy, a drzewo o tysiącach liści zapamięta wyjątki. Regularyzacja, ograniczenie głębokości, dobór danych i wcześniejsze zatrzymanie treningu pomagają, ale nie istnieje jeden niezawodny przepis. Rozróżnij wariancję modelu od wariancji estymacji metryki na małym zbiorze.

**Głębsze dno.** To konflikt między pamięcią o przeszłości a zdolnością do działania w przyszłości. Naukowo odpowiada problemowi odróżnienia stabilnej regularności od przypadku. Dobry model nie musi wyjaśniać każdego punktu treningowego; ma dobrze działać w warunkach, dla których go zaprojektowano. Zbyt mocny model bywa paradoksalnie słaby, jeśli nauczył się historii, zamiast relacji o trwałym znaczeniu.

**Pytanie.** „Co oznacza 100% accuracy na danych treningowych?” Samo w sobie niemal nic o generalizacji.

### 29. Data leakage: błąd, który wygląda jak sukces

**Scenariusz mówiony.** „Wyciek danych to sytuacja, gdy model otrzymuje podczas uczenia lub ewaluacji informację, której nie powinien mieć w chwili prawdziwej predykcji”. Przykład: przewidujemy niewypłacalność na dzień składania wniosku, lecz w zbiorze pojawia się zmienna „liczba dni windykacji”, możliwa do poznania dopiero później. Wynik staje się imponujący, ponieważ model dostaje odpowiedź ukrytą w cechach.

Przeanalizuj inne formy: ta sama osoba w treningu i teście, powtarzające się zdjęcia tego samego obiektu, normalizacja lub selekcja cech liczona na całym zbiorze przed podziałem, tunowanie hiperparametrów na teście. Lekarstwem jest projektowanie walidacji zgodnie z rzeczywistą linią czasu i jednostką decyzji. Przy pytaniu o przyszłość nie możemy pozwolić modelowi zaglądać do przyszłych informacji.

**Głębsze dno.** Data leakage to nie tylko błąd techniczny. To błąd logiczny w konstrukcji dowodu. Twierdzimy, że algorytm odkrył regułę przewidywania, podczas gdy zaaranżowaliśmy sytuację, w której przewidywanie nie było potrzebne. Prawdziwa metodologia AI wymaga uczciwego odtworzenia granic wiedzy systemu w momencie decyzji. To ten sam rygor, który odróżnia eksperyment od iluzji eksperymentu.

**Pytanie.** „Czy zmienna powstała po zdarzeniu może się znaleźć w raporcie analitycznym?” Tak, ale nie jako predyktor zdarzenia ocenianego wcześniej.

## BLOK III. ALGORYTMY MACHINE LEARNING

### 30. Algorytmy Machine Learning: otwarcie modułu

**Scenariusz mówiony.** „Teraz otwieramy skrzynkę narzędziową, ale nie będziemy robić katalogu nazw. Każdy algorytm odpowiada na inne pytanie o geometrię danych, sposób reprezentacji i rodzaj błędu”. Podaj strukturę porównania: jakie zadanie? Jak wygląda rodzina funkcji? Co jest uczone? Jaka funkcja celu? Co trzeba założyć? Kiedy algorytm zawiedzie? Wróć do pięciu pytań ze slajdu 4.

Zarysuj dwa bieguny. Metody parametryczne narzucają często zwartą strukturę modelu, np. liniową zależność. Metody bardziej elastyczne, jak drzewa czy zespoły drzew, uczą skomplikowanych granic bez ręcznego zapisywania wzoru. Nie znaczy to, że elastyczny model jest zawsze lepszy: różnią się koszt, interpretowalność, wymagania danych i odporność na zmianę rozkładu.

**Głębsze dno.** Wybór algorytmu to wybór *hipotez o świecie*. Regresja liniowa zakłada przydatność struktury addytywnej po przekształceniach. kNN zakłada, że bliskie obiekty mają podobne odpowiedzi. Drzewo zakłada użyteczność progowych podziałów. SVM operuje marginesem, a klastry odpowiednią geometrią podobieństwa. Algorytm nie zastępuje myślenia; formalizuje jego określony fragment.

**Przejście.** „Zacznijmy od tego, jaki rodzaj wyniku w ogóle chcemy uzyskać”.

### 31. Mapa klasycznego Machine Learning

**Scenariusz mówiony.** Uporządkuj zadania. W regresji przewidujemy wielkość liczbową: czas dostawy lub wartość zużycia energii. W klasyfikacji przewidujemy klasę bądź jej prawdopodobieństwo: awaria/bez awarii. W klasteryzacji nie mamy gotowej odpowiedzi; chcemy odkryć grupy według wybranej miary podobieństwa. Redukcja wymiarowości zmienia opis obiektów, zachowując część informacji. Detekcja anomalii szuka przykładów nietypowych względem modelu normalności.

Ważne jest, że ten sam zbiór danych można analizować różnymi metodami, ale rezultaty oznaczają coś innego. Klaster danych transakcyjnych nie staje się automatycznie kategorią „oszustwo”. PCA nie jest klasyfikatorem. Wynik regresji może wymagać dalszego progu, jeśli chcemy podjąć decyzję operacyjną.

**Głębsze dno.** Przydział zadania determinuje rodzaj odpowiedzialności za błąd. Regresja mierzy odchylenie wartości, klasyfikacja rozkład pomyłek, klasteryzacja sens przyjętej geometrii, a anomalia niejednoznaczność rzadkości. Nie da się uczciwie porównywać metod, które nie rozwiązują tej samej definicji problemu. Najpierw trzeba nazwać obiekt analizy i decyzję, którą wynik ma wspierać.

**Pytanie.** „Czy do wykrycia oszustwa lepsza jest klasyfikacja czy wykrywanie anomalii?” To zależy od jakości i liczby etykiet oraz charakteru nowych oszustw.

### 32. Regresja liniowa: najprostszy model zaskakująco daleko sięga

**Scenariusz mówiony.** Zapisz $\hat y=\beta_0+\beta_1x_1+\dots+\beta_px_p$. W najprostszym ujęciu współczynnik $\beta_j$ opisuje zmianę przewidywanej wartości po jednostkowym wzroście $x_j$ przy pozostałych cechach utrzymanych na stałym poziomie. Model dopasowuje parametry, często minimalizując sumę kwadratów odchyleń. Pokaż na prostym przykładzie kosztu energii: prognoza jako funkcja temperatury zewnętrznej, powierzchni budynku i sposobu użytkowania.

Wymień ograniczenia i pułapki: zależność może być nieliniowa, wpływy mogą się zmieniać w czasie, obserwacje mogą być odstające, a cechy silnie skorelowane. Nie mów jednak, że regresja liniowa nie potrafi modelować nieliniowości: po dodaniu odpowiednich transformacji cech, np. $x^2$ i interakcji, pozostaje liniowa w parametrach, a jest nieliniowa w oryginalnym wejściu.

**Głębsze dno.** Współczynnik nie jest automatycznie przyczyną. Jeśli większa sprzedaż współwystępuje z większym wydatkiem reklamowym, nie oznacza to, że cały współczynnik jest efektem reklamy. Potrzebne są założenia lub odrębne metody przyczynowe. Interpretowalność modelu matematycznego oznacza, że potrafimy opisać jego rachunek, nie że rozstrzygnęliśmy strukturę przyczyn świata.

**Pytanie.** „Czy niski błąd regresji znaczy, że poznaliśmy przyczyny zjawiska?” Nie, może świadczyć wyłącznie o użytecznej zależności predykcyjnej.

### 33. Regresja logistyczna: prawdopodobieństwo zamiast etykiety

**Scenariusz mówiony.** Nazwa bywa myląca: w typowym zastosowaniu regresja logistyczna służy do klasyfikacji binarnej. Oblicza $z=w^Tx+b$, następnie $p=\sigma(z)=1/(1+e^{-z})$. Wynik od 0 do 1 interpretujemy jako modelową ocenę prawdopodobieństwa klasy dodatniej pod odpowiednimi założeniami. Próg, np. 0,5, nie jest święty; może zależeć od kosztów błędów. Dla $p=0{,}3$ model nie mówi „klasa to 0 z pewnością”, tylko podaje wynik użyteczny do decyzji progowej.

Podaj prosty przykład: przy ryzyku niewypłacalności zaniechanie interwencji może kosztować więcej niż fałszywy alarm. Zamiast maksymalizować samą accuracy, dobieramy próg z uwzględnieniem skutków. Log-loss penalizuje nadmiernie pewne błędne prognozy. Powiedz też o kalibracji: nawet gdy model porządkuje przypadki dobrze, jego prawdopodobieństwa mogą wymagać sprawdzenia.

**Głębsze dno.** Model klasyfikacyjny i decyzja etyczna to różne poziomy. Wartość $p$ jest wynikiem oszacowania warunkowego na określonych danych i cechach, a nie moralną oceną osoby. Dwa identyczne prawdopodobieństwa mogą prowadzić do różnych działań w zależności od kontekstu, prawa, ryzyka i dostępności interwencji.

**Pytanie.** „Czy osoba z 80% szacowanym ryzykiem musi automatycznie otrzymać odmowę?” Nie; decyzja wymaga jawnej, uzasadnionej polityki działania.

### 34. k-nearest neighbors: decyzja na podstawie otoczenia

**Scenariusz mówiony.** „kNN ma niemal dziecięcą intuicję: podobni do siebie często zachowują się podobnie”. Dla nowej obserwacji znajdujemy $k$ najbliższych punktów w przestrzeni cech. W klasyfikacji decyduje głosowanie lub ważone sąsiedztwo, w regresji średnia lub ważona średnia wartości. Tu nie trenujemy klasycznej globalnej funkcji o niewielkiej liczbie parametrów; znaczną część pracy wykonuje się przy predykcji, porównując przypadek z zapisanymi przykładami.

Pokaż, dlaczego jednostki zmieniają wynik: odległość dla cechy mierzonej w tysiącach może zdominować cechę w skali 0–1. Standaryzacja ma znaczenie. W wysokich wymiarach odległości mogą tracić zdolność wyraźnego odróżniania bliskich i dalekich punktów; to fragment „przekleństwa wymiarowości”. Małe $k$ zwiększa wrażliwość na szum, duże $k$ wygładza granicę kosztem szczegółów.

**Głębsze dno.** kNN pokazuje, że „podobieństwo” nie istnieje bez definicji. Podobny klient pod względem wieku może być zupełnie inny pod względem zachowania zakupowego. Wybrana metryka tworzy lokalną ontologię sąsiedztwa: decyduje, które różnice traktujemy jako istotne. Dla danych ludzi ten pozornie techniczny wybór może mieć konsekwencje społeczne.

**Pytanie.** „Czy dwa przypadki podobne w czterdziestu cechach są na pewno podobne pod względem ryzyka?” Nie, może brakować kluczowej zmiennej.

### 35. Drzewo decyzyjne: przestrzeń cięta pytaniami

**Scenariusz mówiony.** Pokaż drzewo jako sekwencję prostych pytań: „czy liczba reklamacji > 2?”, „czy średnia wartość zakupu < 100?”. W każdym węźle algorytm szuka podziału, który poprawia jednorodność podzbiorów. W klasyfikacji służy temu np. indeks Giniego lub entropia; w regresji redukcja wariancji i błędu. Liść zwraca klasę, prawdopodobieństwo szacowane z próbek lub wartość liczbową.

Wyjaśnij, że drzewo łatwo wizualizować, ale głębokie drzewa stają się niestabilne: mała zmiana próby może prowadzić do innego zestawu podziałów. Podziały osiowe są lokalnie proste, lecz potrafią tworzyć złożone granice. Ograniczenie głębokości, minimalna liczba obserwacji w liściu i przycinanie wpływają na generalizację.

**Głębsze dno.** Drzewo kusi pozorem przyczynowości: wygląda jak logiczny tok rozumowania. W rzeczywistości podział jest zwykle wybierany pod poprawę statystycznego kryterium w danych, nie pod dowód przyczynowy. To, że ścieżka brzmi „jeżeli A, to B”, nie znaczy, że A wywołuje B. Drzewo wyjaśnia rachunek klasyfikatora, a niekoniecznie naturę zjawiska.

**Pytanie.** „Czy wyjaśnialność struktury drzewa gwarantuje uczciwość decyzji?” Nie; znaczenie mają również dane, cechy i konsekwencje.

### 36. Random Forest: wiele drzew, stabilniejszy wynik

**Scenariusz mówiony.** „Pojedyncze drzewo jest łatwe do przeczytania, ale bywa nerwowe. Las buduje wiele zróżnicowanych drzew i agreguje ich przewidywania”. Każde drzewo uczy się na próbce bootstrapowej danych, a przy wyborze podziałów zwykle rozpatruje losowy podzbiór cech. Te dwie formy losowości pomagają zmniejszać korelację błędów drzew. W klasyfikacji stosujemy głosowanie lub uśrednianie prognoz, w regresji średnią.

Wyjaśnij mechanizm redukcji wariancji: uśrednianie działa najlepiej, gdy błędy poszczególnych modeli nie są doskonale skorelowane. Las potrafi modelować interakcje i nieliniowości bez jawnego zapisywania wszystkich zależności. Ograniczeniem jest większy koszt obliczeń, mniejsza przejrzystość pojedynczej decyzji i możliwa słabość ekstrapolacji poza zakres obserwowany w treningu.

**Głębsze dno.** Random Forest jest matematycznym przykładem zbiorowej odporności: wiele niedoskonałych perspektyw, odpowiednio zróżnicowanych, może dać stabilniejszy wynik niż jedna. Ale agregacja nie znosi wspólnego błędu systematycznego: jeśli wszystkie drzewa uczą się z tych samych stronniczych danych, las nie stworzy brakującej prawdy. Wariancję można zredukować; biasu wynikającego z błędnej definicji celu nie usunie głosowanie.

**Pytanie.** „Czy tysiąc błędnych modeli zawsze daje lepszy wynik niż jeden?” Nie; decyduje charakter błędów i ich zależność.

### 37. Gradient Boosting: modele korygują wcześniejsze błędy

**Scenariusz mówiony.** Boosting buduje model addytywny etapami: $F_M(x)=F_0(x)+\sum_{m=1}^{M}\eta h_m(x)$. Każdy kolejny słaby model przybliża kierunek, w którym trzeba poprawić dotychczasową predykcję. Dla straty kwadratowej intuicja jest szczególnie prosta: nowy model może uczyć się reszt, czyli różnic między prawdziwą wartością a aktualną prognozą. W innych funkcjach straty używa się pseudo-reszt związanych z ujemnym gradientem.

Odwołaj się do różnicy Random Forest kontra boosting. Las uczy drzewa w dużym stopniu równolegle i uśrednia; boosting buduje kolejne korekty sekwencyjnie. Hyperparametry takie jak liczba etapów, głębokość drzew i learning rate sterują kompromisem jakości, kosztu i przeuczenia. Nie stawiaj ogólnej tezy, że boosting zawsze wygrywa: zależy to od danych i protokołu walidacji.

**Głębsze dno.** Boosting pokazuje uczenie jako proces poprawek, a nie jednorazowe odkrycie „prawdziwej” funkcji. Każdy nowy model powstaje w odniesieniu do ograniczeń poprzedniego. To ważna intuicja całej optymalizacji iteracyjnej: rozwijamy przybliżenie przez lokalne korekty mierzone funkcją celu. Jeśli cel jest niewłaściwy, postęp obliczeniowy może tylko lepiej realizować niewłaściwy zamiar.

**Pytanie.** „Co się stanie, jeśli kolejne drzewa zaczną korygować szum zamiast stabilnych zależności?” Pojawi się przeuczenie.

### 38. SVM: granica z największym marginesem

**Scenariusz mówiony.** „Nie szukamy po prostu dowolnej linii oddzielającej klasy. Szukamy takiej, która zostawia możliwie duży margines bezpieczeństwa”. Dla liniowego przypadku separator ma postać $w^Tx+b=0$. Przy twardym marginesie, dla liniowo separowalnych danych, dążymy do minimalizacji $\|w\|^2$ przy odpowiednich ograniczeniach klas. Dla danych rzeczywistych soft margin dopuszcza naruszenia poprzez zmienne luzu i karę kontrolowaną parametrem $C$.

Wyjaśnij wektory nośne: wybrane próbki blisko granicy szczególnie wpływają na jej położenie. Kernel trick pozwala obliczać podobieństwa tak, jakbyśmy pracowali w bogatszej przestrzeni cech, bez jawnego tworzenia wszystkich jej współrzędnych. SVM bywa wrażliwy na skalę cech i parametry kernela, a trening przy bardzo dużych danych może być kosztowny.

**Głębsze dno.** Margines jest formalną wersją idei odporności na niewielkie zakłócenia wejścia. Nie wystarczy podzielić przykłady; dobrze, jeśli separator nie leży niepotrzebnie blisko nich. Ale duży margines w dobranej geometrii nie gwarantuje odporności na przesunięcie świata. Wybrana przestrzeń cech i kernel decydują, czym jest „bliskość”. Geometria modelu to również hipoteza o zadaniu.

**Pytanie.** „Czy perfekcyjne rozdzielenie treningu jest ważniejsze niż szeroki, rozsądny margines?” Zwykle nie.

### 39. k-means: grupowanie przez centroidy

**Scenariusz mówiony.** „W k-means nie pytamy, do jakiej znanej klasy należy obiekt. Chcemy podzielić obserwacje na $k$ grup, które są wewnętrznie względnie spójne według odległości”. Algorytm naprzemiennie przypisuje punkty do najbliższego centroidu i przelicza centroid jako średnią grupy. Minimalizuje sumę kwadratów odległości od centrów, choć iteracyjny algorytm może zatrzymać się w optimum lokalnym. Dlatego inicjalizacja, często k-means++, ma znaczenie.

Zwróć uwagę na typowe założenia: reprezentacja numeryczna, sensowna skala cech, klastery raczej zwarte i podobne pod względem geometrii. Grupowanie może się zmieniać wraz z wyborem $k$. „Ładny” rysunek klastrów nie dowodzi istnienia naturalnych typów ludzi czy klientów.

**Głębsze dno.** Klaster to rezultat przyjętej miary podobieństwa i kryterium optymalizacji, a nie odkryta esencja obiektu. Segmentację klientów można tworzyć ze względu na częstotliwość zakupu, wartość lub reakcję na ofertę; powstaną różne podziały. Zjawisko nie posiada koniecznie jednej „prawdziwej” klasyfikacji. To przypomnienie, że wiele struktur w ML zależy od celu badacza.

**Pytanie.** „Jeśli algorytm znajduje trzy grupy, czy oznacza to, że świat obiektywnie dzieli się na trzy rodzaje obiektów?” Nie.

### 40. DBSCAN: klastry jako obszary zagęszczenia

**Scenariusz mówiony.** DBSCAN odpowiada na problem, w którym grupy mogą mieć nieregularne kształty. Ustalamy promień sąsiedztwa $\varepsilon$ i wymaganą liczbę obserwacji w sąsiedztwie, `min_samples`. Punkty rdzeniowe mają dostatecznie gęste otoczenie. Z punktów rdzeniowych budujemy obszary połączone przez gęstość; niektóre obserwacje pozostają szumem. Nie trzeba wskazywać liczby klastrów z góry.

Pokaż przykład dwóch koncentrycznych pierścieni: k-means może je przeciąć nieintuicyjnie, DBSCAN potrafi odzyskać zakrzywione struktury. Potem pokaż trudność: różne gęstości w tym samym zbiorze oraz źle dobrana metryka sprawiają, że jedna wartość $\varepsilon$ nie wystarcza. Wysokie wymiary również komplikują pojęcie lokalnego zagęszczenia.

**Głębsze dno.** To, czy punkt nazwany zostanie „szumem”, zależy od definicji normalnego sąsiedztwa. Szum algorytmiczny nie znaczy błąd, zagrożenie ani bezużyteczność. W badaniu rzadkich sytuacji właśnie takie punkty mogą być najciekawsze. Warto pytać, czy zadaniem jest odkrycie głównej struktury populacji, czy ochrona wyjątków przed zignorowaniem.

**Pytanie.** „Czy obserwację oznaczoną jako szum należy usunąć?” Nie bez sprawdzenia jej znaczenia domenowego.

### 41. PCA: mniej wymiarów, zachowana wariancja

**Scenariusz mówiony.** PCA konstruuje nowe, wzajemnie prostopadłe osie, które wyjaśniają kolejne największe części wariancji danych. W klasycznym podejściu centrujemy dane, często decydujemy też o skalowaniu cech, a następnie analizujemy kierunki własne macierzy kowariancji lub równoważnie rozkład SVD. Pierwsza składowa jest kierunkiem największego rozproszenia, druga największego spośród kierunków do niej prostopadłych, itd.

Wyjaśnij zastosowania: wizualizacja, kompresja, odszumianie, czasem przygotowanie danych. Podkreśl, że PCA nie zna celu predykcyjnego. Kierunek największej wariancji nie musi być kierunkiem najlepiej rozróżniającym klasy. Jeśli zróżnicowanie etykiet kryje się w małej, ale istotnej składowej, agresywna redukcja może zaszkodzić.

**Głębsze dno.** PCA uczy pokory wobec słowa „informacja”. Matematycznie zachowujemy zmienność, ale to nie znaczy, że zachowujemy znaczenie istotne dla konkretnego zadania. Największy ruch w danych może być skutkiem oświetlenia zdjęcia, a drobny sygnał istotnym objawem uszkodzenia. Algorytm nie wie, co jest cenne, dopóki nie zakodujemy celu lub założeń.

**Pytanie.** „Czy zachowanie 95% wariancji gwarantuje zachowanie 95% informacji potrzebnej do klasyfikacji?” Nie.

### 42. Detekcja anomalii: szukamy tego, co nietypowe

**Scenariusz mówiony.** Zacznij od wykrywania awarii przemysłowej. Mamy wiele pomiarów poprawnej pracy maszyny, ale mało przypadków uszkodzeń. Trening może polegać na nauczeniu modelu normalności i wskazywaniu rzadkich lub słabo dopasowanych obserwacji. Przykładowe podejścia to Isolation Forest, metody lokalnej gęstości czy modele rekonstrukcyjne. Każde inaczej definiuje nietypowość: izolowalność, niską gęstość lub wysoki błąd rekonstrukcji.

Omów konsekwencje. W praktyce prawdziwe awarie mogą być bardzo rzadkie, a fałszywe alarmy częste. Trzeba wyznaczyć próg zgodny z kosztem interwencji i utraty sprawności. Rozkład normalności zmienia się wraz z sezonem, zużyciem, zmianą procesu i czujników, więc model wymaga monitoringu.

**Głębsze dno.** „Nietypowe” nie znaczy „złe”. Niezwykła transakcja może być błędem, przestępstwem, ważnym zakupem albo działaniem osoby o nietypowym profilu. Przypisanie znaczenia wymaga dodatkowej wiedzy i weryfikacji. Model anomalii jest narzędziem zwracania uwagi, nie autonomicznym sądem o człowieku czy przyczynie zdarzenia.

**Pytanie.** „Czy w systemie medycznym lepiej mieć mniej fałszywych alarmów czy mniej przeoczonych przypadków?” Odpowiedź zależy od skutków i kontekstu użycia.

### 43. Dlaczego accuracy potrafi wprowadzać w błąd?

**Scenariusz mówiony.** „Załóżmy, że tylko 1% transakcji jest oszustwem. Model, który zawsze mówi »uczciwa«, ma 99% accuracy. Czy nadaje się do wykrywania oszustw? Nie, bo nie wykrywa żadnego”. Zdefiniuj TP, FP, FN i TN. Precision = $TP/(TP+FP)$ oznacza wiarygodność pozytywnych alarmów; recall = $TP/(TP+FN)$ oznacza udział wykrytych prawdziwych przypadków. F1 to średnia harmoniczna precision i recall; nie uwzględnia samodzielnie wszystkich kosztów i nie mówi nic o klasyfikacji negatywnej poza pośrednim wpływem na metryki.

Wyjaśnij wpływ progu klasyfikacyjnego. Zwiększając czułość, możemy zwiększyć liczbę alarmów fałszywych. ROC-AUC mierzy zdolność rankingową w różnych progach, PR-AUC bywa bardziej informatywna przy rzadkich klasach, ale obie metryki wymagają interpretacji względem częstości zjawiska. Kalibracja pyta, czy wśród przypadków ocenionych na 0,8 około 80% rzeczywiście należy do klasy pozytywnej.

**Głębsze dno.** Metryka nie jest neutralnym lustrem skuteczności: wycina fragment konsekwencji. W niektórych systemach fałszywy alarm kosztuje kilkanaście złotych, a przeoczona awaria miliony. W innych sytuacjach automatyczne fałszywe oskarżenie może mieć poważny koszt społeczny. Ocena modelu jest niepełna bez analizy szkody i celu działania.

**Ćwiczenie.** Daj klasie 1000 przypadków, w tym 10 pozytywnych. Niech oszacują accuracy modelu zawsze przewidującego negatywność: 99%; recall: 0%.

### 44. Który algorytm wybrać? Nie ma zwycięzcy uniwersalnego

**Scenariusz mówiony.** „Jeżeli mamy dane tabelaryczne, dobry baseline, sensowne cechy i silne zespoły drzew, nie potrzebujemy na siłę sieci neuronowej. Jeżeli mamy obrazy i dźwięk, warto rozważyć architektury uczące reprezentacji. Jeśli decyzja musi być łatwa do prześledzenia, prosta regresja albo małe drzewo mają istotne zalety”. Podaj macierz kryteriów: jakość na niezależnym teście, koszt treningu i predykcji, odporność, dostępność danych, interpretowalność, wymagania prawne, łatwość utrzymania i rozkład konsekwencji błędów.

Wyjaśnij zasadę baseline: porównujemy model z rozwiązaniem prostym, np. medianą, regułą biznesową albo regresją logistyczną. Bez punktu odniesienia nie wiemy, czy złożoność przyniosła wartość. Dla każdej rodziny modeli istnieją scenariusze, w których jest naturalnym wyborem, i sytuacje, w których zawiedzie.

**Głębsze dno.** Algorytmy to konkurujące hipotezy, nie hierarchia prestiżu. Wybór najbardziej skomplikowanej metody może być objawem źle postawionego pytania. „Najlepszy” oznacza najlepszy względem konkretnego problemu, zestawu założeń, kosztów i okresu użytkowania. Odpowiedzialny projekt AI wymaga możliwości powiedzenia: „nie wiemy jeszcze; sprawdzimy kilka alternatyw w uczciwym eksperymencie”.

**Pytanie.** „Jeśli najprostszy model ma wynik o pół punktu procentowego słabszy, ale jest dziesięciokrotnie tańszy i bardziej przejrzysty, który wybieramy?” To decyzja inżyniersko-biznesowa, nie konkurs metryk.

### 45. Studium przypadku: przewidujemy rezygnację klienta

**Scenariusz mówiony.** Poprowadź małe studium od problemu do decyzji. „Chcemy oszacować, którzy klienci zrezygnują w ciągu następnych 60 dni”. Najpierw określ definicję rezygnacji i dzień, w którym wydajemy prognozę. Następnie wybierz cechy dostępne w tym dniu: historia zakupów, częstotliwość kontaktów, terminy płatności. Podziel zbiór czasowo, aby udawać przyszłe wdrożenie. Zbuduj baseline regresji logistycznej, porównaj z Random Forest i boostingiem. Oceniaj nie tylko ROC-AUC, lecz także precision, recall i kalibrację dla scenariusza interwencji.

Policz intuicyjnie decyzję: koszt telefonu 10 zł, utracona marża przy odejściu 500 zł, a prawdopodobieństwo uratowania klienta po kontakcie zależy od grupy. Wtedy sam churn-score nie wystarczy; należy oszacować także efekt działania. Model przewidujący odejście nie identyfikuje automatycznie klientów, których *da się zatrzymać*.

**Głębsze dno.** Tu ujawnia się różnica między predykcją a interwencją przyczynową. Klient może być wysoko zagrożony, lecz nie reagować na ofertę. Inny ma umiarkowane ryzyko, ale jest bardzo podatny na kontakt. Prawdziwy cel biznesowy często wymaga oszacowania przyrostowego efektu działania, nie wyłącznie ryzyka zdarzenia. To przykład, dlaczego „dobra predykcja” nie jest równoznaczna z „dobrą decyzją”.

**Zamknięcie modułu.** „Przeszliśmy od prostych funkcji do zespołów modeli. Teraz zobaczmy, jak sieć potrafi uczyć nie tylko odpowiedzi, ale i kolejnych poziomów reprezentacji”.


## BLOK IV. SIECI NEURONOWE I DEEP LEARNING

### 46. Sieci neuronowe: otwarcie modułu

**Scenariusz mówiony.** „Tu docieramy do serca szkolenia: jak z elementarnych operacji matematycznych powstaje model, który rozpoznaje obraz, przewiduje złożony sygnał albo generuje tekst”. Zapowiedz cztery pytania. Po pierwsze, czym jest pojedyncza sztuczna jednostka obliczeniowa? Po drugie, co zmienia połączenie setek i tysięcy takich jednostek w warstwy? Po trzecie, jak informacja o błędzie może wpłynąć na każdy parametr, także ten daleko od wyjścia? Po czwarte, dlaczego architektury obrazowe i językowe nie są po prostu ogromnym MLP?

Wyjaśnij język techniczny: sieć neuronowa to zwykle funkcja złożona z wielu parametryzowanych transformacji i nieliniowości. Podczas treningu minimalizujemy określoną stratę. Po treningu wykonujemy przeważnie sam przepływ w przód, czyli wnioskowanie. Nie nazywaj sieci miniaturowym mózgiem; podobieństwo jest inspiracją, nie tożsamością biologiczną.

**Głębsze dno.** Fascynujące jest to, że złożone zachowanie może wyłonić się z prostych reguł lokalnych połączonych w odpowiednią architekturę. Nie wynika z tego, że system ma wiedzę symboliczną o każdym użytym pojęciu. Dobrze oddzielić *moc reprezentacji* od *gwarancji rozumienia*. Sieć może tworzyć bardzo skuteczne kodowanie sygnału, a jednocześnie zawodzić na prostych zmianach kontekstu.

**Przejście.** „Najpierw pojedynczy neuron: żadnej magii, tylko wagi, suma i nieliniowość”.

### 47. Sieć neuronowa nie jest kopią mózgu

**Scenariusz mówiony.** Wyjaśnij historyczną inspirację biologicznym neuronem i od razu pokaż granice analogii. Neuron biologiczny jest złożonym obiektem elektrochemicznym, funkcjonującym w tkance, z dynamiką czasową, plastycznością i wieloma rodzajami sygnałów. W typowym MLP sztuczny „neuron” wykonuje jedną operację: suma ważona plus aktywacja. Miliony takich jednostek nie oznaczają milionów biologicznych neuronów w sensie funkcjonalnej równoważności.

W sieci wiedza nie jest zwykle wpisana w jeden parametr odpowiadający jednemu pojęciu. Parametry współtworzą rozproszone reprezentacje. Przejście od warstwy do warstwy można interpretować jako kolejne przekształcenia cech na potrzeby zadania. Model nie musi posiadać wyraźnie odrębnych modułów „rozumienia”, „pamięci” i „wyobraźni”, aby uzyskiwać wyniki przypominające pewne kompetencje.

**Głębsze dno.** Nie należy wnioskować o naturze umysłu tylko na podstawie wydajności sieci obliczeniowej. Podobieństwo funkcji nie jest dowodem identyczności mechanizmu ani doświadczenia. Z drugiej strony samo to, że sztuczna sieć nie przypomina biologii, nie jest argumentem unieważniającym jej kompetencje obliczeniowe. Najuczciwsze rozróżnienie brzmi: neuron sztuczny jest modelem matematycznym, a nie pełną teorią mózgu.

**Pytanie.** „Czy rozpoznawanie twarzy wymaga od maszyny takiej samej architektury jak ludzki układ wzrokowy?” Nie; może, lecz nie musi, a różne mechanizmy mogą rozwiązywać podobne zadania.

### 48. Anatomia sztucznego neuronu: wejście, waga, bias, aktywacja

**Scenariusz mówiony.** Narysuj trzy wejścia: $x_1,x_2,x_3$. Każde ma przypisaną wagę $w_1,w_2,w_3$. Liczymy $z=w_1x_1+w_2x_2+w_3x_3+b$, potem $a=\phi(z)$. Waga oznacza, jak dana współrzędna wejścia uczestniczy w sumie; jej znak i wartość wpływają na wynik, ale nie należy interpretować jej w oderwaniu od skali i pozostałych parametrów. Bias przesuwa próg działania jednostki. Funkcja aktywacji wprowadza nieliniowość niezbędną do składania naprawdę nowych zależności.

Zrób obliczenie na głos: $x=(2,1)$, $w=(0{,}5,-1)$ i $b=0{,}2$. Otrzymujemy $z=0{,}5\cdot2-1\cdot1+0{,}2=0{,}2$. Dla ReLU wynik to 0,2; dla funkcji progowej, przy progu 0, wynik to 1; dla sigmoid otrzymamy około 0,55. Widzimy, że sama suma ważona i sposób interpretowania wyniku są odrębnymi etapami.

**Głębsze dno.** Parametry neuronu nie są zapisanymi zdaniami o świecie. Są liczbami dostosowywanymi do celu. Kiedy mówimy, że „sieć wie, że rysa jest istotna”, to skrót opisujący stabilny związek między pewnymi aktywacjami a decyzją. Takie skróty bywają przydatne dydaktycznie, lecz łatwo prowadzą do antropomorfizowania rachunku.

**Pytanie.** „Co się stanie, jeżeli dla wszystkich wag ustawimy zero?” W wielu architekturach wystąpi problem symetrii i niemożności zróżnicowania neuronów podczas uczenia.

### 49. Perceptron: granica decyzyjna ma geometrię

**Scenariusz mówiony.** W klasyfikacji liniowej decyzja zależy od znaku $w^Tx+b$. Dla dwóch cech granica $w_1x_1+w_2x_2+b=0$ jest prostą, dla trzech płaszczyzną, dla wielu hiperpłaszczyzną. Wektor wag jest prostopadły do tej granicy. Bias pozwala ją przesuwać. Prosta może skutecznie oddzielić dwie klasy, jeśli w reprezentacji wejściowej ich geometria jest odpowiednia.

Przypomnij XOR. Dla wejść $(0,0)$ i $(1,1)$ klasa ma wartość 0, a dla $(0,1)$ i $(1,0)$ wartość 1. Nie istnieje jedna prosta oddzielająca obie klasy. Potrzebujemy przekształcenia przestrzeni cech albo układu nieliniowych jednostek w warstwie ukrytej. Wyjaśnij, że ograniczenie nie jest wadą sposobu implementacji perceptronu, ale własnością jego klasy funkcji.

**Głębsze dno.** Geometria perceptronu jest lekcją o granicach „prostych odpowiedzi”. To, co w jednej reprezentacji jest nieliniowe i trudne, w innej może stać się łatwo separowalne. Naukę reprezentacji można interpretować jako poszukiwanie przestrzeni, w której ważne relacje ujawniają się w prostszej formie. Dlatego głębokość sieci bywa wartościowa nie przez liczbę parametrów samą w sobie, lecz przez sposób organizacji kolejnych transformacji.

**Ćwiczenie.** Poproś o wskazanie, czy dwie grupy punktów ułożone w koncentryczne kręgi da się rozdzielić jedną prostą. Nie; ale cecha odległości od środka może pomóc.

### 50. MLP: jak powstaje sieć wielowarstwowa?

**Scenariusz mówiony.** MLP, multilayer perceptron, to sieć pełnych połączeń między sąsiednimi warstwami w typowym wariancie. Dla warstwy $l$ zapisujemy $z^{(l)}=W^{(l)}a^{(l-1)}+b^{(l)}$ oraz $a^{(l)}=\phi(z^{(l)})$. Pierwsza warstwa otrzymuje cechy wejściowe, kolejne przekształcają reprezentację, a wyjściowa zwraca odpowiedź dostosowaną do zadania. Przy klasyfikacji wieloklasowej bywa to rozkład po softmax, przy regresji pojedyncza wartość liczbowa.

Wytłumacz liczbę parametrów. Dla warstwy o 10 wejściach i 20 jednostkach otrzymujemy 200 wag plus 20 biasów. Jeśli takich warstw jest wiele, liczba parametrów szybko rośnie. Architektura jest zatem kompromisem pomiędzy ekspresywnością, kosztem obliczeń, ryzykiem przeuczenia i dostępną liczbą przykładów. MLP sprawdza się w wielu zadaniach, ale dla obrazów nie wykorzystuje tak naturalnie struktury sąsiedztwa pikseli jak CNN.

**Głębsze dno.** Każda warstwa wytwarza nowy język opisu danych. Warstwa nie musi jednak tworzyć pojęć, które da się nazwać po ludzku. Wewnętrzne reprezentacje są narzędziami optymalizacji, nie gwarantowaną ontologią świata. Ucząc sieć, wybieramy architekturę, w której złożenie prostych operacji tworzy pożądaną klasę funkcji. To duży krok od ręcznego kodowania cech do ich częściowo automatycznego konstruowania.

**Pytanie.** „Czy dodanie kolejnej warstwy musi poprawić wynik?” Nie, jeśli dane, trening i cel nie uzasadniają większej złożoności.

### 51. ReLU, sigmoid i tanh: po co sieci funkcja aktywacji?

**Scenariusz mówiony.** „Gdyby każda warstwa składała się wyłącznie z mnożenia przez macierz i dodania wektora, to złożenie wielu warstw nadal można byłoby zapisać jako jedną transformację afiniczną”. Zapisz: $W_2(W_1x+b_1)+b_2=(W_2W_1)x+(W_2b_1+b_2)$. Głębokość bez nieliniowości nie zwiększyłaby w tym przypadku rodzaju możliwych funkcji. ReLU, sigmoid i tanh wprowadzają zmiany charakteru transformacji.

ReLU ma postać $\max(0,z)$: dla dodatniego argumentu pochodna wynosi 1, dla ujemnego 0, a w zerze definiujemy ją umownie. Sigmoid zamienia liczby na przedział $(0,1)$ i jest przydatna m.in. na wyjściu binarnym. tanh daje wartości od −1 do 1 i jest symetryczna względem zera. Sigmoid i tanh mogą się nasycać, co skutkuje niewielkimi pochodnymi. ReLU także ma ograniczenia, np. martwe jednostki przy trwale ujemnych aktywacjach.

**Głębsze dno.** Funkcja aktywacji jest małym elementem z dużą konsekwencją: zmienia geometrię funkcji, które cała sieć potrafi reprezentować, oraz jakość przepływu gradientu. To pokazuje, jak duża zmiana właściwości systemu może wynikać z pozornie drobnej decyzji architektonicznej. Uczenie głębokie nie jest jedynie „dodawaniem neuronów”; jest inżynierią przestrzeni reprezentacji i optymalizacji.

**Pytanie.** „Dlaczego nie użyć w każdej warstwie tylko sigmoid?” Z powodu charakterystyki gradientu i warunków treningu.

### 52. Forward pass: od sygnału do predykcji

**Scenariusz mówiony.** Przejdź krok po kroku przez sieć: wejście $x$, pierwsza warstwa $a^{(1)}=\phi(W^{(1)}x+b^{(1)})$, druga warstwa $a^{(2)}=\phi(W^{(2)}a^{(1)}+b^{(2)})$, wyjście $\hat y=g(W^{(3)}a^{(2)}+b^{(3)})$. To *forward pass*: sekwencja działań liczbowych obliczająca predykcję na podstawie aktualnych wag. Podczas zwykłego użycia wytrenowanego modelu wykonujemy właśnie ten proces, bez aktualizacji wag.

Wyjaśnij różnicę między wartościami aktywacji a parametrami. Aktywacje zależą od konkretnego przykładu i zmieniają się między obserwacjami. Wagi stanowią utrwaloną część modelu po treningu, choć mogą zostać zmienione w osobnym procesie dalszego uczenia. Przy klasyfikacji wyjście można interpretować przez softmax, ale nie należy utożsamiać wysokiej liczby po softmax z pewnością w sensie rzeczywistej kalibracji.

**Głębsze dno.** Forward pass odpowiada na pytanie: „Co ta architektura liczy dla danego wejścia?”. Nie mówi jeszcze, czy wynik jest dobry, ani czy model reprezentuje właściwe zjawisko. To obliczenie, a nie samodzielne uzasadnienie. Trafność powstaje dopiero w relacji między wynikiem, celem i procedurą walidacji. Z tego względu kod działający bez błędu i model działający właściwie to dwa różne osiągnięcia.

**Przejście.** „Zobaczmy teraz w animacji, jak sygnał przesuwa się między warstwami”.

### 53. Animacja: sygnał płynie do przodu, błąd wraca

**Scenariusz mówiony.** „Proszę patrzeć na niebieskie impulsy. To tylko ilustracja zależności obliczeniowej: najpierw mamy wejścia, potem aktywacje pierwszej warstwy, później następnej, a na końcu odpowiedź. Teraz wyobraźmy sobie, że odpowiedź jest błędna. Nie cofamy czasu ani nie przesyłamy ‘prawdziwej odpowiedzi’ fizycznie z powrotem. Liczymy pochodne tego błędu względem parametrów. Złoty ruch wstecz symbolizuje obliczenie gradientu zgodnie z regułą łańcuchową”. Zatrzymaj narrację po pierwszej fazie i zapytaj, co już wiemy. Odpowiedź: wynik. Po fazie drugiej wiemy, jak lokalnie zmiana parametrów wpłynęłaby na stratę.

Podkreśl, że animacja jest schematem, a nie zapisem faktycznego treningu z dokładnymi intensywnościami neuronów. Niektóre połączenia mogą w realnym modelu otrzymywać dodatnie, ujemne lub niemal zerowe gradienty. Wagi mogą być współdzielone, a rzeczywiste architektury mają rozgałęzienia, normalizację i połączenia rezydualne.

**Głębsze dno.** Zwróć uwagę na niezwykły charakter wstecznego różniczkowania: nie musimy ręcznie obliczać wpływu każdej wagi na cały wynik od początku. Struktura grafu obliczeniowego pozwala rozłożyć złożony problem na lokalne pochodne. To matematyczny mechanizm przypisywania wpływu, nie psychologiczne poczucie winy modelu. „Błąd wraca” to użyteczna metafora, której granice trzeba znać.

**Pytanie.** „Czy sama propagacja błędu zmienia wagę?” Nie; gradient trzeba jeszcze wykorzystać w kroku optymalizatora.

### 54. Funkcja straty mówi, co poprawić

**Scenariusz mówiony.** Po forward pass mamy predykcję, lecz model nie zna jej jakości, dopóki nie zdefiniujemy celu. Dla regresji użyj przykładu $L=\frac12(\hat y-y)^2$. Dla klasyfikacji binarnej można stosować $L=-[y\log p+(1-y)\log(1-p)]$. Wyjaśnij, że funkcja straty powinna być różniczkowalna lub obsługiwana metodą optymalizacji odpowiednią do jej struktury. Im lepszy sygnał uczenia, tym łatwiej parametrom stopniowo poprawiać wynik, choć obliczenia i jakość danych nadal decydują.

Rozróżnij stratę pojedynczej próbki, stratę średnią batcha i metrykę na walidacji. Możemy uczyć model cross-entropy, a wdrożeniowo optymalizować recall albo koszt fałszywych alarmów. Nie ma obowiązku, aby wszystko było tym samym wzorem; ważne jest logiczne uzasadnienie związku między treningiem a celem użycia.

**Głębsze dno.** W uczeniu nadzorowanym funkcja straty formalizuje to, co uznajemy za poprawne. Wybór celu nie jest neutralny. Dla modelu diagnozującego awarie błąd w jednym kierunku może być droższy niż w drugim. Jeżeli cel zapisano niewłaściwie, sieć może się uczyć doskonale, ale nie tego, czego naprawdę potrzebujemy. To odpowiednik problemu Goodharta w sztucznej inteligencji: matematyczne zwycięstwo nad metryką nie musi być realnym zwycięstwem nad problemem.

**Pytanie.** „Czy sieć powinna maksymalizować prawdopodobieństwo odpowiedzi czy minimalizować ryzyko decyzji?” To często dwa różne etapy systemu.

### 55. Gradient: w którą stronę zmienić każdą wagę?

**Scenariusz mówiony.** „Wyobraźcie sobie krajobraz górski, gdzie wysokość jest wartością straty, a położenie w przestrzeni to wektor wszystkich parametrów”. Gradient $\nabla_\theta L$ pokazuje kierunek najszybszego lokalnego wzrostu straty w zwykłej geometrii euklidesowej. Aby zmniejszać stratę, wykonujemy krok przeciwny: $\theta_{new}=\theta_{old}-\eta\nabla_\theta L$. Wielkość $\eta$ to learning rate. W jednym wymiarze wyjaśnij znak: jeśli pochodna jest dodatnia, zmniejszamy parametr; jeśli ujemna, zwiększamy.

Zaznacz, że powierzchnia straty w głębokiej sieci jest wielowymiarowa i niekoniecznie wypukła. Gradient opisuje lokalną informację, nie globalną gwarancję najlepszego minimum. Przy zbyt dużym kroku można przekroczyć dolinę i destabilizować trening; przy zbyt małym uczenie będzie powolne. Minibatch wprowadza szum do estymacji gradientu, który czasem jest użyteczny, choć utrudnia interpretację jednej aktualizacji.

**Głębsze dno.** Gradient mówi, jak zmienia się liczba reprezentująca nasz cel, nie jak „prawdziwy” jest model. Jest mechanizmem optymalizacji, a nie świadectwem poprawności zadania. Sieć może błyskawicznie schodzić po krajobrazie straty, a jednocześnie generalizować źle albo realizować źle zdefiniowaną funkcję celu. Zrozumienie matematyki uczy zarazem jej ograniczeń.

**Pytanie.** „Czy spadek straty treningowej oznacza automatycznie coraz lepszą jakość wdrożeniową?” Nie.

### 56. Backpropagation: reguła łańcuchowa w skali sieci

**Scenariusz mówiony.** Zacznij od zależności złożonej: $L=L(a(z(w)))$. Aby policzyć wpływ wagi na stratę, używamy $\partial L/\partial w=(\partial L/\partial a)(\partial a/\partial z)(\partial z/\partial w)$. To po prostu reguła łańcuchowa. W sieci są tysiące lub miliardy wag, dlatego wykorzystujemy strukturę grafu obliczeniowego: obliczamy aktywacje w przód, przechowujemy potrzebne wartości pośrednie, a następnie propagujemy pochodne od wyjścia do wcześniejszych warstw.

Dla dwóch warstw pokaż symboliczną zależność: $\delta^{(L)}=\partial L/\partial z^{(L)}$, a dla warstwy ukrytej $\delta^{(l)}=(W^{(l+1)})^T\delta^{(l+1)}\odot\phi'(z^{(l)})$. Gradient wag to $\partial L/\partial W^{(l)}=\delta^{(l)}(a^{(l-1)})^T$. Nie musisz wymagać zapamiętania tych wzorów. Celem jest zrozumienie, że wpływ na błąd przechodzi przez pochodne kolejnych operacji.

**Głębsze dno.** Odseparuj trzy pojęcia. **Forward pass** wylicza przewidywanie. **Backpropagation** efektywnie wylicza gradienty straty względem parametrów. **Optymalizator** (np. SGD lub Adam) wykorzystuje je do aktualizacji wag. W szkoleniach często miesza się te etapy, co utrudnia zrozumienie działania. Backprop nie jest również uniwersalną teorią uczenia biologicznego; to algorytm różniczkowania funkcji złożonych.

**Pytanie.** „Czy optymalizator musi znać wszystkie pochodne ręcznie?” Nie; można je obliczać automatycznie na grafie operacji.

### 57. Jedna iteracja uczenia w ruchu

**Scenariusz mówiony.** Odtwórz czterostopniową sekwencję: (1) wejście przesuwa się przez warstwy zgodnie z aktualnymi wagami; (2) wyjście jest porównywane z celem i powstaje strata; (3) pochodne są obliczane wstecz; (4) optymalizator aktualizuje parametry. Potem kolejna próbka lub batch przechodzi przez już nieco inny model. Powiedz wyraźnie, że podczas wnioskowania produkcyjnego zwykle wykonujemy tylko etap pierwszy, bez etykiety i bez kroku aktualizacji.

Zrób analogię z kalibracją przyrządu: mamy ustawienia, odczyt i odchylenie od wzorca. Obliczamy, jak zmiana każdego regulatora może wpłynąć na błąd. To analogia do optymalizacji, ale sieć posiada wiele wzajemnie sprzężonych „regulatorów”. W praktyce update nie zawsze zmniejsza stratę pojedynczej próbki; ważniejszy jest trend jakości na danych treningowych i walidacyjnych.

**Głębsze dno.** Uczenie jest sekwencją lokalnych korekt w zdefiniowanej przestrzeni parametrów. Nie oznacza, że system buduje kompletną teorię świata. Zmienia sposób przetwarzania sygnałów tak, aby zredukować błąd w zadaniu. Właśnie dlatego potrafi nabywać potężne kompetencje, a jednocześnie dziedziczyć błędne etykiety i korelacje pozorne.

**Ćwiczenie.** Zatrzymaj animację mentalnie na fazie gradientu: „Czy teraz znamy nową predykcję?” Nie, dopóki nie zaktualizujemy wag i nie przeprowadzimy kolejnego forward pass.

### 58. Przykład: jeden neuron i jeden krok gradientowy

**Scenariusz mówiony.** Pokaż cały rachunek bez skrótów. Dane: $x=2$, początkowa waga $w=0{,}5$, bias $b=0$, wartość oczekiwana $y=2$. Predykcja neuronu liniowego: $\hat y=wx+b=0{,}5\cdot2=1$. Przy stracie $L=\frac12(\hat y-y)^2$ otrzymujemy $L=\frac12(1-2)^2=0{,}5$. Liczymy pochodną względem wagi: $\frac{\partial L}{\partial w}=(\hat y-y)\cdot x=(1-2)\cdot 2=-2$. Przy learning rate $\eta=0{,}1$ mamy $w_{new}=0{,}5-0{,}1\cdot(-2)=0{,}7$. Jeśli bias pozostaje nieruchomy, nowa predykcja to $0{,}7\cdot2=1{,}4$.

Dopowiedz, że nowa strata wynosi $\frac12(1{,}4-2)^2=0{,}18$, czyli w tym przykładzie spadła z 0,5 do 0,18. Gdyby równocześnie uczono bias, mielibyśmy dodatkową pochodną $\partial L/\partial b=\hat y-y=-1$, a nowy bias wyniósłby 0,1; slajd świadomie trzyma bias stały, żeby rachunek był przejrzysty.

**Głębsze dno.** Ten prosty przykład jest matematycznym „mikroskopem” uczenia głębokiego. W rzeczywistej sieci każda waga ma analogiczny wpływ na stratę, tyle że zależność biegnie przez wiele operacji. Backpropagation pozwala policzyć takie pochodne efektywnie. Algorytm nie „wie”, że 1,4 jest semantycznie bliżej celu 2; to własność wybranej funkcji straty i rachunku pochodnych.

**Pytanie.** „Czy po jednej dobrej aktualizacji mamy już wytrenowany model?” Nie, iterujemy dla wielu przykładów, obserwując generalizację.

### 59. Epoch, batch, learning rate: rytm uczenia

**Scenariusz mówiony.** Wyjaśnij trzy terminy w języku procesu. **Epoch** to jedno przejście przez zbiór treningowy. **Batch** to porcja przykładów, na której wyliczamy zbiorczy gradient. **Learning rate** steruje skalą kroku aktualizacji. Jeśli mamy 10 000 przykładów i batch size 100, typowe pełne przejście wymaga około 100 aktualizacji (pomijając szczegóły ostatniej partii). Sto epok nie oznacza sto kroków, lecz około 10 tysięcy aktualizacji w takim przykładzie.

Omów trade-off. Małe batche powodują bardziej zaszumione gradienty; duże pozwalają sprawniej wykorzystać sprzęt i zmieniają charakter optymalizacji. Optymalizator, harmonogram learning rate, inicjalizacja i regularizacja współdecydują o stabilności. Nie należy dobierać liczby epok „na oko” bez sprawdzania wyniku walidacyjnego. Warto obserwować także rozjazd między stratą treningową i walidacyjną.

**Głębsze dno.** Uczenie to proces zależny od ścieżki. Dwa modele z tymi samymi danymi i architekturą mogą uzyskać różne parametry, jeśli różnią się inicjalizacją i kolejnością batchy. Nie oznacza to, że nauka jest arbitralna: testujemy statystyczną stabilność. Wysoka dokładność jednego treningu bez sprawdzenia wariancji wyników może dawać złudne poczucie pewności.

**Pytanie.** „Czy większa liczba epok zawsze poprawia model?” Nie; może poprawiać trening, a pogarszać walidację.

### 60. Dlaczego głęboka sieć może się nie uczyć?

**Scenariusz mówiony.** Przedstaw zanikanie gradientu: jeśli pochodne wielu kolejnych operacji mają niewielkie wartości, ich iloczyn może stać się bardzo mały i pierwsze warstwy uczą się wolno. Eksplodujące gradienty są zjawiskiem przeciwnym: pochodne mogą niekontrolowanie rosnąć, prowadząc do niestabilności. Źródłami problemów mogą być nasycające funkcje aktywacji, zła skala inicjalizacji, głębokość, brak normalizacji albo nieodpowiedni learning rate.

Wyjaśnij metody zaradcze bez robienia katalogu bibliotek: dobra inicjalizacja, ReLU i pokrewne aktywacje w odpowiednich miejscach, normalizacja, połączenia rezydualne, gradient clipping w niektórych architekturach, ostrożny harmonogram uczenia. Podkreśl, że żadna z technik nie gwarantuje sukcesu przy złych danych lub funkcji celu.

**Głębsze dno.** Pojawia się subtelna zasada: zdolność modelu do reprezentowania rozwiązania i zdolność algorytmu do *odnalezienia* tego rozwiązania to dwie różne rzeczy. Istnieją funkcje, które dana architektura mogłaby teoretycznie obliczać, ale trening praktyczny nie znajduje dobrych parametrów. Matematyczna ekspresywność bez dobrze uwarunkowanej optymalizacji nie wystarcza.

**Pytanie.** „Jeżeli model ma miliony parametrów, czy na pewno potrafimy je skutecznie nauczyć?” Nie; zależy to także od dynamiki gradientu i danych.

### 61. Dropout, early stopping i regularizacja wag

**Scenariusz mówiony.** Regularizacja ma pomagać zachować dobrą predykcję na nowych danych, zamiast bez końca dopasowywać trening. **Dropout** losowo wyłącza część aktywacji podczas treningu, co ogranicza nadmierne poleganie na pojedynczych ścieżkach i może poprawiać uogólnianie. **Weight decay** ogranicza wielkość parametrów lub wprowadza odpowiednią presję optymalizacyjną. **Early stopping** kończy trening, gdy jakość walidacyjna przestaje się poprawiać według ustalonej reguły.

Dodaj inne możliwości: więcej reprezentatywnych danych, sensowna augmentacja, uproszczenie architektury i poprawienie etykiet. Wyjaśnij, że dropout działa zwykle inaczej podczas treningu i ewaluacji; nie należy w prostym języku mówić, że model „zapomina losowo neurony na produkcji”.

**Głębsze dno.** Regularizacja jest matematycznym wyrazem ostrożności wobec nadmiernej pewności dopasowania. Preferujemy rozwiązania, które nie wymagają zapamiętania każdej osobliwości danych. W filozofii nauki podobną intuicję wyraża oszczędność hipotez, lecz analogii nie należy rozumieć dosłownie: prostota parametryczna nie gwarantuje prawdziwości, a skomplikowane zjawiska czasem wymagają skomplikowanych modeli.

**Pytanie.** „Co jest bardziej wartościowe: model perfekcyjny na treningu czy nieco słabszy na treningu, ale stabilniejszy na przyszłych danych?” W produkcji zwykle ten drugi.

### 62. CNN: dlaczego konwolucja działa na obrazach?

**Scenariusz mówiony.** Obraz ma strukturę przestrzenną: pobliskie piksele zwykle tworzą lokalne wzorce. CNN wykorzystuje tę własność przez filtry stosowane w wielu położeniach. Ten sam zestaw wag wykrywa podobny motyw niezależnie od miejsca jego wystąpienia, co ogranicza liczbę parametrów i wprowadza użyteczną własność równoważności względem przesunięć dla określonych operacji. Kolejne mapy cech mogą reprezentować krawędzie, tekstury i bardziej złożone struktury.

Przy prostym filtrze 3×3 pokaż intuicję: dziewięć wag przechodzi nad kolejnymi fragmentami obrazu i tworzy wynikowy sygnał. Przesunięcie `stride` lub pooling zmniejsza rozdzielczość reprezentacji, zwykle kosztem części informacji przestrzennej. CNN nie jest jedynym nowoczesnym podejściem do wizji, ale znakomicie pokazuje rolę założeń architektury.

**Głębsze dno.** CNN to przykład *inductive bias*: twórca modelu zakłada, że lokalność i powtarzalność wzorców w obrazie są ważne. Te założenia nie są błędem; ograniczają przestrzeń możliwych modeli tak, aby wykorzystać strukturę świata. Głębokie uczenie nie jest zatem całkowicie wolne od wiedzy projektanta. Jest połączeniem założeń architektury i relacji odkrywanych w danych.

**Pytanie.** „Dlaczego nie stosować identycznego układu cech do obrazu i tabeli księgowej?” Bo struktura i rodzaj istotnych relacji są inne.

### 63. Od pikseli do reprezentacji: hierarchia cech w CNN

**Scenariusz mówiony.** Pokaż obraz jako kolejne warstwy interpretacji. Wczesne filtry mogą reagować na kontrast, orientacje krawędzi i lokalne częstotliwości przestrzenne. Warstwy późniejsze mogą łączyć informacje w tekstury, fragmenty kształtów oraz reprezentacje zależne od zadania. Nie każda sieć wykazuje idealną, jednoznaczną „hierarchię od krawędzi do obiektów”; to użyteczna tendencja, nie żelazne prawo. Uczciwy opis mówi o coraz bogatszych reprezentacjach cech związanych z optymalizowanym zadaniem.

Opisz przykład wady materiału: pojedynczy filtr reaguje na ostrą zmianę jasności, kilka filtrów na układ linii, a dalsze warstwy mogą rozpoznawać wzór charakterystyczny dla pęknięcia. Sieć nie musi posiadać jawnego zdania „to jest pęknięcie”, aby końcowa funkcja skutecznie klasyfikowała obraz. Ale wynik może być fałszywie napędzany tłem, oznaczeniem partii lub charakterystycznym oświetleniem.

**Głębsze dno.** Hierarchia reprezentacji przypomina abstrakcję: od lokalnego sygnału do pojęcia użytecznego dla zadania. Jednak model może nauczyć się także skrótów pozornych, tzw. shortcut learning. Głębia nie gwarantuje semantycznej czystości. Aby sprawdzić, *na czym* model rzeczywiście polega, potrzebne są testy odporności, zmiany warunków obrazu, analiza błędów, a czasem eksperymenty interwencyjne.

**Pytanie.** „Czy model rozpoznaje wadę, jeśli po zmianie koloru oświetlenia przestaje działać?” Być może polegał na niewłaściwej wskazówce.

### 64. Attention: modelowanie zależności między elementami

**Scenariusz mówiony.** Wyjaśnij, że Transformer tworzy reprezentacje tokenów i pozwala im dynamicznie pobierać informację z innych pozycji. Każda pozycja ma wektory query, key i value. Dopasowanie query do key pomaga ustalić wagi uwagi, a te służą do połączenia wartości. W uproszczeniu: $\mathrm{Attention}(Q,K,V)=\mathrm{softmax}(QK^T/\sqrt{d_k})V$. Nie trzeba wykonywać dużego mnożenia macierzy na tablicy; liczy się mechanizm ważonej wymiany informacji.

Daj zdanie: „Anna dała Marii książkę, ponieważ *ona* miała ją przeczytać”. Która osoba jest referentem „ona”? Kontekst ma znaczenie, a zależności nie muszą dotyczyć tylko sąsiednich słów. Mechanizm uwagi może modelować takie powiązania, ale sama mapa uwagi nie jest pełnym, prostym wyjaśnieniem przyczyn decyzji modelu. Wiele głów uwagi wychwytuje różne typy relacji; nie wszystkie są semantycznie intuicyjne.

**Głębsze dno.** „Attention” jest nazwą mechanizmu matematycznego, a nie twierdzeniem o świadomości lub intencjonalności. Ujawnia ważną ideę: znaczenie reprezentacji elementu jest zależne od kontekstu. W wyrażeniach językowych podobne tokeny mają inne role w różnych zdaniach. Transformer uczy się funkcji aktualizacji reprezentacji na podstawie statystycznych zależności; nie otrzymujemy przez to automatycznej gwarancji prawdziwości każdej odpowiedzi.

**Pytanie.** „Czy wysokie wagi attention stanowią wystarczające wyjaśnienie odpowiedzi?” Zwykle nie; potrzebne są dodatkowe metody analizy.

### 65. Embedding: znaczenie zamienione w geometrię

**Scenariusz mówiony.** Embedding jest wektorową reprezentacją obiektu: słowa, fragmentu tekstu, obrazu, klienta czy produktu. W modelu możemy badać odległości i podobieństwo takich wektorów. Dla tekstu podobne użycia językowe mogą prowadzić do podobnych reprezentacji, choć konkretna geometria zależy od danych i celu uczenia. Nie twierdź, że każda oś wektora ma odrębne znaczenie słownikowe; często informacja jest zakodowana rozproszenie.

Pokaż zastosowanie do wyszukiwania semantycznego. Pytanie „jak reklamować wadliwy produkt?” może być bliskie fragmentowi „procedura zgłoszenia usterki”, nawet jeśli słowa nie są identyczne. Embedding pomaga odszukać kandydatów. Wyszukanie podobnego fragmentu nie jest jeszcze dowodem, że jest on aktualny, prawdziwy lub prawnie właściwy. Dlatego retrieval potrzebuje kontroli źródła, wersji i kontekstu.

**Głębsze dno.** Geometria reprezentacji jest mapą relacji przydatnych w zadaniu, nie pełnym odwzorowaniem znaczenia. Podobieństwo statystyczne może odzwierciedlać także stereotypy i historyczne nierówności obecne w danych. W tym sensie embedding pokazuje siłę uczenia reprezentacji, ale też jego zależność od materiału, w którym język i świat zostały zapisane.

**Pytanie.** „Jeśli dwa zdania są blisko w przestrzeni wektorowej, czy ich twierdzenia są równie prawdziwe?” Nie; podobieństwo i prawda są różnymi wielkościami.

### 66. Czego sieci neuronowe nie gwarantują?

**Scenariusz mówiony.** Podsumuj typowe granice: model może błędnie generalizować po zmianie rozkładu, polegać na pozornych korelacjach, mylić się z dużą pewnością, przenosić stronniczość danych i być podatny na celowo nietypowe wejścia. W generowaniu treści płynność języka nie gwarantuje prawdziwości. Dobre wyniki benchmarkowe są ważnym dowodem, ale nie stanowią gwarancji we wszystkich możliwych warunkach.

Omów praktykę wdrożeniową: wersjonowanie danych i modeli, testy przypadków granicznych, pomiar kalibracji, monitoring przesunięć rozkładu, analiza błędów krytycznych, możliwość ludzkiej kontroli i warunków wyłączenia. Nie każdy projekt wymaga identycznej procedury; skala kontroli powinna odpowiadać ryzyku i skutkom błędów.

**Głębsze dno.** Model jest reprezentacją wycinka rzeczywistości, a nie rzeczą samą w sobie. Nie potrafimy dowieść jego uniwersalnej prawdziwości przez ograniczony zestaw testów. Możemy natomiast gromadzić dowody, określać granice użycia i budować mechanizmy odpowiedzialnego reagowania na błąd. W nauce ważne jest nie tylko to, co model trafnie opisuje, ale także umiejętność rozpoznania, gdzie jego kompetencja się kończy.

**Pytanie.** „Kiedy powinniśmy pozwolić algorytmowi działać samodzielnie, a kiedy wymagać potwierdzenia człowieka?” Powiąż odpowiedź z odwracalnością skutków i kosztem pomyłki.

### 67. Od formalnego neuronu do modeli fundamentalnych

**Scenariusz mówiony.** Zepnij całą historię czterema poziomami. **Neuron:** liczbowo przekształca wejście w aktywację. **Sieć:** złożenie wielu transformacji tworzy funkcję zdolną do reprezentowania skomplikowanych zależności. **Uczenie:** dopasowuje parametry przez minimalizowanie straty i wyznaczanie gradientu. **System:** łączy wytrenowany model z danymi, narzędziami, politykami, ludźmi i środowiskiem działania. Rozdzielenie tych poziomów zapobiega myleniu przełomu matematycznego z rozwiązaniem operacyjnym.

Wyjaśnij, dlaczego duże modele stały się praktyczne: architektury, duże dane, sprzęt, optymalizacja i sposoby adaptacji. Sama liczba parametrów nie stanowi definicji inteligencji ani niezawodności. System z mniejszym modelem może być lepszy w wąskim, kontrolowanym zadaniu, jeśli ma poprawne źródła i procedury sprawdzania wyniku.

**Głębsze dno.** Ewolucja sieci jest także historią przejścia od ręcznej reprezentacji do reprezentacji uczonej. Ale z „model uczy się cech” nie wynika „model posiada kompletną wiedzę o świecie”. Odpowiedzialna architektura powinna znać miejsce granicy: co jest wyuczone, co jawnie zapisane, co musi być sprawdzone i kto może uruchomić działanie.

**Przejście.** „Zostało nam pięć pytań, od których zaczęliśmy. Sprawdźmy, czy potrafimy na nie odpowiedzieć”.

## ZAKOŃCZENIE I SYNTEZA

### 68. Co warto zapamiętać po całym wykładzie?

**Scenariusz mówiony.** Podsumuj w czterech zdaniach. „AI to nie jeden algorytm, lecz wiele sposobów budowania systemów wnioskujących i działających. Machine Learning uczy się zależności na podstawie danych i informacji zwrotnej. Deep Learning składa wiele transformacji, aby wytwarzać użyteczne reprezentacje. A wdrożona AI to model plus dane, procedury, ludzie i odpowiedzialność”. Następnie przejdź jeszcze raz przez pięć pytań: problem, wejście i wyjście, reprezentacja, kryterium błędu, test poza treningiem.

Przywołaj kilka przykładów: regresja dobrze nadaje się do zrozumiałego punktu odniesienia, SVM pokazuje sens marginesu, Random Forest redukcję wariancji przez agregację, boosting iteracyjną korektę, CNN wykorzystanie lokalności obrazu, attention kontekstowe ważenie relacji. Każda metoda jest odpowiedzią na konkretny rodzaj problemu, a nie kolejnym szczeblem prestiżu.

**Głębsze dno.** Dojrzałość w AI polega na umiejętności odróżniania obliczenia od wiedzy, korelacji od przyczynowości, sprawności zadaniowej od pełnego rozumienia oraz modelu od systemu społeczno-technicznego. Matematyka daje narzędzia do mierzenia i poprawy działania, ale nie usuwa konieczności odpowiedzialnego formułowania celu. W tym sensie AI jest nie tylko historią bardziej wyrafinowanych algorytmów, lecz także historią coraz trudniejszych pytań, które zadajemy własnym narzędziom poznawczym.

**Pytanie końcowe przed bibliografią.** „Które założenie o danych najłatwiej przeoczyć, gdy zachwyca nas wynik modelu?”

### 69. Źródła i dalsza lektura

**Scenariusz mówiony.** „Nie musicie zapamiętać wszystkich dat i równań. Ważne, by wiedzieć, gdzie szukać źródeł pierwotnych i jak odróżniać wynik badania od popularnego uproszczenia”. Wskaż publikację Turinga z 1950 roku jako źródło filozoficzno-metodologiczne, propozycję Dartmouth z lat 1955–1956 jako dokument założycielski, pracę McCullocha i Pittsa jako wczesną formalizację neuronu, klasyczne prace o propagacji wstecznej jako podstawę treningu warstwowego, AlexNet jako przełom w rozpoznawaniu obrazów, badania Deep Blue i AlphaGo jako dwa odmienne paradygmaty rozwiązywania problemów oraz „Attention Is All You Need” jako ważną publikację w rozwoju Transformerów.

Oddziel źródła naukowe od źródeł definicji regulacyjnych, takich jak OECD i instytucjonalne materiały do AI Act. Definicje regulacyjne służą określeniu zakresu prawa i obowiązków, nie zastępują eksperymentalnego dowodu skuteczności. Właściwa praktyka to czytać nie tylko streszczenie, ale również założenia, zbiór danych, metodę i ograniczenia.

**Głębsze dno.** AI to dziedzina, w której narracja medialna bywa znacznie szybsza od krytycznej weryfikacji. Nauka wymaga czegoś odwrotnego: dokładnego określenia, jaki rezultat uzyskano, w jakim środowisku, dla jakiej próby i jakimi metodami. Rozróżnienie między demonstracją a powtarzalnym wynikiem jest lekcją dotyczącą całej współczesnej technologii.

**Wskazówka.** Zachęć do dalszej lektury zarówno matematyków uczenia, jak i tekstów o metodologii, ograniczeniach, kalibracji oraz bezpieczeństwie systemów.

### 70. Czy model nauczył się świata, czy tylko śladów po nim?

**Scenariusz mówiony.** Zatrzymaj na chwilę slajd bez dodatkowego przełączania. „To nie jest pytanie retoryczne, na które trzeba odpowiedzieć jednym słowem. Model otrzymuje ślady świata: obrazy, pomiary, teksty, decyzje, etykiety. Uczy się regularności w tych śladach. Czasem są tak stabilne, że pozwalają skutecznie przewidywać nowe zdarzenia. Czasem stanowią jedynie echo sposobu, w jaki zebraliśmy dane. Wówczas system działa świetnie w laboratorium i zawodzi w zetknięciu z innym światem”.

„Nie umniejszajmy potęgi tego mechanizmu. Z samych statystycznych regularności można zbudować zdumiewająco skuteczne systemy. Jednocześnie nie powinniśmy mylić skutecznego modelowania z pełną wiedzą o przyczynach, znaczeniu i skutkach działania. Dobrze zaprojektowana AI potrafi nam pomóc zobaczyć wzory, których nie dostrzegaliśmy. Ale odpowiedzialność za to, co uznamy za ważne, jakie pytanie zadamy i co zrobimy z odpowiedzią, nadal wymaga świadomego projektu i nadzoru”.

**Głębsze dno.** Najtrwalsza myśl tego wykładu jest epistemologiczna: reprezentacja nie jest tożsama z rzeczywistością. Nie oznacza to, że wszystkie modele są bezużyteczne czy arbitralne. Oznacza, że ich prawomocność jest warunkowa: związana z danymi, celem, założeniami i testami. Inteligencję maszyn można badać przez mechanizmy i kompetencje, ale nie należy z każdej udanej predykcji wyciągać twierdzenia metafizycznego. Nasze zadanie jako projektantów systemów polega na tym, by wiedzieć, gdzie kończą się dowody, a zaczynają oczekiwania.

**Ostatnie pytanie do słuchaczy.** „Gdy jutro zobaczycie model, który imponuje odpowiedziami, jakie pięć pytań zadacie, zanim uznacie, że można mu powierzyć decyzję?” Zakończ powrotem do slajdu 4.

---

## Bibliografia orientacyjna i uwagi metodologiczne

- Alan M. Turing (1950), *Computing Machinery and Intelligence*, *Mind*, 59(236), 433–460, https://doi.org/10.1093/mind/LIX.236.433.
- McCulloch, W. S., Pitts, W. (1943), *A Logical Calculus of the Ideas Immanent in Nervous Activity*, *Bulletin of Mathematical Biophysics*.
- McCarthy, J., Minsky, M., Rochester, N., Shannon, C. (1955), *A Proposal for the Dartmouth Summer Research Project on Artificial Intelligence*, https://www-formal.stanford.edu/jmc/history/dartmouth/dartmouth.html.
- Rumelhart, D. E., Hinton, G. E., Williams, R. J. (1986), *Learning representations by back-propagating errors*, *Nature*.
- Krizhevsky, A., Sutskever, I., Hinton, G. (2012), *ImageNet Classification with Deep Convolutional Neural Networks*.
- Silver, D. i in. (2016), *Mastering the game of Go with deep neural networks and tree search*, *Nature*.
- Vaswani, A. i in. (2017), *Attention Is All You Need*, arXiv:1706.03762.
- Goodfellow, I., Bengio, Y., Courville, A. (2016), *Deep Learning*, MIT Press, https://www.deeplearningbook.org/.
- Bishop, C. M. (2006), *Pattern Recognition and Machine Learning*, Springer.
- Murphy, K. P. (2022), *Probabilistic Machine Learning: An Introduction*, MIT Press.
- Sutton, R. S., Barto, A. G. (2018), *Reinforcement Learning: An Introduction*, 2nd ed.
- OECD AI Principles / definition of an AI system: https://oecd.ai/en/ai-principles.

W notatkach odróżniono uproszczenia dydaktyczne od twierdzeń matematycznych. Animacja propagacji sygnału i gradientu jest schematyczna. Daty historyczne odnoszą się do znanych publikacji/wydarzeń, nie oznaczają, że idee pojawiły się dokładnie w danym roku po raz pierwszy.
