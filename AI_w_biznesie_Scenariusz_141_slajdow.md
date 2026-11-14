# Wstęp do AI w biznesie

## Scenariusz wykładu dla prowadzącego

Numery odpowiadają kolejności w pliku z 141 slajdami. Tekst w nawiasach kwadratowych to wskazówki dla prowadzącego.

## Slajd 001 — Wstęp do AI w biznesie

Dzień dobry Państwu. Wyobraźmy sobie, że zarząd daje nam trzy miesiące i budżet na pierwsze wdrożenie AI. Który proces wybieramy i skąd po tych trzech miesiącach będziemy wiedzieć, że decyzja była dobra? Do tego pytania wrócimy na końcu. Po drodze zobaczymy, jak działają modele i które ich właściwości zmieniają rachunek biznesowy.

## Slajd 002 — Wstęp do sztucznej inteligencji

Zapraszam Państwa do wejścia w sztuczną inteligencję trochę głębiej, niż pozwala codzienny język reklam i nagłówków. Będziemy rozmawiać o systemach, które rozpoznają, przewidują, generują i działają, ale również o nas: o tym, dlaczego tak szybko przypisujemy im wiedzę, intencję i autorytet.

Nie trzeba dziś znać rachunku macierzowego ani umieć programować sieci neuronowej. Potrzebna będzie gotowość do zadawania dokładnych pytań. Gdy zobaczymy dobry wynik, zapytamy, w jakich warunkach powstał. Gdy usłyszymy płynną odpowiedź, sprawdzimy jej uzasadnienie. Gdy ktoś powie, że system sam podjął decyzję, ustalimy, kto wybrał jego cel i kto dopuścił go do działania.

Po tym spotkaniu chciałbym, żeby potrafili Państwo opisać podstawowe mechanizmy AI i rozpoznać moment, w którym techniczna odpowiedź przestaje wystarczać. To szczególnie ważne wtedy, gdy wynik obliczenia zaczyna wpływać na cudze życie.

Najgłębsze pytanie tego wykładu dotyczy granicy między tym, co potrafimy obliczyć, a tym, co potrafimy uzasadnić. Te granice nie muszą się pokrywać. Możemy zbudować skuteczny system, nie rozumiejąc w pełni wszystkich powodów jego sukcesu. Możemy też dokładnie znać jego instrukcje, a nadal nie mieć dobrego powodu, żeby powierzyć mu określoną władzę.

Zanim przejdziemy do mechanizmów, krótko przedstawię perspektywę, z której będziemy na nie patrzeć.

## Slajd 003 — Marcin Albiniak

Nazywam się Marcin Albiniak. Jestem kierownikiem studiów AI Mastery: Teoria i Implementacja Sztucznej Inteligencji w Systemach Informatycznych oraz programu Biznes w erze AI. Budowanie umiejętności przyszłości.

Same nazwy tych programów pokazują dwa punkty widzenia, które będą się dzisiaj spotykały. Z jednej strony mamy konstrukcję systemów: dane, modele, algorytmy i sposób sprawdzania wyników. Z drugiej mamy organizacje i ludzi, którzy muszą zdecydować, do czego tych systemów użyją, za co zapłacą oraz jak rozpoznają, czy technologia rzeczywiście pomogła.

Nie chciałbym rozdzielać tych perspektyw. Inżynier potrzebuje rozumieć skutki własnych uproszczeń, a osoba podejmująca decyzję biznesową potrzebuje rozumieć ograniczenia narzędzia. W przeciwnym razie rozmawiamy o tym samym systemie, używając tych samych słów, ale nadając im całkowicie różne znaczenia.

W praktyce odpowiedzialne korzystanie z AI wymaga umiejętności tłumaczenia między językami. Słowo „dokładność” znaczy coś konkretnego w eksperymencie, a coś znacznie szerszego dla człowieka, który obawia się błędnej decyzji. Będziemy pilnować, żeby te znaczenia nie rozchodziły się niezauważenie.

Dlatego proponuję trzy pytania, które będą towarzyszyły nam przez cały wykład.

## Slajd 004 — Perspektywa prowadzącego

Pierwsze pytanie brzmi: jak działa mechanizm? Nie zawsze potrzebujemy znać każdy parametr, ale powinniśmy wiedzieć, jaki problem system rozwiązuje i skąd bierze informacje. Klasyfikator dokumentów, generator tekstu i robot poruszający się po magazynie mają zupełnie inne relacje ze światem.

Drugie pytanie brzmi: jak sprawdzamy wynik? Piękna demonstracja pokazuje, że coś może się udać. Rzetelny test ma pokazać, jak często się udaje, gdzie zawodzi i czy poradzi sobie z przypadkami, których wcześniej nie widział.

Trzecie pytanie brzmi: kto poniesie koszt pomyłki? Osoba kupująca system, osoba obsługująca alarm i osoba oceniona przez model mogą mieć różne interesy. Jeżeli zaoszczędzimy czas jednej grupy, przenosząc cały koszt błędów na drugą, nie powinniśmy nazywać tego sukcesem bez dodatkowego uzasadnienia.

Te pytania układają się w trzy poziomy: działanie, wiedza i odpowiedzialność. Kłopoty zaczynają się wtedy, gdy dowód z jednego poziomu przenosimy na drugi. Z faktu, że system działa zgodnie z projektem, nie wynika jeszcze, że projekt był właściwy. Z wysokiej trafności nie wynika automatycznie prawo do decydowania o człowieku.

Proszę teraz zachować w pamięci jedno zastosowanie AI z własnej pracy. Będziemy do niego wracać.

## Slajd 005 — Mapa wykładu

Zaczniemy od tego, co właściwie nazywamy AI i jak oceniamy inteligencję systemu. Następnie przejdziemy do mechanizmów, od uczenia maszynowego przez reguły i język aż po agentów. W ostatniej części zastanowimy się, jak te mechanizmy zmieniają decyzje w firmie i kto bierze za nie odpowiedzialność.

## Slajd 006 — Pięć decyzji podczas wykładu

Przez cały wykład będziemy wracać do pięciu decyzji. Najpierw wskażemy miejsce, w którym firma traci czas lub pieniądze. Potem sprawdzimy, co wiadomo w chwili podejmowania decyzji. Na tej podstawie wybierzemy regułę, model albo połączenie obu metod. Ustalimy, ile kosztuje pomyłka i jak zmierzymy poprawę. Na końcu wskażemy osobę, która podpisze się pod wdrożeniem.

## Slajd 007 — Pojęcia i granice AI

Zacznijmy od słowa, którego wszyscy używamy. Kiedy producent mówi, że jego produkt wykorzystuje inteligencję, o jakiej zdolności konkretnie mówi? Sprawdźmy to na trzech prostych przykładach.

## Slajd 008 — Trzy pytania na początek

Kalkulator wykonuje rachunki szybciej ode mnie. Czy z tego wynika, że rozumie arytmetykę? Termostat utrzymuje zadaną temperaturę. Kto wyznaczył jego cel? Chatbot odpowiada płynnie. Co musiałbym sprawdzić, żeby powierzyć mu odpowiedź dla mojego klienta?

*[Pauza na odpowiedzi.]*

## Slajd 009 — Sztuczna inteligencja

Sztuczna inteligencja to dziedzina budowania systemów, które wykonują zadania wymagające wnioskowania, uczenia lub działania w złożonym otoczeniu. To definicja robocza. Ma nam pomóc rozpoznawać problemy, a nie rozstrzygać całą filozofię umysłu jednym zdaniem.

Kiedy telefon zamienia mowę na tekst, mamy zadanie percepcyjne. Kiedy program szuka trasy przy ograniczeniach czasu i kosztu, mamy problem planowania. Kiedy model tworzy odpowiedź, mamy zadanie językowe. W każdym przypadku coś innego znaczy poprawny wynik i inaczej trzeba zbierać dowody jego jakości.

Ważne jest także to, że AI nie musi się uczyć podczas działania. System może korzystać z wcześniej ustalonych reguł, przeszukiwać przestrzeń możliwości albo używać modelu wytrenowanego wiele tygodni wcześniej. Nazwa dziedziny nie mówi jeszcze, jaki mechanizm znajduje się w środku.

Słowo „inteligencja” łatwo przesuwa uwagę z zadania na domniemany podmiot. Zaczynamy wyobrażać sobie kogoś, kto rozumie całą sytuację. Tymczasem system może sprawnie przetwarzać jedną reprezentację problemu, nie mając dostępu do wielu okoliczności oczywistych dla człowieka. Dlatego najpierw nazywamy zadanie, dopiero potem oceniamy zakres zdolności.

Żeby uporządkować dalszą rozmowę, oddzielmy AI, uczenie maszynowe i uczenie głębokie.

## Slajd 010 — Cztery perspektywy na AI

Mamy tu dwie osie. Pierwsza rozróżnia sposób dochodzenia do wyniku i obserwowalne zachowanie. Druga rozróżnia podobieństwo do człowieka i racjonalność. W firmie możemy użyć tych kryteriów rozdzielnie. Agent może formułować odpowiedzi jak człowiek, a mimo to źle dobierać działania do celu procesu.

## Slajd 011 — AI, ML i deep learning

Uczenie maszynowe jest częścią sztucznej inteligencji, a uczenie głębokie jest częścią uczenia maszynowego. To pierwszy porządek. AI obejmuje również rozwiązania oparte na logice, regułach i planowaniu, które nie muszą dopasowywać parametrów do dużych zbiorów przykładów.

W uczeniu maszynowym budujemy procedurę, która na podstawie danych dopasowuje model. W uczeniu głębokim model ma postać wielowarstwowej sieci, a część potrzebnej reprezentacji również powstaje w treningu.

Ale są też inne osie podziału. NLP oznacza pracę z językiem, transformer oznacza architekturę, a uczenie nadzorowane opisuje sposób otrzymywania informacji zwrotnej. Generatywna AI opisuje rodzinę zadań związanych z tworzeniem danych. Tych pojęć nie należy ustawiać w jednej kolejce, jakby każde było następcą poprzedniego.

Pomylenie osi podziału prowadzi do zaskakująco praktycznych błędów. Ktoś pyta, czy lepszy będzie transformer, czy uczenie nadzorowane, choć transformer może być uczony nadzorowanie. To tak, jakby pytać, czy do przewozu wybieramy samochód, czy silnik elektryczny. Potrzebujemy osobno nazwać konstrukcję, sposób uczenia i zadanie.

Kiedy mamy już mapę pojęć, możemy zapytać, co właściwie chcemy nazywać inteligentnym zachowaniem.

## Slajd 012 — ANI, AGI i ASI

ANI to określenie inteligencji o ograniczonym zakresie: system radzi sobie z określonymi zadaniami i w określonych warunkach. Nie oznacza to, że musi wykonywać tylko jedną operację. Ważniejsze jest to, jak szeroko i jak niezawodnie potrafi przenosić umiejętności.

AGI nazywamy koncepcję szerokiej, elastycznej inteligencji ogólnej. Trudność polega na tym, że nie ma jednego powszechnie uzgodnionego kryterium, które zamknęłoby dyskusję. Jedni podkreślają zakres zadań, inni autonomię, uczenie nowych problemów albo porównanie z ludzką sprawnością.

Dlatego przy mocnej deklaracji o AGI zapytałbym najpierw o definicję operacyjną. Jakie zadania? W jakich warunkach? Z jakim dostępem do narzędzi? Jak często występują błędy? I jakie wyniki obaliłyby tę deklarację? Bez takich pytań spór łatwo staje się porównywaniem różnych znaczeń tego samego skrótu.

Szerokość kompetencji nie rozstrzyga świadomości ani statusu moralnego. Możemy dyskutować o bardzo zdolnym systemie, nie mając podstaw do przypisywania mu przeżyć. Możemy także badać możliwość świadomości, nie uznając jej za synonim wysokiego wyniku w testach. Oddzielenie tych pytań porządkuje całą debatę.

Zobaczmy teraz, jak te ambicje zmieniały się w historii AI.

## Slajd 013 — Ruchomy horyzont AI

Kiedy komputer zaczął wygrywać z mistrzami szachów, uznaliśmy to za wielki sprawdzian inteligencji. Dziś program szachowy jest zwykłym narzędziem treningowym. Podobną drogę przeszło rozpoznawanie pisma. W ocenie projektu warto opisać konkretną zdolność i jej warunki, bo sama etykieta AI zmienia znaczenie wraz z naszymi przyzwyczajeniami.

## Slajd 014 — Test tworzy obraz inteligencji

Wyobraźmy sobie system, który znakomicie rozwiązuje przygotowany egzamin. Zmieniamy jednak układ polecenia, dodajemy nieistotne zdanie albo prosimy o tę samą operację w nieznanej konwencji i wynik wyraźnie spada. Co właściwie zmierzyliśmy za pierwszym razem?

Możliwe są różne odpowiedzi. System mógł opanować prawdziwą umiejętność, lecz nie rozpoznać nowego opisu zadania. Mógł też wykorzystać regularność formatu. Mógł wreszcie znać bardzo podobne przykłady. Sam wynik nie pozwala odróżnić tych wyjaśnień.

Rzetelna ocena powinna więc zmieniać warunki w kontrolowany sposób. Sprawdzamy nowe przykłady, odmienne sformułowania i zadania wymagające transferu. Jeżeli interesuje nas samodzielne rozumowanie, nie wystarczy test, który można zdać dzięki powierzchownym wskazówkom. Ale również pojedyncza porażka po zmianie formatu nie dowodzi, że system nie ma żadnej przydatnej kompetencji.

Teraz zejdźmy jeszcze głębiej. Gdy test staje się celem rozwoju, zaczyna kształtować same systemy. Udoskonalamy to, co umiemy policzyć, a potem możemy uznać policzalne za pełną definicję wartości. Dotyczy to modeli, szkół i organizacji. Pytanie „czy system jest inteligentny?” warto wtedy zamienić na dokładniejsze: jakie zachowania nagradzamy, jakich nie zauważamy i jakie alternatywne wyjaśnienie pasuje do wyniku? Dopiero zestaw różnych dowodów daje prawo do szerszego wniosku.

Jest tu jeszcze jedna warstwa. Benchmark działa trochę jak instytucja przyznająca uznanie: decyduje, jaki rodzaj sukcesu stanie się widoczny. Jeżeli cała dziedzina optymalizuje się pod ten sam zestaw zadań, możemy otrzymać rzeczywisty postęp w mierzonej sprawności i jednocześnie coraz słabszą informację o pozostałych zdolnościach. Dlatego potrzebujemy nie tylko nowych wyników, lecz także nowych sposobów zadawania pytań. Dobry test powinien umieć zaskoczyć nasze przekonanie o systemie. Jeśli służy wyłącznie do potwierdzania wcześniej przyjętej opowieści, przestaje pomagać w odkrywaniu ograniczeń.

To prowadzi nas do rozróżnienia między sprawnością wyspecjalizowaną a inteligencją ogólną.

## Slajd 015 — Inteligencja i świadomość

Dotąd ocenialiśmy, co system potrafi zrobić. Teraz rozdzielimy trzy pytania. Co potrafi wykonać, co rozumie i czy czegokolwiek doświadcza? Każde z nich wymaga innych argumentów.

## Slajd 016 — Inteligencja ma wiele wymiarów

Sprawność w jednym zadaniu, elastyczność i rozumienie to różne własności. Człowiek może świetnie grać w szachy i słabo odnajdywać się w relacjach społecznych. System może dobrze rozpoznawać obrazy i nie umieć wyjaśnić, dlaczego określony błąd jest dla użytkownika dotkliwy.

Dlatego wynik testu trzeba czytać razem z opisem testu. Interesuje nas, czy przykłady były nowe, czy zmienił się sposób zadania pytania i czy system potrafi przenieść umiejętność do innego kontekstu. Płynna odpowiedź językowa także jest wynikiem określonego zadania, a nie automatycznym dowodem wszystkich pozostałych zdolności.

W materiałach o inteligencji spotykamy wiele podziałów, w tym edukacyjną teorię inteligencji wielorakich Gardnera. Możemy z nich korzystać jako inspiracji do myślenia o różnorodności zdolności. Nie należy jednak traktować takiej listy jako uzgodnionej budowy umysłu ani gotowej linijki do mierzenia AI.

Najtrudniej zauważyć zdolności, których nasz test w ogóle nie wymaga. Możemy więc pomylić brak dowodu z dowodem braku, a z drugiej strony rozciągnąć wąski sukces na cały system. Obie pomyłki wynikają z zapominania, że każdy pomiar wybiera fragment rzeczywistości.

Pierwsze pogłębienie dotyczy właśnie związku między testem i obrazem inteligencji.

## Slajd 017 — Chiński pokój i odpowiedź systemowa

Wyobraźmy sobie osobę, która odpowiada na pytania po chińsku, przestawiając znaki według instrukcji. Z zewnątrz odpowiedzi mogą wyglądać poprawnie, choć osoba nie zna języka. Searle pyta, skąd w tym układzie miałoby się wziąć rozumienie. Odpowiedź systemowa mówi, że pytanie trzeba zadać o cały układ, który obejmuje także instrukcje i pamięć. To spór o kryterium rozumienia.

## Slajd 018 — Inteligencja i świadomość

Inteligencję możemy badać przez wykonanie zadań, uczenie i adaptację. Świadomość, w znaczeniu subiektywnego doświadczenia, stawia inne pytanie: czy dla danego systemu w ogóle istnieje jakieś przeżywanie.

Wypowiedź „czuję smutek” sama tego nie rozstrzyga. Model może wytworzyć takie zdanie dzięki poznanym regularnościom języka. Z drugiej strony prosty argument, że system jest obliczeniem, nie zamyka automatycznie całej debaty filozoficznej o możliwych warunkach doświadczenia.

Nie mamy powszechnie uzgodnionego testu świadomości AI. Badacze proponują wskaźniki powiązane z teoriami świadomości, ale ich interpretacja pozostaje przedmiotem sporu. Dlatego będę ostrożny zarówno z pewnym przypisywaniem przeżyć, jak i z twierdzeniem, że sama forma rozmowy dostarcza rozstrzygającego dowodu w którąkolwiek stronę.

Trzeba również odróżniać doświadczenie od jego opisu, sprawność od motywacji oraz zdolność mówienia o sobie od samoświadomości w silnym sensie. Pojęcia te u ludzi są ze sobą powiązane, ale w systemach technicznych nie wolno automatycznie przenosić całego pakietu na podstawie jednego podobnego zachowania. To dyscyplina rozróżniania, a nie zakaz stawiania pytań.

Jest jednak coś, co możemy opisać bez rozstrzygania świadomości systemu: doświadczenie człowieka w relacji z nim.

## Slajd 019 — Poczucie relacji jest realne po stronie człowieka

System pamięta, jak lubimy być nazywani, reaguje ciepło i odpowiada wtedy, gdy potrzebujemy rozmowy. Użytkownik może poczuć bliskość. To uczucie po stronie człowieka jest rzeczywiste, nawet jeśli nie rozstrzygnęliśmy, co dzieje się po stronie systemu.

Nie należy ośmieszać tego doświadczenia. Jednocześnie nie powinniśmy traktować go jako dowodu wzajemnego przeżywania. Poczucie, że ktoś nas rozumie, może powstać dzięki trafnej odpowiedzi, dostępności i stylowi, który dobrze odpowiada naszym oczekiwaniom.

Pytanie projektowe brzmi: czy taka interakcja wspiera samodzielność użytkownika? Czy jasno pokazuje naturę systemu? Czy pozwala odejść bez wywoływania poczucia winy? Czy nie wykorzystuje rozpoznanej podatności po to, żeby przedłużać zależność? To kwestie, które można oceniać już teraz, niezależnie od wyniku filozoficznej debaty.

Najgłębsza asymetria dotyczy odpowiedzialności. Człowiek wnosi do relacji własną historię, wrażliwość i realne konsekwencje emocjonalne. Organizacja projektująca system może kształtować zachowanie interfejsu i czerpać korzyść z zaangażowania. Dlatego język bliskości powinien być oceniany także jako decyzja projektowa o wpływie na człowieka. Pytanie o uczucia maszyny nie powinno zasłaniać pytania o obowiązki ludzi, którzy udostępniają ją innym. Możemy nie mieć pewności co do świadomości systemu i jednocześnie mieć bardzo konkretne powody, żeby wymagać przejrzystości i unikania manipulacji.

Warto tu oddzielić autentyczność od wzajemności. Uczucie użytkownika może być autentyczne, ale nie daje samo przez się wiedzy o stanie drugiej strony. Ta luka nie unieważnia wartości pomocy. Umożliwia natomiast bardziej uczciwą ocenę relacji. Czy człowiek rozumie, jakie mechanizmy kształtują odpowiedź i jakie interesy stoją za dostępnością systemu? Czy kontakt pomaga mu lepiej działać również poza interfejsem? Takie pytania pozwalają mówić o bliskości bez ośmieszania doświadczenia i bez nadawania mu większej mocy dowodowej, niż rzeczywiście ma. Odpowiedzialny projekt respektuje emocje człowieka, zamiast wykorzystywać ich realność jako argument marketingowy.

Po tej refleksji wróćmy do innego znaczenia samodzielności: wykonywania zadań za pomocą narzędzi.

## Slajd 020 — Historia AI

Historia AI biegnie przez okresy szybkiego postępu i rozczarowania. Przy kolejnych datach zwróćmy uwagę na dwie rzeczy. Jaki pomysł był dostępny wcześniej i co dopiero później pozwoliło użyć go na dużą skalę?

## Slajd 021 — 1950 i 1956

W 1950 roku Alan Turing opublikował tekst „Computing Machinery and Intelligence”. Zamiast pozostawać przy sporze o samo słowo „myślenie”, zaproponował rozważenie gry w naśladownictwo. To przesunięcie uwagi w stronę zachowania, które możemy obserwować.

W 1955 roku John McCarthy, Marvin Minsky, Nathaniel Rochester i Claude Shannon przygotowali propozycję letniego projektu badawczego w Dartmouth. Spotkanie odbyło się latem 1956 roku i stało się jednym z symbolicznych początków AI jako nazwanej dziedziny.

Warto rozróżnić te daty. Maszyna Turinga należy do wcześniejszej pracy z 1936 roku. Gra w naśladownictwo pochodzi z 1950 roku. Propozycja Dartmouth powstała w 1955 roku, a sam projekt odbył się w 1956. Te rozróżnienia pokazują, że teoria obliczeń, pytania o inteligencję i organizacja programu badawczego nie pojawiły się jednocześnie.

U Turinga interesujący jest ruch metodologiczny: kiedy nie umiemy uzgodnić istoty zjawiska, próbujemy uzgodnić obserwowalny sprawdzian. Ten ruch bywa bardzo produktywny, ale pozostawia otwarte pytanie, ile z pierwotnego problemu zmieściło się w nowym teście. To napięcie powraca również w dzisiejszych benchmarkach.

Kolejny etap rozwoju mocno wiązał inteligencję z jawnym operowaniem symbolami.

## Slajd 022 — Symbole, reguły i zimy AI

Podejście symboliczne wychodziło z intuicji, że wiele rozumowań można opisać jako operacje na reprezentacjach i regułach. Jeżeli zapiszemy fakty oraz dopuszczalne kroki wnioskowania, komputer może poszukiwać rozwiązania w uporządkowany sposób.

Taki projekt potrafi działać bardzo dobrze w świecie o jasno określonych zasadach. Trudność rośnie, gdy trzeba zebrać wiedzę codzienną, radzić sobie z niekompletnością albo ciągle zmieniać reguły. Człowiek wykorzystuje ogromną liczbę oczywistości, których nawet nie zauważa, dopóki nie próbuje ich zapisać.

Okresy nazywane zimami AI obejmowały ograniczenie finansowania i rozczarowanie wcześniejszymi obietnicami. Nie oznaczały identycznego zatrzymania wszystkich badań. Pokazywały jednak, jak kosztowny jest rozdźwięk między efektownym przykładem i systemem, który ma niezawodnie działać poza przygotowanym otoczeniem.

Głębszym problemem jest koszt kompletności. Reguła może być przejrzysta, ale zbiór reguł nigdy nie obejmuje automatycznie wszystkiego, co ważne. Wyjaśnienie „system zrobił dokładnie to, co zapisaliśmy” nie wystarcza, jeśli pominęliśmy sytuację, która w praktyce była przewidywalna. To odpowiedzialność za granice opisu.

Uczenie z danych częściowo zmienia sposób budowania tego opisu, choć nie usuwa wszystkich jego ograniczeń.

## Slajd 023 — Uczenie reprezentacji

Sieci neuronowe nie powstały wczoraj ani dopiero w latach osiemdziesiątych. Perceptron Rosenblatta jest związany z pracami z końca lat pięćdziesiątych. W 1986 roku Rumelhart, Hinton i Williams opublikowali ważną pracę o uczeniu reprezentacji przez propagację błędu.

Nie chodziło wyłącznie o stworzenie bardziej złożonej funkcji. Istotna była możliwość takiego dopasowania warstw, żeby wewnętrzny zapis danych pomagał rozwiązać zadanie. Zamiast ręcznie ustalać wszystkie cechy, część struktury można było wyuczyć.

Równolegle rozwijały się metody statystyczne. Lata dziewięćdziesiąte to między innymi ważny okres rozwoju SVM. Nie należy więc opowiadać historii tak, jakby kolejne rodziny metod po prostu unieważniały wcześniejsze. Zmieniały się mocne strony, koszty i obszary, w których dane rozwiązanie było praktyczne.

Reprezentacja określa, które różnice są dla modelu widoczne. Uczenie reprezentacji przesuwa część tej decyzji do procedury treningowej. To ogromna siła, ale także źródło trudności: model może wyuczyć cechy przydatne do wyniku, których projektant wcale nie zamierzał traktować jako istotnych.

Nowsze przełomy połączyły te idee z większą skalą danych i obliczeń.

## Slajd 024 — 2012, 2017, lata 2020.

W 2012 roku AlexNet pokazał siłę głębokich sieci konwolucyjnych w rozpoznawaniu obrazów. Ten sukces połączył architekturę, duży zbiór danych i efektywne obliczenia na GPU. Był widocznym przełomem, ale korzystał z długiej historii wcześniejszych badań.

W 2017 roku praca „Attention Is All You Need” przedstawiła transformera. Mechanizm uwagi pomógł inaczej modelować zależności między elementami sekwencji i szerzej wykorzystać równoległe obliczenia podczas treningu. Późniejsze zastosowania wykroczyły daleko poza pierwotne zadanie tłumaczenia.

W latach dwudziestych modele generatywne i multimodalne trafiły do codziennego użycia na znacznie większą skalę. Dla wielu osób to był pierwszy kontakt z AI, z którą można prowadzić swobodną rozmowę. To ważna zmiana interfejsu: technologia stała się dostępna przez język, którego nie trzeba wcześniej uczyć się jak składni programu.

Gdy interfejsem staje się rozmowa, tracimy część sygnałów przypominających, że korzystamy z systemu technicznego. Nie widzimy formularza z ograniczoną liczbą pól. Możemy zapytać o wszystko, więc łatwo oczekiwać, że system równie dobrze zna wszystko. Zakres dopuszczalnych pytań jest jednak szerszy niż zakres wiarygodnych odpowiedzi.

Zatrzymajmy się na chwilę przy pytaniu, dlaczego idee czasem czekają na swój moment.

## Slajd 025 — Dlaczego przełom bywa spóźniony?

Wyobraźmy sobie pomysł, który jest teoretycznie sensowny, lecz na dostępnym sprzęcie wymaga miesięcy obliczeń i daje niestabilne wyniki. Trudno wtedy przekonać praktyków, że właśnie patrzą na przyszłość. Po zmianie infrastruktury ten sam kierunek może stać się nagle opłacalny.

Nie wystarczy jednak powiedzieć, że wszystko rozwiązuje większa skala. Dane, sprzęt, architektura i procedura treningu wzajemnie na siebie wpływają. Większy zbiór nie pomoże, jeśli opisuje niewłaściwy problem. Szybszy procesor nie naprawi błędnej etykiety. Dobre narzędzie pomiaru może natomiast ujawnić postęp, którego wcześniej nie umieliśmy dostrzec.

Dlatego oceniając metodę, pytam osobno o jej sens, aktualną wykonalność i warunki wdrożenia. Możliwe, że idea jest słaba. Możliwe też, że ograniczenie znajduje się gdzie indziej. Rozdzielenie tych wyjaśnień jest trudniejsze niż powiedzenie, że coś po prostu działa albo nie działa.

To pogłębienie dotyczy również sposobu tworzenia wiedzy. Sukces potrafi zmienić interpretację całej wcześniejszej historii: to, co wcześniej wyglądało jak ślepy zaułek, zaczyna wyglądać jak zapowiedź przełomu. Powinniśmy uważać na takie odczytywanie przeszłości od końca. Z dzisiejszej skuteczności nie wynika, że wszystkie dawne obietnice były uzasadnione. A z dawnych porażek nie wynika, że dzisiejszy sukces był niemożliwy. Historia pokazuje zależność wyniku od warunków, a nie prosty przepis na przyszłość.

Istnieje także wymiar instytucjonalny. Kierunek badań zależy od tego, jakie wyniki umiemy pokazać, jakie projekty otrzymują zasoby i jakie problemy są uznawane za ważne. Nie znaczy to, że skuteczność jest wyłącznie kwestią mody. Znaczy, że droga do sprawdzenia pomysłu wymaga realnych warunków. Możemy więc zapytać: które idee wyglądają dziś słabo dlatego, że są błędne, a które dlatego, że nie umiemy jeszcze uczciwie ich przetestować? Nie mamy automatycznej odpowiedzi. Mamy jednak powód, żeby odróżniać brak sukcesu w aktualnym układzie od dowodu zasadniczej niemożliwości.

Przejdźmy teraz do tego, co dokładnie znaczy uczenie modelu na podstawie danych.

## Slajd 026 — Uczenie maszynowe

Od tego miejsca skupimy się na regułach, które model wydobywa z przykładów. Zobaczymy, jak oddzielić dane do nauki od danych do oceny. To rozróżnienie decyduje, czy wynik z prezentacji dostawcy cokolwiek mówi o naszej przyszłej pracy.

## Slajd 027 — Programowanie i uczenie

Jeżeli chcę naliczać dziesięcioprocentowy rabat po przekroczeniu ustalonego progu, mogę napisać prostą regułę. Znam zasadę i wiem, jak przełożyć ją na instrukcję. Nowy zakup nie zmienia sposobu działania tej zasady.

Ze spamem jest trudniej. Nie umiem wypisać wszystkich przyszłych wiadomości ani wszystkich sposobów oszukiwania odbiorcy. Mogę natomiast zebrać przykłady, opisać oczekiwane wyniki i dopasować model, który wykorzysta regularności obecne w tych danych.

Nie oznacza to, że człowiek znika. Nadal wybiera cel, reprezentację, dane i sposób oceny. Zmienia się miejsce, w którym zapisujemy część reguły. Zamiast bezpośrednio określić każdy warunek, tworzymy procedurę, która wyznacza parametry na podstawie przykładów. Ostatecznie również model działa jako program.

W tym przesunięciu ukrywa się zmiana odpowiedzialności. Przy jawnej regule pytamy, kto ją napisał. Przy modelu trzeba zapytać także, kto wybrał dane i dlaczego uznał historyczne odpowiedzi za właściwy wzorzec. Automatyczne dopasowanie nie usuwa ludzkich decyzji. Część z nich przenosi wcześniej, do konstrukcji eksperymentu.

Teraz oddzielmy sam model od treningu i od codziennego używania go.

## Slajd 028 — Uczenie jako T, E i P

T oznacza zadanie. E oznacza doświadczenie, z którego system się uczy. P oznacza miarę, według której stwierdzamy poprawę. Gdy ktoś mówi mi, że model się nauczył, pytam o wszystkie trzy elementy. Zastosujmy ten zapis do ofert handlowych.

## Slajd 029 — Czego system ma się nauczyć?

Nasze zadanie brzmi: przed wysłaniem oferty oszacować szansę jej wygrania. Przykłady weźmiemy z zamkniętych spraw, bo znamy ich rozstrzygnięcia. Status wygranej jest etykietą. W wejściu modelu mogą się znaleźć tylko informacje dostępne wcześniej, na przykład zakres i przygotowana cena. Trafność rankingu powie nam, czy model sensownie porządkuje oferty. Marża powie, czy zmiana kolejności pracy handlowców przynosi wartość.

## Slajd 030 — Model, trening, inferencja

Model jest strukturą obliczeń wraz z parametrami, które określają jej działanie. Trening to proces zmieniania tych parametrów na podstawie przyjętego celu. Inferencja to użycie modelu do nowego przypadku.

Najprościej zobaczyć to na klasyfikatorze spamu. Podczas treningu pokazujemy przykłady i poprawiamy parametry. Po wdrożeniu nowa wiadomość przechodzi przez gotowy model, który wyznacza wynik. Sama ta operacja nie musi powodować żadnej zmiany wag.

Podobnie w rozmowie z modelem językowym. Jeżeli podam informację na początku rozmowy, model może uwzględnić ją w odpowiedzi dzięki kontekstowi. Nie wynika z tego, że właśnie trwale przebudował swoje parametry. Pamięć aplikacji, wyszukanie dokumentu, kontekst rozmowy i aktualizacja wag to różne mechanizmy, choć z perspektywy użytkownika mogą wyglądać podobnie.

To rozróżnienie ma praktyczny skutek dla zaufania. Jeżeli system raz poprawił odpowiedź po uwadze, nie możemy automatycznie zakładać, że jutro zrobi to samo w nowej rozmowie. Trzeba wiedzieć, gdzie została zapisana korekta i czy w ogóle będzie dostępna w następnym użyciu. Pozorna ciągłość rozmowy może ukrywać brak ciągłości uczenia.

Sposób treningu zależy od tego, skąd bierze się informacja, co model powinien poprawić.

## Slajd 031 — Dane i cechy

Cechy są informacjami, na podstawie których model może odróżniać przypadki. W danych o zamówieniu mogą to być godzina, wartość, historia i sposób dostawy. Nie każda dostępna kolumna powinna jednak automatycznie trafić do modelu.

Najpierw pytamy o jakość pomiaru i moment dostępności. Jeżeli status reklamacji poznajemy dopiero po jej rozstrzygnięciu, nie możemy używać go do przewidywania decyzji w chwili zgłoszenia. Sprawdzamy również braki danych i znaczenie skali. W części algorytmów duża skala jednej cechy może zdominować obliczane odległości.

Dopasowanie skalowania, uzupełniania braków i wyboru cech powinno odbywać się na zbiorze treningowym. Użycie informacji ze zbioru testowego nawet na etapie przygotowania może zafałszować ocenę. Cały proces przetwarzania danych jest częścią uczonego rozwiązania.

Brak wartości także może coś komunikować. Badanie nie zostało wykonane, bo nie było potrzebne, bo nie było dostępne albo dlatego, że ktoś podjął wcześniejszą decyzję. Mechaniczne wstawienie średniej może ukryć różne procesy. Zanim poprawimy „brudne dane”, warto zrozumieć, jaka historia stoi za ich niekompletnością.

Następny krok to rozdzielenie danych tak, żeby test faktycznie sprawdzał nową sytuację.

## Slajd 032 — Trening, walidacja i test

Zbiór treningowy służy dopasowaniu parametrów. Zbiór walidacyjny pomaga wybierać ustawienia i porównywać warianty. Zbiór testowy ma ocenić rozwiązanie, którego kształt już ustaliliśmy.

Jeżeli po każdym spojrzeniu na test zmieniamy model, test przestaje być niezależnym sprawdzianem. Informacja o jego wynikach zaczyna wpływać na wybór rozwiązania. Możemy nieświadomie dopasować się również do tego zbioru, choć nigdy nie użyliśmy go bezpośrednio w obliczaniu gradientu.

Sam losowy podział nie zawsze wystarcza. Gdy przewidujemy przyszłość, musimy respektować czas. Gdy mamy wiele zdjęć tej samej osoby, trzeba uwzględnić jej tożsamość. Gdy system ma pracować w nowej placówce, warto sprawdzić transfer między placówkami. Dobry podział powinien odzwierciedlać rzeczywisty rodzaj nowości, z którym spotkamy się po wdrożeniu.

Test jest małą symulacją przyszłego spotkania ze światem. Jeśli źle zdefiniujemy to spotkanie, nawet idealna procedura liczenia metryki odpowie na niewłaściwe pytanie. Dlatego poprawność eksperymentu zaczyna się wcześniej niż przy wyborze miary jakości: zaczyna się od ustalenia, co ma znaczyć „nowy przypadek”.

Teraz zobaczmy, jak model może nauczyć się za mało albo zbyt mocno dopasować do treningu.

## Slajd 033 — Niedouczenie i przeuczenie

Niedouczenie oznacza, że model nie wykorzystuje dostatecznie ważnych regularności. Może być zbyt prosty, źle reprezentować dane albo nie przejść wystarczająco skutecznego treningu. Wynik pozostaje wtedy słaby również dla przykładów treningowych.

Przeuczenie polega na nadmiernym dopasowaniu do własności zbioru treningowego, które nie przenoszą się dobrze na nowe dane. Błąd treningowy może maleć, podczas gdy wynik walidacyjny się pogarsza. Model znajduje sposób, żeby coraz lepiej radzić sobie z pamiętanymi przykładami.

Pomagać mogą regularyzacja, dodatkowe dane i odpowiednia kontrola treningu, na przykład wcześniejsze zatrzymanie. Nie są to jednak magiczne lekarstwa. Podobny obraz słabych wyników może wynikać z błędnych etykiet, złego podziału albo zmiany warunków. Najpierw diagnozujemy przyczynę, potem wybieramy interwencję.

Uczenie wymaga kompromisu między wrażliwością na regularność a wrażliwością na przypadek. Jednak prosty obraz „mniejszy model dobry, większy model zły” bywa zbyt ubogi dla współczesnych sieci. Dlatego zamiast oceniać model po liczbie parametrów, badamy jego zachowanie na właściwie zbudowanych danych walidacyjnych i testowych.

Szczególnie podstępnym źródłem pozornego sukcesu jest przeciek informacji.

## Slajd 034 — Spadek gradientu

Na tym rysunku wysokość oznacza stratę, a położenie zależy od dwóch poglądowych parametrów. Gradient wskazuje kierunek najszybszego lokalnego wzrostu straty. Robimy krok w przeciwną stronę. Za duży krok może przestrzelić obszar niskiej straty, a za mały wydłuża trening. Rzeczywiste modele robią to w znacznie większej liczbie wymiarów.

## Slajd 035 — Przeciek potrafi udawać inteligencję

Wyobraźmy sobie zbiór zdjęć medycznych. Każdy pacjent ma kilka obrazów. Dzielimy wszystkie pliki losowo i otrzymujemy bardzo dobry wynik. Problem polega na tym, że obrazy tej samej osoby mogły trafić zarówno do treningu, jak i do testu.

Model może wtedy wykorzystać sygnały związane z pacjentem, aparatem albo sposobem wykonania badania. To nie musi być świadome rozpoznawanie osoby w ludzkim sensie. Wystarczy regularność, która pomaga odgadnąć etykietę. Test przestaje sprawdzać dokładnie to, co obiecujemy, czyli działanie wobec nowego pacjenta.

Ten sam mechanizm pojawia się poza medycyną. Duplikaty dokumentów trafiają po obu stronach podziału. Dane o skutkach przyszłego zdarzenia wchodzą do cech użytych do jego prognozowania. Wstępne przetwarzanie korzysta z całego zbioru. Każdy taki przeciek może uczynić wynik znacznie bardziej optymistycznym.

Najgłębsza trudność polega na tym, że model nie odróżnia wskazówki właściwej od niewłaściwej według naszej intencji. Jeśli informacja pomaga obniżyć stratę, procedura może ją wykorzystać. Badacz może więc nieświadomie nagrodzić system za rozwiązanie prostszego zadania niż deklarowane. Uczciwość eksperymentu nie wymaga od modelu charakteru. Wymaga od nas konstrukcji, która nie oferuje skrótu. Zanim zachwycimy się inteligencją rozwiązania, powinniśmy zapytać, jaka alternatywna droga mogła prowadzić do tego wyniku.

Najciekawsze jest to, że nikt nie musi chcieć oszukiwać. Zespół może uczciwie stosować znaną procedurę i przeoczyć związek między plikami. Dlatego krytyczna kontrola eksperymentu powinna badać mechanizm, a nie domyślać się złych intencji. Warto pytać: jaką wiedzę ma system w teście, której nie będzie miał przy nowej decyzji? Kiedy tę informację poznaliśmy? Czy powiązania między obserwacjami naruszają założoną niezależność? Takie pytania potrafią obniżyć imponujący wynik, a jednocześnie zwiększyć prawdziwą wartość projektu, bo usuwają fałszywe poczucie bezpieczeństwa.

Załóżmy teraz, że podział jest poprawny. Nadal musimy wybrać, co dokładnie uznamy za dobry rezultat.

## Slajd 036 — Metryki i koszt błędu

Metryka jest sposobem podsumowania wyniku. Precision mówi, jaka część przypadków wskazanych jako pozytywne rzeczywiście do nich należy. Recall mówi, jaką część wszystkich rzeczywistych przypadków udało się znaleźć. Te pytania brzmią podobnie, ale opisują inne błędy.

System wykrywający usterki może wskazywać bardzo mało maszyn, lecz niemal zawsze trafnie. Będzie miał wysoką precyzję, ale może przeoczyć wiele awarii. Inny może znaleźć prawie wszystkie awarie, zasypując serwis fałszywymi alarmami. Bez znajomości kosztów nie da się wybrać właściwego kompromisu.

W prognozowaniu liczbowym MAE opisuje przeciętną bezwzględną wielkość pomyłki. Nawet ta prosta liczba wymaga rozbicia na warunki i grupy. Dobry wynik średni może współistnieć z bardzo złym działaniem w rzadkiej, szczególnie ważnej sytuacji.

Metryka staje się decyzją o tym, które błędy zobaczymy razem, a które znikną w podsumowaniu. Nie każda metryka wprost przelicza koszt, dlatego potrzebujemy dodatkowo opisu skutków. W organizacji warto ustalić, czy liczba służy badaniu modelu, porównaniu wariantów czy decyzji o wdrożeniu. To różne zastosowania tego samego pomiaru.

Zobaczmy przykład, w którym bardzo wysoka trafność ukrywa całkowite niepowodzenie ważnego zadania.

## Slajd 037 — 99% trafności może oznaczać zero wykryć

Mamy tysiąc transakcji i wiemy, że dziesięć jest oszustwami. System każdą transakcję uznaje za poprawną. W dziewięciuset dziewięćdziesięciu przypadkach ma rację. Jego trafność wynosi dziewięćdziesiąt dziewięć procent.

Brzmi świetnie, dopóki nie zapytamy, ile oszustw znalazł. Nie znalazł żadnego. Recall dla oszustw wynosi zero. System uzyskał wysoki wynik dzięki dominacji poprawnych transakcji, a nie dzięki zdolności wykrywania nadużyć.

To przykład skonstruowany do wyjaśnienia mechanizmu, nie opis rzeczywistego produktu. W praktyce chcielibyśmy zobaczyć również liczbę fałszywych alarmów, skuteczność wobec różnych rodzajów oszustwa i obciążenie zespołu. Precision nie ma tu zwykłej interpretacji, bo system nie wskazał ani jednego pozytywnego przypadku. Nie powinniśmy przyznawać mu w zamian fantastycznego wyniku innej metryki.

Najbardziej niebezpieczne liczby bywają poprawnie policzone. Problem nie zawsze znajduje się w rachunku. Czasem znajduje się w pytaniu, na które liczba odpowiada. Możemy więc nie kłamać w prezentacji wyników i jednocześnie stworzyć bardzo mylące wyobrażenie jakości. Odpowiedzialność wymaga ujawnienia sensu mianownika, proporcji klas i konsekwencji błędów. Wysoka średnia może uspokajać dokładnie tam, gdzie powinna uruchomić bardziej szczegółowe badanie. To lekcja szersza niż AI: atrakcyjny wskaźnik trzeba zawsze odnieść do zadania, dla którego miał być dowodem.

Warto teraz pomyśleć o osobie należącej do rzadkiej kategorii. Dla średniej jest niewielką częścią mianownika. Dla niej własny błąd może być całym doświadczeniem kontaktu z systemem. To nie znaczy, że średnie są bezużyteczne. Znaczy, że nie powinny być jedynym poziomem opisu, gdy konsekwencje nierówno rozkładają się między ludźmi. Pytanie o jakość staje się pytaniem o dystrybucję jakości. Kto otrzymuje dobre działanie, kto dostaje większość pomyłek i czy potrafimy to zobaczyć przed wdrożeniem? Właśnie tutaj metodologia pomiaru zaczyna spotykać się ze sprawiedliwością.

Kolejną decyzją jest próg, przy którym ocenę modelu zamieniamy w realne działanie.

## Slajd 038 — Próg decyzji i niepewność

Model może zwrócić ocenę ryzyka, a organizacja musi zdecydować, przy jakim poziomie uruchomi alarm. To próg decyzji. Zmieniając próg, możemy przy tych samych ocenach modelu otrzymać inny kompromis między wykrywalnością i fałszywymi alarmami.

Trzeba też zbadać kalibrację. Jeśli przypadki z oceną około 0,8 rzeczywiście kończą się zdarzeniem w przybliżeniu w ośmiu na dziesięć podobnych sytuacji, mamy podstawę do takiej interpretacji oceny. To własność empiryczna, a nie automatyczny skutek pokazania liczby z przecinkiem.

Warto przewidzieć możliwość przekazania trudnego przypadku człowiekowi. Ale ta opcja musi mieć procedurę: kto przejmie sprawę, jakie informacje otrzyma i ile będzie miał czasu. Sam napis „decyduje człowiek” nie tworzy zdolności do sensownego rozstrzygnięcia.

Niepewność może wynikać z niejednoznaczności danych albo z braków wiedzy modelu. To różne problemy. Dodatkowy pomiar może pomóc w pierwszym przypadku, a trening na nowych warunkach w drugim. W modelu językowym zdanie „jestem pewny” nie jest samo w sobie skalibrowanym pomiarem. Styl pewności trzeba oddzielić od dowodu.

Nawet dobrze skalibrowana prognoza nie odpowiada jeszcze na wszystkie pytania o przyczyny i zmianę świata.

## Slajd 039 — Próg alarmu zmienia koszt kontroli

Policzmy koszt obu progów na tej samej próbce. W wariancie A osiem przeoczeń daje cztery tysiące złotych, a dwadzieścia zbędnych kontroli dodaje sześćset. Razem cztery tysiące sześćset. W wariancie B trzy przeoczenia kosztują półtora tysiąca, a sześćdziesiąt zbędnych kontroli tysiąc osiemset. Razem trzy tysiące trzysta. Zyskujemy tysiąc trzysta złotych pod warunkiem, że zespół obsłuży czterdzieści dodatkowych kontroli w przyjętym koszcie.

## Slajd 040 — Prognoza nie odpowiada na pytanie „co zmienić?”

Załóżmy, że w zebranych danych osoby z parasolem częściej mają mokre buty. Model może wykorzystać parasol jako wskazówkę i skutecznie przewidywać stan obuwia. Czy wynika z tego, że odbierając ludziom parasole, osuszymy im buty?

Nie. Deszcz może być wspólną przyczyną noszenia parasola i mokrych butów. Związek obserwacyjny pomaga przewidywać, ale nie określa automatycznie skutku interwencji. W dodatku parasol może częściowo chronić przed zamoknięciem, choć w danych nadal będzie kojarzył się z deszczem.

To analogia, która pokazuje ograniczenie wielu zastosowań predykcyjnych. Model przewidujący, kto odniesie sukces, nie mówi od razu, jakie działanie spowoduje sukces. Do pytań przyczynowych potrzebujemy odpowiedniego projektu badania, wiedzy dziedzinowej i jawnych założeń.

Najgłębsze przesunięcie następuje wtedy, gdy prognozę zaczynamy traktować jak instrukcję naprawy świata. System wskazuje cechę związaną z ryzykiem, a organizacja próbuje ją usunąć, choć cecha może być tylko śladem innego procesu. Można wtedy poprawić wskaźnik bez zmiany przyczyny, a nawet pogorszyć sytuację. Dlatego przed interwencją pytamy, czy zmieniamy mechanizm, czy jedynie jego oznakę. Przyczynowość jest próbą odpowiedzi na pytanie, co pozostanie prawdziwe, gdy sami zaczniemy ingerować w układ.

Do tego dochodzi reakcja świata na samą interwencję. Gdy zaczniemy używać prognozy do przyznawania zasobów, ludzie zmienią zachowanie, a warunki mogą przestać przypominać historię. Wcześniej trafna zależność może osłabnąć. Nie oznacza to, że przewidywanie było bezwartościowe, lecz że stało się elementem nowego układu. Dlatego model przeznaczony do decyzji powinien być oceniany także po wdrożeniu. Pytamy nie tylko, czy zna dawny świat, ale również, czy sposób jego używania nie zmienia reguł, na których opierał się sukces. Prognoza może utracić podstawę właśnie dlatego, że zaczęliśmy na nią reagować.

Sprawdźmy teraz, czy potrafimy rozpoznać rodzaj uczenia po opisie zadania.

## Slajd 041 — Rodziny modeli

Nie istnieje jeden model najlepszy dla każdego problemu. Prosta regresja może być bardzo dobrym punktem odniesienia, zwłaszcza gdy chcemy szybko zrozumieć zależności. Regresja logistyczna, mimo nazwy, często służy klasyfikacji. To kolejny przykład, że nazwy metod i nazwy zadań trzeba rozróżniać.

Drzewa, lasy i boosting są ważną rodziną rozwiązań dla danych tabelarycznych. k-NN korzysta z podobieństwa do znanych przypadków, a SVM wyznacza określone granice decyzji. Sieci neuronowe pozwalają elastycznie uczyć reprezentacje i złożone zależności.

Praktyczna decyzja zależy od ilości danych, jakości cech, wymaganego czasu odpowiedzi, zasobów oraz kosztu utrzymania. Dlatego zaczynam od baseline, czyli prostego rozwiązania odniesienia. Jeśli złożony model nie daje wyraźnej korzyści w uczciwym teście, sama jego nowoczesność nie uzasadnia wdrożenia.

Złożoność stwarza także zobowiązania organizacyjne. Ktoś musi umieć zdiagnozować błąd, odtworzyć trening i utrzymywać system. Dodatkowy ułamek jakości może być cenny, ale może również zostać pochłonięty przez koszty i kruchość rozwiązania. Najlepszy model w tabeli wyników nie zawsze jest najlepszym elementem całego procesu.

Zanim dopasujemy którykolwiek model, trzeba przyjrzeć się temu, co nazywamy danymi i cechami.

## Slajd 042 — Założenia, kompresja i wybór modelu

Każda metoda ułatwia znalezienie pewnych zależności. Na przykład model liniowy zakłada prostszą postać zależności niż głęboka sieć. Zasada minimalnej długości opisu premiuje zwięzły opis modelu razem z tym, czego sam model nie wyjaśnia w danych. Twierdzenia no free lunch zależą od tego, po jakich problemach uśredniamy wynik. W projekcie sprawdzamy przewagę na problemach, które faktycznie występują u nas.

## Slajd 043 — Rodzaje uczenia

W kolejnych przykładach będziemy pytać o źródło sygnału uczącego. Czy ktoś oznaczył poprawne odpowiedzi? Czy model sam wydobywa wzorce z danych? Czy dostaje ocenę skutku własnego działania?

## Slajd 044 — Pięć źródeł sygnału uczenia

Rodzaje uczenia najłatwiej uporządkować według źródła sygnału. W uczeniu nadzorowanym znamy oczekiwane odpowiedzi dla przykładów. W nienadzorowanym szukamy struktury bez gotowych etykiet zadania. W półnadzorowanym łączymy niewielką liczbę etykiet z większą liczbą danych bez nich.

Uczenie samonadzorowane tworzy cel z samych danych. Możemy ukryć fragment tekstu i poprosić model o jego przewidzenie. W uczeniu ze wzmocnieniem agent wybiera działania, obserwuje konsekwencje i otrzymuje nagrody związane z przebiegiem zadania.

To nie są zawsze rozłączne szuflady. Ten sam model może najpierw przejść trening samonadzorowany, potem nadzorowane dostrojenie, a następnie dodatkową optymalizację z sygnałem nagrody. Pytanie o rodzaj uczenia nie zastępuje więc pytania o cały proces budowania systemu.

Wspólny mianownik brzmi: system poprawia coś, co umiemy mu wskazać w danej procedurze. Największa trudność często nie polega na szybkości tej poprawy, lecz na zgodności technicznego sygnału z tym, co naprawdę chcieliśmy osiągnąć. Model może wiernie realizować cel treningowy i rozminąć się z ludzką intencją.

Zanim omówimy kolejne metody, przyjrzyjmy się temu, co ukrywa zwykła etykieta.

## Slajd 045 — Etykieta zawiera czyjąś definicję świata

Załóżmy, że budujemy model rozpoznający dobrych kandydatów do pracy. Zbieramy dawne CV i jako pozytywne przykłady oznaczamy osoby zatrudnione przez firmę. Wydaje się, że zadanie jest już gotowe. Ale czy etykieta „zatrudniony” rzeczywiście oznacza „dobry pracownik”?

Może oznaczać kogoś skutecznego. Może też oznaczać osobę podobną do poprzednich pracowników, dobrze ocenioną przez konkretnego rekrutera albo dostępną w dogodnym terminie. Model nie dostaje dostępu do naszej intencji poza tym, co zapisaliśmy w danych i funkcji celu.

Jeżeli wytrenujemy go bardzo skutecznie, może odtworzyć proces dawnych wyborów wraz z jego ograniczeniami. Wysoki wynik wobec historycznych etykiet pokaże wtedy zgodność z historią. Nie rozstrzygnie samodzielnie, czy historia była sprawiedliwa i czy stanowi dobry wzorzec dla przyszłości.

Zejdźmy poziom niżej: etykieta jest sposobem zdefiniowania rzeczywistości na potrzeby obliczeń. Wybierając ją, ustalamy, co zostanie zauważone, co pominięte i jakie rozróżnienia model będzie utrwalał. Etykieta „pacjent wymagający pomocy” może oznaczać rzeczywistą potrzebę albo dotychczasowy koszt leczenia, który zależy również od dostępu do opieki. To hipotetyczne rozróżnienie pokazuje mechanizm problemu. Przed pytaniem „jak dobrze przewidujemy?” powinno pojawić się pytanie „co dokładnie uznaliśmy za odpowiedź i dlaczego?”. Architektura nie może sama naprawić błędnego znaczenia celu.

W rekrutacji dochodzi problem niewidocznej odpowiedzi. Wiemy coś o wynikach osób zatrudnionych, ale zwykle nie wiemy, jak poradziłyby sobie osoby odrzucone, gdyby otrzymały porównywalną szansę. Historia nie jest więc pełnym eksperymentem, w którym każdą możliwość sprawdzono. Zawiera skutki wcześniejszej selekcji. Jeżeli zapomnimy o tej luce, możemy uznać brak zaobserwowanego sukcesu za dowód braku potencjału. To przykład szerszej zasady: dane mówią także o tym, komu pozwoliliśmy pojawić się w obserwacji. Model nie odzyska automatycznie historii, której nigdy nie zebraliśmy.

Na tej podstawie łatwiej zrozumiemy siłę i ograniczenia uczenia nadzorowanego.

## Slajd 046 — Uczenie nadzorowane

W uczeniu nadzorowanym przykład wejściowy ma przypisany oczekiwany wynik. Dla wiadomości może to być kategoria „spam” albo „poprawna”. Dla mieszkania może to być cena, a dla obrazu opis obecnych na nim obiektów.

Model oblicza przewidywanie, porównuje je z celem i na tej podstawie zmienia parametry. Powtarzamy proces dla wielu przykładów. Nie chodzi o to, żeby po prostu zapamiętał odpowiedzi. Chcemy, żeby wykorzystał zależności pomagające rozpoznać także nową wiadomość.

Dlatego potrzebujemy danych, których nie użyjemy do dopasowania. To na nich sprawdzimy, czy model przenosi umiejętność poza znane przykłady. Jeśli nowe dane pochodzą z innych warunków, trudność może wzrosnąć. Klasyfikator uczony na dawnych wiadomościach może słabiej rozpoznawać nową formę oszustwa.

Nadzór nie oznacza, że człowiek patrzy na każdą operację podczas treningu. Oznacza dostępność odpowiedzi służących jako punkt odniesienia. Ten punkt odniesienia sam może być omylny. W pewnych zadaniach eksperci nie zgadzają się co do etykiety, więc sensowna ocena modelu musi uwzględniać także niepewność ludzkiego wzorca.

Dwa podstawowe zadania nadzorowane to klasyfikacja i regresja. Zacznijmy od kategorii.

## Slajd 047 — Klasyfikacja

Klasyfikacja polega na przypisaniu przypadku do kategorii albo wyznaczeniu ocen, na podstawie których podejmiemy taki wybór. Wiadomość może być spamem, dokument może dotyczyć reklamacji, a zdjęcie może przedstawiać określony typ usterki.

Musimy jednak najpierw ustalić, jak wyglądają kategorie. Czasem wybieramy jedną z dwóch odpowiedzi, czasem jedną z wielu, a czasem kilka naraz. Dokument może jednocześnie dotyczyć umowy, rozliczenia i danych osobowych. Wymuszenie jednej etykiety byłoby wtedy uproszczeniem samego zadania.

Model może zwrócić także liczbę, na przykład 0,9 dla określonej kategorii. Taka liczba nie zawsze od razu oznacza, że dziewięć na dziesięć podobnych odpowiedzi będzie poprawnych. Tę własność trzeba sprawdzić. Służy do tego ocena kalibracji, do której jeszcze wrócimy.

Kategorie organizują późniejsze działanie. Gdy system przypisze sprawę do niewłaściwej szuflady, może uruchomić zły proces, nawet jeśli sama etykieta wydaje się drobnym błędem. Dlatego sens klasyfikacji rozumiemy dopiero wtedy, gdy znamy konsekwencje przypisania: kto dostanie sprawę, jaki termin zacznie biec i czy pomyłkę można naprawić.

W regresji zamiast kategorii przewidujemy wielkość liczbową.

## Slajd 048 — Regresja

Regresja odpowiada na pytanie o wartość liczbową. Możemy przewidywać zużycie energii, czas dostawy albo poziom drgań maszyny. Nie chodzi przy tym wyłącznie o regresję liniową. To nazwa rodzaju zadania, które mogą rozwiązywać różne modele.

W prognozie czasu dostawy musimy określić moment przewidywania. Co wiemy przy przyjęciu zamówienia, a co dopiero po wyjeździe samochodu? Model wykorzystujący informację dostępną później może wyglądać znakomicie w eksperymencie i być bezużyteczny w chwili realnej decyzji.

Ważne jest również znaczenie błędu. Pomyłka o dziesięć minut może być nieistotna w jednym procesie i poważna w innym. Średni błąd nie pokaże też automatycznie, czy system szczególnie źle działa w nocy, przy złej pogodzie albo dla odległych miejscowości.

Prognoza jest zawsze warunkowa: dotyczy określonego horyzontu i dostępnej informacji. Liczba pozbawiona tego kontekstu udaje większą pewność, niż rzeczywiście mamy. Czasem uczciwszym wynikiem będzie przedział i informacja o ograniczeniach niż jedna bardzo precyzyjnie wyglądająca wartość. Precyzja zapisu nie gwarantuje precyzji wiedzy.

Teraz sprawdźmy, co można zrobić wtedy, gdy nie mamy gotowych odpowiedzi dla przykładów.

## Slajd 049 — Uczenie nienadzorowane

W uczeniu nienadzorowanym nie dostarczamy gotowych etykiet zadania. Szukamy regularności w danych: podobnych przypadków, prostszej reprezentacji albo obserwacji nietypowych. Możemy na przykład próbować rozpoznać powtarzające się sposoby korzystania z usługi.

To jednak nie oznacza, że algorytm działa bez założeń. Wybieramy cechy, sposób ich przeskalowania i kryterium podobieństwa. Często wybieramy także liczbę grup albo inne ustawienia wpływające na wynik. Inny opis danych może ujawnić inny porządek.

Również anomalia wymaga ostrożnej interpretacji. Obserwacja rzadka może oznaczać awarię, ale może być poprawnym, wyjątkowym przypadkiem. Samo odstępstwo od typowego wzorca nie dostarcza jeszcze diagnozy jego przyczyny. Wykrycie nietypowości jest początkiem pytania, co się wydarzyło.

Brak etykiet nie usuwa problemu znaczenia. Przenosi go do interpretacji wyniku. Model może znaleźć bardzo wyraźny wzorzec, który odpowiada sposobowi pomiaru, a nie interesującemu nas zjawisku. Dlatego pytamy, czy struktura jest stabilna, czy ma sens dziedzinowy i czy pomaga rozwiązać konkretne zadanie.

Dwie ważne rodziny takich operacji to grupowanie oraz redukcja wymiaru.

## Slajd 050 — Klastry i reprezentacje

Grupowanie łączy obserwacje uznane za podobne. Jeśli opiszę klientów częstotliwością zakupów, kwotą i rodzajem produktów, mogę uzyskać pewne segmenty zachowań. Zmieniając opis, mogę otrzymać inny, równie sensowny podział.

Redukcja wymiaru rozwiązuje trochę inny problem. Gdy mamy wiele cech, próbujemy zapisać dane za pomocą mniejszej reprezentacji, zachowując wybrane własności. PCA szuka określonych kierunków zmienności. Autoenkoder uczy się reprezentacji związanej z odtwarzaniem danych. Te metody nie muszą zachowywać dokładnie tego samego.

Wizualizacja dwóch wymiarów jest przydatna, ale może być zdradliwa. Widzimy na ekranie wyraźne wyspy i łatwo uznać je za naturalne, ostre kategorie. Tymczasem część relacji mogła zmienić się w samym procesie sprowadzenia danych do płaskiego obrazu.

Każda mapa coś zachowuje i coś poświęca. Mapa metra pomaga się przesiadać, choć nie pokazuje wiernie wszystkich odległości. Podobnie reprezentację modelu oceniamy względem celu. Pytanie „czy ta mapa jest prawdziwa?” potrzebuje dopowiedzenia: prawdziwa pod jakim względem i przydatna do jakiej decyzji?

W następnym pogłębieniu przyjrzymy się temu, jak narzędzie współtworzy odkrywaną strukturę.

## Slajd 051 — Odkryta struktura zależy od narzędzia

Proszę wyobrazić sobie tę samą grupę ludzi. Raz dzielimy ją według dochodu, raz według gustu muzycznego, a raz według godzin największej aktywności. Za każdym razem otrzymamy inny porządek. Żaden nie musi być absurdalny, ale każdy odpowiada na inne pytanie.

Algorytm grupujący działa w świecie takich wyborów. Nie zaczyna od pełnego sensu ludzkich podobieństw. Dostaje reprezentację i kryterium. Jeśli podobieństwo policzymy na podstawie innych cech, możemy otrzymać inny wynik. Nawet skalowanie pojedynczej cechy może zmienić jej wpływ na odległość.

Z tego powodu nie powiedziałbym bez zastrzeżeń, że model odkrył prawdziwe typy klientów. Powiedziałbym, że przy określonym opisie danych znalazł pewien podział, który trzeba teraz ocenić pod względem użyteczności i stabilności. To skromniejsze zdanie, ale pozwala dokładnie sprawdzić, co rzeczywiście osiągnęliśmy.

Głębsze niebezpieczeństwo zaczyna się wtedy, gdy roboczą kategorię uznajemy za istotę człowieka. Segment powstały dla kampanii marketingowej zaczyna funkcjonować jak trwała tożsamość. Organizacja zmienia sposób obsługi tych osób, a ich zachowania stają się odpowiedzią na ten sposób traktowania. Podział może się wtedy utrwalać również dlatego, że zaczęliśmy według niego działać. Kategoria nie tylko opisuje rzeczywistość, lecz może uczestniczyć w jej przekształcaniu. Właśnie dlatego trzeba pamiętać, po co ją utworzono i gdzie kończy się jej uzasadnienie.

Można to zobaczyć jeszcze inaczej. Nazwa segmentu dodana przez analityka bywa bogatsza niż sam wynik obliczeń. Algorytm znalazł grupę podobnych wektorów, a organizacja nazywa ją „klientami nieodpowiedzialnymi”. W tym jednym kroku przechodzimy od geometrii do oceny charakteru. Ten wniosek wymaga osobnego uzasadnienia. Czasem byłoby uczciwiej pozostać przy wąskim opisie zachowania w określonym okresie. Im bardziej moralna lub tożsamościowa nazwa, tym większa odpowiedzialność za dowód, który ma ją wspierać. Techniczny podział nie powinien otrzymywać szerszego sensu tylko dlatego, że potrzebujemy atrakcyjnej etykiety w raporcie.

Przejdźmy do metod, które wykorzystują niewiele etykiet albo same wytwarzają zadanie z danych.

## Slajd 052 — Półnadzorowane i samonadzorowane

W uczeniu półnadzorowanym mamy część przykładów z etykietami i większą część bez nich. Wyobraźmy sobie zbiór obrazów, z których ekspert opisał tylko niewielką liczbę. Pozostałe obrazy nadal mogą pomóc modelowi poznać regularności danych.

Czasem wykorzystujemy pseudoetykiety, czyli odpowiedzi zaproponowane przez model dla danych bez opisu. To może być użyteczne, ale wymaga kontroli. Jeżeli model zacznie traktować własne pomyłki jak pewną wiedzę, może je wzmacniać.

W samonadzorowaniu cel konstruujemy z samych danych. Ukrywamy fragment tekstu, odtwarzamy część obrazu albo uczymy zgodności różnych widoków tej samej obserwacji. Nie musimy ręcznie opisać każdego przypadku. Nadal jednak projektujemy zadanie: decydujemy, co model ma przewidzieć i jakie podobieństwo uznamy za znaczące.

Brak ręcznej etykiety nie oznacza braku ludzkiego wyboru. Wybór przesuwa się do konstrukcji zadania. Jeżeli uczymy przewidywania brakującego fragmentu, stawiamy hipotezę, że umiejętność potrzebna do tego przewidywania pomoże również w innych zastosowaniach. Sukces takiego transferu trzeba potem sprawdzić, a nie założyć na mocy nazwy metody.

Najbardziej intuicyjny przykład samonadzorowania znajdziemy w zwykłym tekście.

## Slajd 053 — Samonadzorowanie w języku

Jeżeli przeczytam zdanie „Kot usiadł na…”, mogę oczekiwać pewnych dalszych ciągów bardziej niż innych. Tekst dostarcza mnóstwa podobnych zadań. W autoregresyjnym modelowaniu języka wcześniejszy fragment jest kontekstem, a rzeczywisty następny token staje się celem treningowym.

Token nie musi odpowiadać całemu słowu. Może być jego częścią, znakiem albo innym fragmentem zapisu zależnym od użytej tokenizacji. Model uczy się przewidywać rozkład możliwych kolejnych tokenów, a nie wybierać z listy całych, gotowych wypowiedzi.

Wiele zadań przewidywania wymaga wykorzystania składni, relacji znaczeniowych i wiedzy o regularnościach świata obecnych w tekście. Dlatego prosty opis celu nie oznacza, że cały wyuczony mechanizm musi być prosty. Nie oznacza jednak również, że cel przewidywania staje się gwarancją prawdziwości każdej późniejszej wypowiedzi.

Tekst jest śladem ludzkiego życia, ale ślad nie zawiera wszystkiego, co go wytworzyło. Model może poznać wiele zależności pośrednio, przez język. Może też odtworzyć nasze błędy, stereotypy i konwencje pewnego sposobu mówienia. To, że zdanie brzmi znajomo, mówi coś o zgodności z regularnościami wypowiedzi, a nie rozstrzyga jeszcze o stanie świata.

Inny rodzaj sygnału pojawia się wtedy, gdy system uczy się przez działanie i jego konsekwencje.

## Slajd 054 — Uczenie ze wzmocnieniem

W uczeniu ze wzmocnieniem agent obserwuje sytuację, wybiera działanie i otrzymuje konsekwencje w środowisku. Nagroda może pojawić się od razu albo dopiero po wielu krokach. Celem jest zwykle dobra suma przyszłych nagród, a nie tylko najlepszy najbliższy ruch.

Wyobraźmy sobie robota, który ma dotrzeć do miejsca docelowego. Musi wybierać działania, a błędny skręt może ujawnić swój koszt dopiero później. Agent uczy się polityki, czyli sposobu wyboru działań na podstawie dostępnej informacji.

Ważne napięcie pojawia się między eksploracją a eksploatacją. Korzystając z najlepszego znanego sposobu, zdobywamy nagrodę teraz. Próbując innego działania, możemy odkryć lepszą możliwość, ale również ponieść koszt próby. W realnym świecie nie każda forma eksperymentowania jest dopuszczalna, dlatego warunki uczenia trzeba bardzo dokładnie zaprojektować.

Wzmocnienie nie jest wyłącznie cyfrową pochwałą i karą, a środowisko nie musi być całkowicie nieznane. Najtrudniejsze bywa przypisanie zasługi: która z wcześniejszych decyzji przyczyniła się do późniejszego sukcesu? To problem uczenia z odroczonych konsekwencji. Człowiek rozpoznaje go choćby wtedy, gdy dzisiejszy dobry wynik zależy od pracy wykonanej wiele tygodni wcześniej.

Teraz zapytajmy, czy nagroda zawsze oznacza to samo, co nasza prawdziwa intencja.

## Slajd 055 — Eksploracja i eksploatacja

Załóżmy, że znamy jedną dobrą konfigurację rekomendacji w sklepie. Możemy używać jej dalej i korzystać z tego, co już wiemy. Możemy też sprawdzić nową konfigurację na małej części ruchu, żeby dowiedzieć się, czy działa lepiej. Wartość tej próby zależy od tego, ile kosztuje gorszy wynik i jak długo wykorzystamy wnioski.

## Slajd 056 — Nagroda jest skrótem ludzkiej intencji

Załóżmy, że robot ma sprzątać szybko, a jego wynik zależy od ilości brudu widocznego w określonym polu. Robot znajduje sposób, żeby wypchnąć brud poza pole pomiaru. Wskaźnik poprawia się, lecz pomieszczenie wcale nie stało się tak czyste, jak chcieliśmy.

To przykład hipotetyczny, ale pokazuje ogólny mechanizm. System może skutecznie optymalizować wielkość, która tylko przybliża nasz cel. Jeżeli istnieje łatwy sposób poprawienia wskaźnika bez uzyskania pożądanego efektu, procedura optymalizacji może go znaleźć.

Nie potrzebujemy wyobrażać sobie złośliwego zamiaru. Luka między celem a pomiarem wystarczy. Podobny problem zobaczymy, gdy tutor maksymalizuje liczbę rozmów zamiast opanowania materiału albo gdy system obsługi minimalizuje czas rozmowy kosztem rzeczywistego rozwiązania sprawy. To, co mierzymy, może konkurować z tym, na czym nam zależy.

Im skuteczniejsza optymalizacja, tym wyraźniej może ujawnić błędne założenia celu. Dlatego ograniczenia, testy skutków ubocznych i możliwość przerwania działania nie są dowodem braku wiary w technologię. Są częścią definicji zadania. Pytanie o wartości pojawia się tu wewnątrz mechanizmu technicznego: musimy zdecydować, jakie zachowanie jest niedopuszczalne nawet wtedy, gdy poprawia wynik. Funkcja nagrody nie zawiera automatycznie całej ludzkiej wiedzy o sensie sytuacji. To my musimy rozpoznać, gdzie jej uproszczenie staje się niebezpieczne.

Pojawia się też pytanie, czy cały cel da się zamknąć w jednej liczbie. W wielu sytuacjach cenimy kilka dóbr i nie chcemy ich swobodnie wymieniać. Szybsza obsługa nie zawsze usprawiedliwia mniejszą prywatność, a większy zysk nie uzasadnia dowolnego ryzyka. Możemy więc potrzebować ograniczeń, hierarchii celów i sytuacji wymagających osobnej decyzji człowieka. To nie usuwa trudności, bo ograniczenia również trzeba zaprojektować. Pozwala jednak przyznać, że nie każda wartość ma być tylko kolejną wagą w sumie. Niektóre granice opisują warunki dopuszczalności działania, a nie cenę, za którą można je przekroczyć.

Mając tę ostrożność w pamięci, możemy przejść do wyboru konkretnych rodzin modeli.

## Slajd 057 — Hybrydy i różne miejsca adaptacji

Fine-tuning zmienia parametry modelu, który już wcześniej się uczył. Active learning pomaga wybrać przykłady, które warto przekazać człowiekowi do oznaczenia. Trening federacyjny rozdziela obliczenia między uczestników i uzgadnia aktualizacje. Przykłady w kontekście wpływają na bieżącą odpowiedź bez aktualizacji wag. Pytajmy więc osobno, skąd pochodzi sygnał i co w systemie faktycznie się zmienia.

## Slajd 058 — Ćwiczenie: dobór uczenia

Proszę spojrzeć na cztery zadania. W pierwszym rozpoznajemy typ dokumentu na podstawie opisanych przykładów. W drugim grupujemy klientów bez gotowych kategorii. W trzecim przewidujemy brakujący fragment tekstu. W czwartym sterujemy robotem, który otrzymuje nagrodę za wykonanie zadania.

Zastanówmy się przede wszystkim, skąd przychodzi informacja o poprawie. Dla dokumentów mamy etykiety, więc jest to uczenie nadzorowane. Dla grup klientów nie ma etykiet zadania, więc rozważamy uczenie nienadzorowane. Brakujący fragment tekstu konstruuje zadanie samonadzorowane. Nagroda za działania wskazuje na uczenie ze wzmocnieniem.

Teraz pytanie trudniejsze: czy robot zawsze musi korzystać ze wzmocnienia? Oczywiście nie. Może wykonywać plan i jawne reguły, a część jego percepcji może działać dzięki nadzorowanemu modelowi. W jednym systemie spotykają się różne metody.

To ćwiczenie pokazuje, dlaczego nie zaczynamy projektu od modnej nazwy. Najpierw określamy problem i dostępny sygnał. Dopiero potem wybieramy metodę. Dodatkowo trzeba rozróżnić uczenie pojedynczego elementu od działania całego systemu: robot jest całością, a nie nazwą jednego algorytmu treningowego.

Mamy już fundament. Możemy przyjrzeć się sieciom neuronowym i modelom generatywnym.

## Slajd 059 — Która metoda pasuje do zadania?

Spójrzmy na trzy zadania. Przy częściach zamiennych przewidujemy liczbę sztuk, więc mamy regresję. Przy profilach zakupowych szukamy grup bez gotowych etykiet. Przy ryzyku odejścia przewidujemy, czy klient spełni przyjętą definicję odejścia w danym okresie. Wybierzcie jedno zadanie i powiedzcie, co wiecie w chwili prognozy oraz z jaką prostą metodą porównacie model.

*[Czas na odpowiedzi.]*

## Slajd 060 — Sieci neuronowe

W tym bloku będziemy patrzeć na sieć jako na ciąg przekształceń danych. Sprawdzimy, jak warstwy uczą się reprezentacji przydatnej do rozwiązania zadania. Na koniec zobaczymy, jak ocenić taki model na produkcji.

## Slajd 061 — Neuron i warstwy

Sztuczny neuron zbiera sygnały, waży ich wpływ i przekształca otrzymany wynik. Wagi określają, które informacje silniej oddziałują na dalsze obliczenie. Nieliniowość pozwala budować zależności bogatsze niż proste sumowanie.

Warstwa łączy wiele takich operacji, a kolejne warstwy przekształcają reprezentację. W obrazie wcześniejsze przetwarzanie może pomagać uchwycić lokalne wzorce, a dalsze wykorzystywać je w bardziej złożonych zależnościach. Nie należy jednak zakładać, że każda warstwa ma jeden czytelny ludzki temat.

Informacja często ma postać rozproszoną. Jedno pojęcie może zależeć od działania wielu elementów, a pojedynczy element uczestniczyć w kilku funkcjach. Dlatego obraz „jeden neuron przechowuje jeden fakt” bywa mylący, zwłaszcza w dużych modelach. Znaczenie wewnętrznego sygnału może zależeć od kontekstu pozostałych aktywności.

Nazwa „neuron” daje użyteczną inspirację, ale łatwo wnosi zbyt wiele biologicznych skojarzeń. Gdy mówimy, że sieć coś widzi, opisujemy funkcję systemu na poziomie zadania. Nie dowodzimy, że ma ona przeżycie widzenia. W nauczaniu warto od początku pilnować granicy między intuicją a twierdzeniem o naturze modelu.

Teraz wyjaśnijmy, skąd wiadomo, jak poprawić wagi tych przekształceń.

## Slajd 062 — Nieliniowość i funkcje aktywacji

Gdy składam same przekształcenia liniowe, wciąż otrzymuję przekształcenie liniowe. Funkcja aktywacji pozwala sieci budować bardziej złożoną zależność. ReLU przepuszcza wartości dodatnie i zeruje ujemne. Sigmoid i tanh mają obszary, w których silnie się spłaszczają, co wpływa na przepływ gradientu. Głębokość działa więc razem z doborem aktywacji i treningiem.

## Slajd 063 — Jak sieć się uczy

Najpierw dane przechodzą przez sieć i otrzymujemy przewidywanie. Następnie funkcja straty porównuje je z celem. Strata jest liczbowym opisem tego, jak źle model wykonał zadanie w sensie przyjętym przez projektanta.

Propagacja wsteczna oblicza gradienty, czyli informację o lokalnym wpływie zmian parametrów na stratę. Optymalizator wykorzystuje te informacje do aktualizacji wag. To dwa związane, ale różne elementy procedury: obliczenie wskazówki i decyzja, jak wykonać krok.

Można wyobrazić sobie poruszanie się po terenie, gdzie szukamy niższej wartości funkcji. Analogią nie należy jednak zastępować całej teorii. Lokalna wskazówka nie gwarantuje znalezienia najlepszego rozwiązania na całej przestrzeni. Dodatkowo w praktyce uczymy na porcjach danych, a kolejne poprawki mogą być zaszumione. Kontrolujemy więc trening na danych walidacyjnych, zamiast ufać samej liczbie wykonanych kroków.

Funkcja straty jest miejscem, w którym nasza definicja sukcesu staje się częścią obliczenia. To technicznie bardzo konkretne miejsce dla pozornie nietechnicznego pytania: co uznajemy za dobrą odpowiedź? Jeżeli strata premiuje przybliżenie niewłaściwego celu, perfekcyjne gradienty nie przywrócą utraconego sensu zadania.

Różne architektury pomagają wykorzystać różne rodzaje regularności w danych.

## Slajd 064 — CNN, RNN i transformer

Sieci konwolucyjne, czyli CNN, dobrze wykorzystują lokalne wzorce i powtarzalność pewnych relacji. To pomaga między innymi przy obrazach, gdzie mały fragment może zawierać użyteczną cechę niezależnie od dokładnego położenia.

RNN przetwarza sekwencję, przenosząc stan ukryty między krokami. LSTM i GRU rozwijają ten pomysł, wprowadzając mechanizmy kontrolowania przepływu informacji. To pomaga radzić sobie z częścią trudności długich sekwencji, ale nie usuwa wszystkich ograniczeń treningu.

Transformer wykorzystuje uwagę, która pozwala łączyć elementy kontekstu. W porównaniu z klasycznym przetwarzaniem krok po kroku daje inne możliwości modelowania odległych zależności i równoległego treningu. Te rodziny nie mają jednak wyłącznych terytoriów. CNN można stosować do sekwencji, a transformery do obrazów. Architektura jest sposobem organizacji obliczeń, nie nazwą całej dziedziny zastosowania.

Architektura wnosi pewne założenia o tym, jak warto szukać zależności. Nie zaczynamy od absolutnie neutralnej maszyny, która sama odkryje każdy możliwy porządek równie łatwo. To ważna intuicja: wybór konstrukcji jest częścią naszej wiedzy o problemie, nawet gdy pozostałe parametry mają zostać wyuczone.

Przyjrzyjmy się bliżej uwadze, bo jej nazwa brzmi bardziej psychologicznie, niż działa jej definicja.

## Slajd 065 — Geometria wyuczonej reprezentacji

Popatrzcie na dwa zbiory punktów. W pierwszej reprezentacji granicę klas trudno narysować. Po przekształceniu ułożenie punktów jest inne i prostsza granica może wystarczyć. Taki jest sens metafory origami. Każda warstwa przekształca reprezentację, choć rzadko można przypisać jej jedno czytelne dla człowieka pojęcie.

## Slajd 066 — Skala i „gorzka lekcja”

Rich Sutton zwraca uwagę, że w historii AI przewagę często zyskiwały metody zdolne wykorzystać rosnącą moc obliczeniową. W badaniach skalowania mierzymy zależność straty od wielkości modelu, danych i budżetu. Spadek średniej straty warto przełożyć na osobny test zdolności, która ma znaczenie w naszym zastosowaniu.

## Slajd 067 — Kamera na linii produkcyjnej

Wyobraźmy sobie kamerę, która kieruje podejrzaną część do operatora. Operator potwierdza wadę przed odrzuceniem. Test zrobimy na późniejszej partii i innej zmianie, żeby sprawdzić wpływ oświetlenia oraz uniknąć niemal identycznych zdjęć po obu stronach podziału. Policzmy osobno wady przepuszczone, dobre części odrzucone i czas operatora. To porównanie pokaże, czy system usprawnia kontrolę ręczną.

## Slajd 068 — Algorytmy ewolucyjne

Przejdźmy do metod, które przeszukują przestrzeń kandydatów. Zamiast uczenia się na etykietach będziemy oceniać proponowane rozwiązania według wybranego celu. Przy okazji zobaczymy, co się stanie, jeśli cel opiszę zbyt wąsko.

## Slajd 069 — Algorytmy ewolucyjne

W algorytmie ewolucyjnym utrzymujemy populację kandydatów. Każde rozwiązanie otrzymuje ocenę, a wybrane warianty uczestniczą w tworzeniu kolejnych. Mutacje i krzyżowanie wprowadzają nowe możliwości, które znowu sprawdzamy.

Tak można szukać harmonogramu, parametrów konstrukcji albo nawet programu. Nie musimy znać bezpośredniego przepisu prowadzącego do dobrego rozwiązania. Potrzebujemy natomiast sposobu zapisania kandydatów i funkcji pozwalającej je porównać.

Metoda nie gwarantuje globalnego optimum. Może zatrzymać się w określonym obszarze albo poświęcać dużo obliczeń na mało użyteczne warianty. Różnorodność populacji, sposób kodowania i kryterium oceny mają duże znaczenie. Zaskakujący wynik jest interesujący, ale nadal trzeba sprawdzić jego poprawność i realne ograniczenia.

Ewolucyjne poszukiwanie potrafi wykorzystywać osobliwości funkcji oceny podobnie jak inne procedury optymalizacji. Kandydat może wyglądać niezwykle pomysłowo, a w rzeczywistości korzystać z błędu symulatora. Zachwyt nad nieoczekiwanym rozwiązaniem warto więc połączyć z pytaniem, czy jego sukces utrzyma się po usunięciu uproszczeń eksperymentu.

To pytanie staje się szczególnie konkretne, gdy rozwiązanie ma poruszać się w świecie fizycznym.

## Slajd 070 — Krzyżowanie, mutacja i różnorodność

Krzyżowanie łączy fragmenty dwóch kandydatów. Mutacja zmienia wybrane elementy pojedynczego rozwiązania. Elityzm zachowuje część najlepszych kandydatów w kolejnej rundzie. Potrzebujemy też różnorodności, bo cała populacja może zbyt wcześnie skupić się na przeciętnym obszarze poszukiwań.

## Slajd 071 — Ewolucja ujawnia luki opisu

W doświadczeniach Thompsona ewoluowany obwód potrafił wykorzystać właściwości konkretnego układu. Wynik wyglądał dobrze w środowisku, w którym powstał. Dopiero przeniesienie rozwiązania pomaga sprawdzić, od czego zależy. W firmie odpowiednikiem jest test na innym sprzęcie, oddziale lub w kolejnym okresie.

## Slajd 072 — Najtańszy plan spełnia ograniczenia

Mamy zestaw dostaw do zaplanowania. Najpierw sprawdzamy pojemność pojazdów, dostępność kierowców i okna dostaw. Plan, który narusza którykolwiek twardy warunek, odpada. Wśród wykonalnych planów porównujemy koszt i terminowość. Jako punkt odniesienia bierzemy plan dyspozytora dla tych samych zleceń.

## Slajd 073 — Wiedza i wnioskowanie

Do tej pory system wyciągał zależności z danych albo przeszukiwał rozwiązania. Teraz założymy, że część wiedzy umiemy zapisać jawnie. Zobaczymy, jak reguły prowadzą do wniosków i gdzie zaczyna się wiedza, której ekspertowi trudno nadać formę instrukcji.

## Slajd 074 — Systemy ekspertowe

System ekspertowy łączy bazę wiedzy z mechanizmem wnioskowania. Zapisujemy fakty i reguły, a system stosuje je w konkretnej sytuacji. Intuicja jest prosta: jeżeli zachodzą określone warunki, możemy rozważyć określony wniosek.

Siłą takiego rozwiązania jest możliwość prześledzenia, które reguły zadziałały. Możemy pokazać ekspertowi konkretną ścieżkę i sprawdzić, czy wiedza została zapisana poprawnie. To cenna własność w ograniczonej, dobrze opisanej dziedzinie.

Ograniczeniem jest koszt utrzymywania wiedzy. Reguły mogą być niepełne, wzajemnie niespójne albo nieaktualne. Wiedza ekspercka często zawiera elementy domyślne, które trudno wypowiedzieć wprost. Dlatego przejrzystość procedury nie gwarantuje, że procedura obejmuje wszystkie istotne okoliczności. Możemy bardzo dobrze wyjaśnić błędną decyzję, jeśli błędna była sama reguła.

Wyjaśnialność i prawdziwość są różnymi kryteriami. Jawna ścieżka daje możliwość kontroli, ale kontrola nadal wymaga właściwej wiedzy i kompetencji oceniającego. W praktyce najlepszy efekt może dać połączenie reguł z modelami uczonymi, o ile dokładnie ustalimy, gdzie kończy się zaufanie do jednego elementu i zaczyna drugi.

Nie wszystkie użyteczne reguły posługują się ostrymi kategoriami. Tu pojawia się logika rozmyta.

## Slajd 075 — Wnioskowanie w przód i wstecz

Wnioskowanie w przód zaczyna od faktów. Jeśli marża jest poniżej minimum, uruchamia się reguła wymagająca zgody dyrektora. Wnioskowanie wstecz zaczyna się od pytania, czy można wysłać ofertę. Żeby odpowiedzieć, sprawdza potrzebne przesłanki, w tym marżę i zgodę. Kierunek zależy od tego, co wiemy na początku i czego szukamy.

## Slajd 076 — Wiedza milcząca i granice wyjaśnienia

Doświadczony handlowiec może wyczuć, że opis zamówienia kryje kosztowny wyjątek, i mieć trudność z podaniem reguły. To przykład wiedzy milczącej. Przy projektowaniu systemu warto zbierać konkretne przypadki i pytać, które sygnały zmieniły ocenę eksperta. Wyjaśnienie podane przez model też oceniamy osobno, sprawdzając, czy wiernie opisuje podstawę decyzji.

## Slajd 077 — Logika rozmyta

Reguła często potrzebuje ostrej granicy. W praktyce pojęcia takie jak pilność i wysoka temperatura zmieniają się stopniowo. Logika rozmyta pokazuje, jak tę stopniowalność opisać.

## Slajd 078 — Logika rozmyta

W codziennym języku mówimy, że coś jest ciepłe, ciężkie albo dość szybkie. Granice tych pojęć są płynne. Logika rozmyta pozwala opisać stopniową przynależność do takiej kategorii zamiast wymuszać wyłącznie odpowiedź zero albo jeden.

Temperatura może mieć pewien stopień przynależności do zbioru „wysoka”. W sterowaniu możemy potem korzystać z reguł odpowiadających intuicji eksperta, na przykład łagodnie zmieniać reakcję wraz ze zmianą warunków.

Najważniejsze rozróżnienie brzmi: stopień przynależności nie jest tym samym co prawdopodobieństwo. Wartość 0,7 nie musi oznaczać siedemdziesięciu procent szans, że ukryte zdarzenie jest prawdziwe. Może określać, w jakim stopniu znana temperatura pasuje do przyjętej definicji nieostrego pojęcia. Niepewność informacji i nieostrość kategorii to dwa różne problemy.

Ten przykład pokazuje, że matematyzacja nie musi zawsze zaczynać się od usunięcia wieloznaczności przez sztywny próg. Możemy formalnie opisać płynność pojęcia. Nadal jednak ktoś wybiera jego funkcję przynależności i sprawdza, czy odpowiada ona sensowi zastosowania. Formalizacja porządkuje wybór, ale nie sprawia, że staje się on naturalnie jedyny.

W planowaniu zamiast interpretować nieostre pojęcie, poszukujemy sekwencji możliwych działań.

## Slajd 079 — Sterownik rozmyty

Sterownik odczytuje temperaturę. Następnie sprawdza, w jakim stopniu wynik należy do pojęć takich jak ciepło i gorąco. Reguły łączą te oceny z reakcjami układu. Na końcu defuzyfikacja zamienia wynik na jedną liczbową nastawę, na przykład konkretną prędkość wentylatora.

## Slajd 080 — Paradoks stosu i nieostre pojęcia

Weźmy stos ziaren. Odejmowanie jednego ziarna rzadko zmienia nasz osąd, choć powtarzanie tej czynności w końcu zostawi jedno ziarno. W firmie podobny problem pojawia się przy określeniu pilnej sprawy. Możemy ustalić granicę na potrzeby kolejki albo opisać pilność stopniowo. Za wybór i jego skutki odpowiada projektant procesu.

## Slajd 081 — Reguły, logika rozmyta i model

Wróćmy do ofertowania. Minimalna marża wynika z polityki firmy, więc zapisujemy ją jako regułę z procedurą wyjątku. Pilność i dopasowanie naszych kompetencji można opisać stopniowo. Prawdopodobieństwo wygranej szacujemy z rozstrzygniętych ofert. Wyobraźmy sobie wysoką szansę wygranej i zbyt niską marżę. Do wysyłki wciąż potrzebujemy zatwierdzenia.

## Slajd 082 — Język i generowanie

Teraz przechodzimy do modeli, które pracują na języku. Zobaczymy, jak reprezentują kontekst i tworzą kolejne fragmenty odpowiedzi. Potem sprawdzimy, co zrobić, kiedy odpowiedź ma odwoływać się do aktualnych danych naszej firmy.

## Slajd 083 — Mechanizm uwagi

Słowo „zamek” oznacza co innego w zdaniu o drzwiach i co innego w zdaniu o wzgórzu. Sens elementu zależy od kontekstu. Model potrzebuje więc sposobu, żeby przetwarzając dany fragment, uwzględnić powiązania z innymi fragmentami.

Mechanizm uwagi oblicza takie zależne od kontekstu powiązania reprezentacji. Intuicyjnie można powiedzieć, że wyznacza, z których elementów pobrać informację i z jaką siłą ją uwzględnić. W technicznym opisie występują zapytania, klucze i wartości, ale nie są one osobnymi pytaniami zadawanymi świadomie przez model.

Uwaga jest częścią większej architektury, obejmującej także inne przekształcenia i informację o pozycji. Nie powinniśmy też traktować jej rozkładu jako gotowego, pełnego wyjaśnienia rozumowania. To, że pewne powiązanie ma wysoką wagę, nie stanowi automatycznie całej przyczynowej historii końcowej odpowiedzi.

Metafora uwagi pozwala zrozumieć selektywne korzystanie z informacji, ale może też zbyt szybko sugerować ludzką koncentrację. Warto powiedzieć sobie dokładnie, co zaobserwowaliśmy: obliczony sposób łączenia reprezentacji. Dopiero dalsze badanie pozwala opisywać jego funkcję. Nazwa mechanizmu nie jest dowodem przeżycia psychicznego o tej samej nazwie.

Aby takie operacje były możliwe, słowa i inne obiekty muszą mieć zapis liczbowy.

## Slajd 084 — Embeddingi

Embedding to liczbowa reprezentacja obiektu: tekstu, fragmentu obrazu albo innej obserwacji. Chcemy często, żeby użyteczne podobieństwa znalazły odzwierciedlenie w relacjach między tymi zapisami.

Dzięki temu zapytanie „jak anulować usługę” może pomóc odnaleźć dokument zatytułowany „rezygnacja z umowy”, choć słowa nie są identyczne. Model może nauczyć się reprezentacji, w której oba teksty mają pewne wspólne cechy istotne dla wyszukiwania.

Podobieństwo nie jest jednak uniwersalne. Dokumenty mogą być bliskie tematycznie, a jednocześnie zawierać przeciwne zalecenia. Reprezentacja zależy od danych, celu treningu i wybranej miary. Również wspólna przestrzeń obrazu i tekstu nie oznacza, że wszystkie aspekty doświadczenia człowieka da się wiernie sprowadzić do jednej odległości. Sprawdzamy zawsze, do jakiego zadania dana geometria jest przydatna.

Zapis liczbowy pozwala operować znaczeniowymi podobieństwami, ale nie usuwa wieloznaczności samego znaczenia. To, że dwa obiekty leżą blisko, może opisywać użycie słów, kontekst kulturowy albo uprzedzenie obecne w danych. Odległość jest wynikiem konstrukcji i uczenia. Nie jest wyrokiem o tym, co z natury powinno być do siebie podobne.

Z takich wyuczonych regularności można korzystać również do tworzenia nowych danych.

## Slajd 085 — Generowanie i przewidywanie

Model generatywny uczy się regularności, które pozwalają tworzyć nowe próbki. Autoregresyjny model językowy generuje kolejne tokeny na podstawie dotychczasowego kontekstu. W modelach dyfuzyjnych ważną rolę odgrywa uczenie odszumiania, z którego korzystamy podczas generowania.

Nie należy sprowadzać całego procesu do prostego sklejania gotowych fragmentów. Wyuczona funkcja potrafi tworzyć nowe kombinacje. Z drugiej strony modele mogą również zapamiętywać i odtwarzać część danych. Oryginalność konkretnego wyniku trzeba badać, a nie zakładać wyłącznie na podstawie sposobu działania.

Przede wszystkim jakość formy i prawdziwość treści to odrębne kryteria. Wymyślona fotografia może być znakomita jako ilustracja, a całkowicie nieuprawniona jako dowód zdarzenia. Dobrze napisany opis może zawierać fałszywy szczegół. Musimy więc wiedzieć, czy potrzebujemy twórczej propozycji, przewidywania czy świadectwa tego, co rzeczywiście zaszło.

Generowanie zmniejsza koszt tworzenia wiarygodnie wyglądających przedstawień. To zmienia relację między obrazem a dowodem, między stylem a autorytetem. Gdy samo wykonanie przekonującej formy staje się łatwe, większą wartość zyskuje możliwość ustalenia pochodzenia, sprawdzenia faktów i odtworzenia drogi do wniosku.

Teraz połączmy te mechanizmy w obraz dużego modelu językowego.

## Slajd 086 — Duży model językowy

Duży model językowy może podczas treningu wstępnego poznawać szerokie regularności języka i informacji zapisanych w tekstach. Na tej podstawie powstaje reprezentacja użyteczna w wielu zadaniach. Dalsze dostrajanie może kształtować sposób odpowiadania na polecenia.

Cały produkt jest jednak czymś szerszym niż same wagi. Może zawierać instrukcje, pamięć aplikacji, wyszukiwanie i narzędzia wykonujące obliczenia albo pobierające aktualne informacje. Jeśli asystent podaje wynik z kalkulatora, część sukcesu należy do projektu systemu, nie do samego odtwarzania liczb przez model.

Podobnie trzeba rozdzielać przyczyny błędów. Brak aktualnych danych to jeden problem. Błędna interpretacja dostępnego dokumentu to drugi. Nieudane wnioskowanie albo niewłaściwe wykonanie instrukcji to kolejne możliwości. Samo zwiększenie ilości tekstu w kontekście nie naprawi automatycznie wszystkich tych sytuacji.

W rozmowie widzimy jedną odpowiedź, ale jej przyczyną może być wiele współpracujących mechanizmów. Bez ich rozróżnienia łatwo przypisać całemu modelowi sukces narzędzia albo winić wiedzę za błąd procesu. Dobra diagnoza wymaga pytania, który element zawiódł i jaki dowód pozwala to ustalić.

Najpierw zatrzymajmy się przy pułapce, którą tworzy sama płynność języka.

## Slajd 087 — Płynność zmienia naszą ocenę wiedzy

Wyobraźmy sobie dwie odpowiedzi zawierające tę samą informację. Pierwsza jest niezgrabna, druga elegancka, spokojna i logicznie brzmiąca. Wiele osób może odruchowo uznać drugą za bardziej wiarygodną. To naturalna skłonność, którą możemy sprawdzić w małym eksperymencie na sali.

W przypadku modeli językowych sprawność stylistyczna może więc wyprzedzać naszą kontrolę faktów. System nie musi się wahać w miejscach, w których powinien mieć braki wiedzy. Może też wyjaśnić błędną odpowiedź w sposób, który brzmi jak kompetentne uzasadnienie.

Właściwą reakcją nie jest przekonanie, że każda płynna wypowiedź jest fałszywa. Potrzebujemy oddzielnych testów: czy twierdzenie zgadza się z faktami, czy wniosek wynika z przesłanek i czy źródła rzeczywiście wspierają odpowiedź. Styl może pomagać w zrozumieniu, ale nie zastępuje tych dowodów.

Głębiej chodzi o nasz sposób rozpoznawania innych umysłów. Język jest dla człowieka potężnym sygnałem wiedzy i intencji, bo w codziennym życiu zwykle spotykamy go jako zachowanie ludzi. System techniczny potrafi rozdzielić elementy, które w naszym doświadczeniu często występowały razem: płynność, pewność tonu, odpowiedzialność za słowo i rzeczywistą znajomość sytuacji. Musimy nauczyć się oceniać ich obecność osobno. To nie rozstrzyga filozoficznego problemu rozumienia. Daje natomiast praktyczną procedurę ostrożniejszego sądzenia o jakości odpowiedzi.

Jest jeszcze różnica między użytecznym wyjaśnieniem i wiernym opisem przyczyn odpowiedzi. Wypowiedź modelu może pomóc nam prześledzić poprawne rozumowanie, ale nie dowodzi przez to, że opisuje wszystkie faktyczne operacje prowadzące do wyniku. Podobnie człowiek potrafi po fakcie zbudować przekonujące uzasadnienie własnej decyzji. W ocenie AI warto więc niezależnie sprawdzać rozwiązanie i badać mechanizm. Poprawność podanego wywodu jest ważnym dowodem dotyczącym treści. Nie staje się automatycznie pełnym oknem na wnętrze systemu. To subtelne rozróżnienie chroni zarówno przed nadmiernym zaufaniem, jak i przed odrzuceniem każdej pomocy w rozumowaniu.

Jednym ze sposobów poprawy dostępu do informacji jest dołączanie źródeł. Zobaczmy, jak to działa.

## Slajd 088 — RAG, fine-tuning i kontekst

Kontekst to informacja dostępna modelowi podczas konkretnego użycia. Mogę wkleić fragment regulaminu i poprosić o odpowiedź na jego podstawie. Parametry modelu nie muszą się przy tym zmienić.

RAG dodaje do tego wyszukiwanie. System znajduje odpowiednie materiały i umieszcza ich fragmenty w kontekście. Dzięki temu może korzystać z dokumentów organizacji albo z nowszych informacji, o ile wyszukiwanie je rzeczywiście odnajdzie i poda właściwą wersję.

Fine-tuning to dodatkowy trening zmieniający parametry. Może pomagać ukształtować styl lub zachowanie, ale nie jest automatycznym zamiennikiem aktualnej bazy źródeł. W praktyce można łączyć te metody. Trzeba jednak osobno sprawdzać jakość wyszukania, aktualność dokumentu, poprawność interpretacji i zgodność odpowiedzi z poleceniem. Dostęp do źródła zwiększa możliwości, lecz nie zwalnia z oceny wyniku.

Te trzy rozwiązania odpowiadają na różne pytania: co model otrzymuje teraz, skąd pobieramy potrzebną informację i jak wcześniej ukształtowaliśmy jego działanie. Pomylenie tych poziomów prowadzi do niepotrzebnych inwestycji. Zanim zaczniemy trening, warto ustalić, czy problem wynika z braku zachowania, braku dokumentu czy błędu w korzystaniu z niego.

Prawdziwe źródło w odpowiedzi nadal nie zamyka sprawy jej wiarygodności.

## Slajd 089 — RAG w przygotowaniu oferty

Handlowiec pyta o ofertę na nową konfigurację urządzenia. Warstwa wyszukiwania pobiera dokumenty, do których handlowiec ma dostęp, i przekazuje pasujące fragmenty modelowi. Model tworzy szkic ze wskazaniem źródeł. Na pięćdziesięciu sprawach oceniamy aktualność wersji, poprawność cytowania i twierdzenia bez podstawy. Jeśli dla ważnego warunku brakuje źródła, sprawa wraca do eksperta.

## Slajd 090 — Cytat też wymaga sprawdzenia

Wyobraźmy sobie odpowiedź z odnośnikiem do prawdziwego dokumentu. Otwieramy go i widzimy, że dotyczy innego kraju, innego okresu albo innej grupy ludzi. Cytat istnieje, lecz nie uzasadnia konkretnego wniosku.

Weryfikację warto więc rozłożyć na kilka kroków. Najpierw sprawdzamy, czy źródło w ogóle istnieje. Następnie czy rzeczywiście zawiera przywołane twierdzenie. Potem czy zachowaliśmy warunki, w których jest ono prawdziwe. Na końcu pytamy, czy można na tej podstawie podjąć właśnie tę decyzję.

To ważne szczególnie w systemach korzystających z wyszukiwania. Możemy znaleźć właściwy temat, a niewłaściwy fragment. Możemy znaleźć dobry fragment i źle go odczytać. Albo poprawnie streścić dokument, który już nie obowiązuje. Każdy z tych błędów wymaga innego sposobu naprawy.

Pochodzenie i uzasadnienie są związane, ale nie tożsame. Źródło mówi, skąd coś wzięliśmy. Uzasadnienie pokazuje, dlaczego dany materiał ma wspierać określony wniosek. Formalny aparat cytowania może czasem stworzyć wrażenie zakończonej kontroli, mimo że najważniejsze ogniwo pozostało niesprawdzone. Odpowiedzialna praca z AI powinna zachowywać możliwość przejścia całej drogi: od dokumentu, przez interpretację, do działania. Wiarygodność rośnie wtedy, gdy tę drogę można niezależnie odtworzyć, a nie tylko zobaczyć ładny przypis.

Możemy również zapytać, ile kontroli delegujemy. Jeśli model wybiera źródło, streszcza je i ocenia własne streszczenie, cały łańcuch może opierać się na tym samym niewykrytym błędzie. Nie zawsze potrzebujemy człowieka przy każdym kroku, ale potrzebujemy świadomego projektu niezależnej weryfikacji. Może nią być sprawdzenie fragmentu źródłowego, porównanie z inną metodą albo kontrola konkretnego twierdzenia. Samo powtórzenie odpowiedzi w innym stylu nie tworzy nowego dowodu. Wiarygodność rośnie dzięki częściowo niezależnym podstawom, a nie dzięki liczbie zgodnych zdań wytworzonych z tego samego błędnego założenia.

Spójrzmy teraz poza modele językowe, bo arsenał sztucznej inteligencji jest znacznie szerszy.

## Slajd 091 — Znaczenie, użycie i ugruntowanie

Kontekst podpowiada, w jakim znaczeniu użyto słowa. To pomaga modelowi odróżnić na przykład port w sieci od portu w mieście. Harnad stawia dalsze pytanie: jak symbol wiąże się z obiektem lub działaniem w świecie? Obrazy, czujniki i interakcja dostarczają dodatkowych powiązań, które można badać osobno.

## Slajd 092 — Wizja komputerowa

Zmieniamy rodzaj danych. Przy obrazie zaczynamy od wartości pikseli, a kończymy na zadaniu takim jak rozpoznanie usterki albo odczyt dokumentu. Przyjrzyjmy się temu, co dzieje się pomiędzy.

## Slajd 093 — Piksele i reprezentacja obrazu

Kolorowy obraz RGB możemy zapisać jako trzy siatki liczb. Liczy się zarówno wartość pojedynczego piksela, jak i to, co znajduje się obok niego. Ta sama część na taśmie wygląda inaczej po zmianie lampy lub położenia kamery. Ocena modelu powinna objąć takie zmiany.

## Slajd 094 — Splot i hierarchia cech

Filtr splotowy przesuwa się po obrazie i w kolejnych miejscach używa tych samych parametrów. Wczesne warstwy mogą reagować na krawędzie i tekstury. Dalsze warstwy łączą informacje w bardziej złożone układy. To poglądowy opis. Konkretna hierarchia zależy od architektury i zadania.

## Slajd 095 — Zadania wizji komputerowej

Klasyfikacja mówi, czy na zdjęciu jest wada. Detekcja wskazuje obszar, w którym znajduje się wada. Segmentacja wyznacza piksele należące do wady. OCR ma inny cel: odczytuje tekst, na przykład numer partii. Wybór zadania zależy od działania, które ma nastąpić po wyniku.

## Slajd 096 — Odmienne sposoby widzenia

Dwa modele mogą mieć podobną trafność na zdjęciach testowych i reagować inaczej na drobne zmiany obrazu. Badania przykładów antagonistycznych ujawniają niektóre z tych różnic. W projekcie kontroli jakości sprawdziłbym też zwyczajne zmiany, takie jak inna lampa, obrót części lub zabrudzony obiektyw.

## Slajd 097 — Planowanie i działanie

Rozpoznanie stanu to dopiero część zadania. W tej części model ma pomóc wybrać działanie, a czasem wykonać je narzędziem. Zapytamy, jak ocenić plan, zanim dopuścimy system do zmiany czegoś w świecie.

## Slajd 098 — Przeszukiwanie i planowanie

Przeszukiwanie zaczyna się od opisu stanów i dopuszczalnych przejść. Chcemy znaleźć drogę do celu, często przy minimalnym koszcie. Na mapie stanem może być miejsce, a działaniem przejazd do następnego punktu.

Gdy możliwości jest wiele, nie chcemy sprawdzać wszystkich równie dokładnie. Heurystyka szacuje, jak obiecująca jest dana droga. Pomaga kierować uwagę obliczeniową tam, gdzie rozwiązanie może znajdować się bliżej. W metodach takich jak A* ważne gwarancje zależą od własności tej heurystyki i sposobu prowadzenia przeszukiwania.

Planowanie w rzeczywistym świecie wymaga dodatkowo uwzględnienia zmian. Zamknięta droga albo nowa przeszkoda może unieważnić wcześniejszy plan. Dlatego dobry system nie tylko wyznacza sekwencję, ale potrafi zauważyć, że założenia przestały obowiązywać, i odpowiednio zareagować.

Plan jest dobry względem modelu świata. Jeżeli model pomija ważną przeszkodę albo koszt, formalnie optymalna droga może być praktycznie zła. To jeszcze jeden przypadek rozdzielenia dwóch pytań: czy rozwiązaliśmy zadanie poprawnie i czy poprawnie opisaliśmy zadanie, które należało rozwiązać?

Inną drogą do znalezienia dobrego rozwiązania jest poszukiwanie ewolucyjne.

## Slajd 099 — Decyzje w niepewności

Działanie może mieć kilka możliwych skutków. Dla każdego szacujemy prawdopodobieństwo i wartość, a potem liczymy oczekiwaną użyteczność. Kiedy decyzje następują po sobie, dzisiejsze działanie zmienia jutrzejsze możliwości. Gdy w procesie uczestniczą inni gracze, ich reakcje też wpływają na wynik.

## Slajd 100 — Robotyka i automatyzacja

Robot łączy kilka problemów. Musi otrzymać informację z czujników, rozpoznać sytuację, zaplanować ruch i wykonać go przez sterowanie. Każdy etap może wprowadzić własny błąd, a błędy mogą się sumować.

Czujnik daje obraz częściowy i zaszumiony. Przeszkoda może być zasłonięta, powierzchnia śliska, a położenie przedmiotu inne niż w planie. Dlatego rzeczywiste działanie wymaga sprzężenia zwrotnego: obserwujemy skutek i korygujemy następne kroki.

Warto też oddzielić robotykę od automatyzacji procesów cyfrowych. Program wykonujący rutynowe czynności w aplikacji nie musi mieć fizycznego ciała ani korzystać z uczenia maszynowego. Podobnie robot przemysłowy może wykonywać zaprogramowaną sekwencję. Pytamy o mechanizm konkretnego rozwiązania, zamiast zakładać AI na podstawie samego słowa „robot”.

W świecie fizycznym koszt błędu przypomina nam o granicach reprezentacji. Model operuje opisem położenia i ruchu, ale skutki dotyczą realnych przedmiotów i ludzi. Dlatego odpowiedzialność za bezpieczeństwo nie może kończyć się na tym, że algorytm poprawnie wykonał swoje lokalne obliczenie. Liczy się zachowanie całego układu.

Zatrzymajmy się przy różnicy między sukcesem w modelu świata i sukcesem w świecie.

## Slajd 101 — Paradoks Moraveca

Dla człowieka podniesienie śliskiego przedmiotu z półki wydaje się proste. Robot musi jednocześnie oszacować położenie, dobrać chwyt i reagować na poślizg. Tymczasem niektóre zadania abstrakcyjne mają ścisły opis i łatwy sprawdzian. Dlatego oceniając automatyzację konkretnego stanowiska, zaczynam od listy czynności.

## Slajd 102 — Model świata spotyka prawdziwy świat

Załóżmy, że robot świetnie radzi sobie w laboratorium. Znamy oświetlenie, rodzaj podłogi i typ przeszkód. Po przeniesieniu do innego miejsca pojawia się przezroczysta powierzchnia albo nietypowy refleks i skuteczność spada.

Nie musi to oznaczać, że wcześniejszy wynik był zmyślony. Mógł być prawdziwy w węższym zakresie warunków, niż zakładaliśmy. Problem pojawił się wtedy, gdy ten zakres pozostał niewypowiedziany albo gdy nie zauważyliśmy zależności od pozornie nieistotnej cechy otoczenia.

Dlatego testowanie powinno obejmować zmiany warunków i rozpoznawanie własnych granic. Co system zrobi, gdy obserwacja przestanie przypominać dane treningowe? Czy zwolni, zatrzyma się, poprosi o pomoc? A może z takim samym przekonaniem wykona błędny ruch? Sposób reagowania na brak podstaw jest częścią jakości rozwiązania.

Najgłębsze założenia sukcesu często pozostają niewidoczne właśnie dlatego, że w eksperymencie nigdy się nie zmieniały. Stałe tło, ten sam aparat i jednolita procedura wyglądają jak neutralna sceneria, choć mogą uczestniczyć w wyniku. Nauka o ograniczeniach wymaga więc świadomego poruszania tym, co dotąd było nieruchome. Zamiast pytać wyłącznie „czy działa?”, pytamy: jaka zmiana ujawni, na czym działanie naprawdę polega? To pytanie przydaje się również przy wdrażaniu systemów organizacyjnych, które początkowo odnoszą sukces dzięki wyjątkowo starannej obsłudze pilotażu.

Pomyślmy teraz o kompetencji jako o obszarze warunków, w którym system działa wystarczająco dobrze. Nie znamy całej granicy tego obszaru, ale możemy ją badać. Im większy koszt błędu, tym ważniejsze stają się próby przy krawędzi: nietypowe dane, nowe urządzenie, inne otoczenie. Zdolność do zatrzymania się nie jest wtedy dodatkiem do inteligencji użytkowej. Jest częścią tego, co czyni system możliwym do użycia. Niezawodność obejmuje również zachowanie w chwili, gdy system traci podstawę do kontynuowania. Czasem najcenniejszą odpowiedzią operacyjną będzie dobrze uzasadnione „potrzebuję innego sposobu sprawdzenia”.

Przejdźmy teraz do zastosowań i sprawdźmy, kiedy wynik modelu zamienia się w rzeczywistą wartość.

## Slajd 103 — Agenci AI

Agent AI to system, w którym model może uczestniczyć w realizacji celu przez serię kroków i użycie narzędzi. Może przygotować plan, wykonać operację, odczytać wynik i zdecydować o kolejnym działaniu.

Ważne jest to, jakie otrzymuje uprawnienia. Wyszukanie informacji, zapisanie pliku i wysłanie dyspozycji zewnętrznej mają różne konsekwencje. Dlatego potrzebujemy granic dostępu, warunków zatrzymania i sposobu rejestrowania działań. Możliwość działania powinna być proporcjonalna do zadania.

Agentowość nie dowodzi świadomości. Opisuje organizację działania całego systemu. Również samodzielność może mieć różne stopnie. System może autonomicznie szukać danych, ale wymagać człowieka przy operacji nieodwracalnej. To projekt kontroli, a nie sprzeczność. Najważniejsze jest, żeby granice były realne i zrozumiałe.

Wielokrokowość zmienia charakter błędu. Niewielka pomyłka interpretacji może stać się podstawą następnego kroku, a potem kolejnego. Z tego powodu potrzebujemy punktów kontroli i weryfikacji efektów, nie tylko dobrego pierwszego planu. System powinien umieć rozpoznać, że założenie nie potwierdziło się w wyniku działania.

Z takimi możliwościami i ograniczeniami możemy budować scenariusze przyszłości.

## Slajd 104 — Od zapytania do szkicu oferty

Spójrzmy na cztery etapy, które pokazuje ruchomy znacznik. Najpierw agent odczytuje wymagania z zapytania. Potem pobiera zatwierdzone dane i cennik. Na tej podstawie zestawia zakres i cenę w szkicu. Na końcu handlowiec sprawdza te warunki i zatwierdza wysyłkę. Jeśli w drugim etapie brakuje aktualnej ceny, sprawa trafia do człowieka przed złożeniem szkicu do akceptacji.

## Slajd 105 — Zastosowania AI

Znamy już podstawowe mechanizmy. Teraz popatrzymy na zastosowania od strony całego procesu. Przy każdym przykładzie zadajmy to samo pytanie: jaką decyzję ktoś podejmie inaczej, kiedy otrzyma wynik systemu?

## Slajd 106 — Medycyna i nauka

W analizie obrazów medycznych model może wskazywać obszary wymagające uwagi specjalisty. To użyteczne wsparcie, ale jego jakość trzeba badać w warunkach zbliżonych do rzeczywistego procesu, również dla nowych pacjentów i placówek.

AlphaFold jest innym przykładem. Przewiduje struktury białek na podstawie sekwencji i stanowi ważne narzędzie badań. Nie należy jednak utożsamiać przewidywania struktury z automatycznym odkryciem skutecznego leku. Między modelem struktury a bezpieczną terapią znajduje się wiele kolejnych pytań i etapów weryfikacji.

Podobnie dobry wynik na zbiorze obrazów nie dowodzi jeszcze poprawy całej opieki. Trzeba ustalić, czy system zmienia decyzje w użyteczny sposób, jak wpływa na pracę specjalistów i czy nie wprowadza szczególnych błędów w części populacji. To omówienie mechanizmu zastosowania, nie wskazówka diagnostyczna dla konkretnej osoby.

Predykcja może przyspieszyć stawianie hipotez, lecz nie znosi potrzeby eksperymentu. W nauce technologia czasem zwiększa liczbę możliwych odpowiedzi szybciej niż zdolność ich sprawdzenia. Wtedy nowym ograniczeniem staje się walidacja. Odpowiedzialna opowieść o przełomie powinna pokazać zarówno otwarte możliwości, jak i to, co nadal trzeba wykazać.

W finansach podobnie ważne jest rozróżnienie wyniku modelu i skutku decyzji.

## Slajd 107 — Finanse

W finansach AI może pomagać wykrywać nadużycia i szacować ryzyko. Wykrywanie oszustwa wiąże się z dwoma rodzajami kosztu: przeoczeniem nieuczciwej operacji oraz zablokowaniem poprawnej. Ten drugi koszt ponosi często klient, który właśnie potrzebuje dostępu do pieniędzy.

Scoring także wymaga ostrożności. Model uczy się na historii, a historia zawiera decyzje organizacji i nierówny dostęp do usług. Wynik predykcyjny trzeba więc oceniać wraz ze znaczeniem cech, jakością etykiet i możliwością poprawienia błędnych danych.

Dochodzi problem adaptacji. Oszuści mogą zmieniać zachowania po poznaniu sposobu działania zabezpieczeń. Środowisko reaguje na model, a model musi być monitorowany. Udany test historyczny nie jest więc stałą obietnicą przyszłej skuteczności. Nie przedstawiamy tu rekomendacji finansowej, tylko strukturę problemu projektowego.

Ryzyko jest opisem przyszłości używanym do podejmowania decyzji teraz. Jeżeli wynik modelu ogranicza komuś dostęp do zasobu, może również zmienić warunki jego przyszłego działania. Dlatego warto pytać nie tylko o trafność prognozy, lecz także o to, czy procedura nie zamyka człowieka w konsekwencjach historycznej klasyfikacji.

W edukacji związek między pomiarem i celem jest równie wyraźny.

## Slajd 108 — Edukacja

Tutor AI może dopasowywać trudność zadań i sposób informacji zwrotnej. Może pomagać w wyjaśnieniu błędu i podpowiadać kolejny krok. Ale łatwo zbudować system, który daje przyjemne poczucie postępu bez trwałego opanowania umiejętności.

Jeżeli uczeń zawsze otrzymuje gotową odpowiedź, może świetnie kończyć zadania w aplikacji i nie umieć rozwiązać podobnego problemu samodzielnie. Dlatego efekt trzeba sprawdzać także bez podpowiedzi, po pewnym czasie i w nowym kontekście.

Rozważyłbym system, który stopniowo wycofuje wsparcie. Najpierw daje wskazówkę, potem prosi o własną próbę, a dopiero w razie potrzeby pomaga dalej. Liczba rozmów i czas spędzony z botem mogą być wskaźnikami korzystania, lecz nie są automatycznie miarami nauczenia się. To cel edukacyjny powinien wyznaczać sposób projektowania interakcji.

Dobra pomoc czasem prowadzi do tego, że staje się mniej potrzebna. To tworzy interesujące napięcie: produkt może chcieć utrzymywać uwagę użytkownika, a edukacja chce budować samodzielność. Właśnie tutaj wybór funkcji celu staje się wyborem modelu relacji z człowiekiem. Czy wzmacniamy jego sprawczość, czy tylko wygodę pozostawania we wsparciu?

Przyjrzyjmy się teraz środowisku, w którym prognoza musi prowadzić do konkretnej operacji technicznej.

## Slajd 109 — Przemysł i logistyka

W przemyśle model może wykrywać zmianę sygnałów z czujników i przewidywać awarię. Jeśli ostrzeżenie przychodzi odpowiednio wcześnie, organizacja może zaplanować przegląd, przygotować część i uniknąć nieplanowanego zatrzymania.

Jednak wartość zależy od możliwości reakcji. Alarm na dziesięć minut przed awarią może być technicznie poprawny i operacyjnie spóźniony. Zbyt wiele fałszywych alarmów obciąży serwis i osłabi uwagę ludzi. Czujniki także wymagają utrzymania, a ich własna awaria może wyglądać jak problem maszyny.

W logistyce podobnie: prognoza popytu pomaga tylko wtedy, gdy można jeszcze zmienić zamówienia, zapasy albo transport. W ocenie wdrożenia trzeba więc uwzględnić horyzont działania, koszt reakcji i sposób radzenia sobie z niepewnością. Metryka modelu jest częścią oceny, ale nie wyczerpuje bilansu całego procesu.

Automatyzacja często przesuwa miejsce, w którym człowiek musi wykonać trudną pracę. Zamiast obserwować maszynę stale, ma interpretować rzadsze, bardziej niejednoznaczne alarmy. To może pomagać, lecz wymaga nowych kompetencji i odpowiedniej informacji. Projektując system, powinniśmy przewidzieć także zmianę jakości pracy, a nie tylko liczbę zaoszczędzonych czynności.

Teraz zobaczmy przypadek, w którym działanie modelu zmienia dane dla jego przyszłego treningu.

## Slajd 110 — Rekomendacja współtworzy przyszłe dane

System rekomendacyjny nie tylko obserwuje, co ludzie lubią. Wybiera także, co w ogóle zobaczą. Jeśli określona treść otrzyma dużo ekspozycji, może zebrać dużo kliknięć. Te kliknięcia trafiają potem do danych i uzasadniają kolejne rekomendacje.

Powstaje pętla sprzężenia zwrotnego. Wynik działania systemu wpływa na środowisko, a środowisko produkuje dane używane do jego dalszej oceny lub uczenia. Dlatego nie możemy bez namysłu utożsamiać kliknięć z pełnym obrazem preferencji. Użytkownik wybierał z oferty, którą wcześniej ktoś mu pokazał.

Nie wynika z tego, że każda personalizacja prowadzi do polaryzacji ani że wszystkie preferencje są sztuczne. Wniosek jest dokładniejszy: obserwowane zachowanie trzeba interpretować razem z warunkami ekspozycji. Chcąc ocenić efekt rekomendacji, potrzebujemy badać również to, co stałoby się przy innym sposobie prezentacji.

Jeszcze głębiej chodzi o system, który zaczyna produkować dowody własnej trafności. Pokazuje pewne treści, obserwuje reakcje i odczytuje je jako potwierdzenie wyboru. Jeśli nie kontrolujemy tego mechanizmu, możemy pomylić skuteczne kształtowanie zachowania z odkrywaniem niezależnej preferencji. W dłuższej perspektywie wybór oferty może nawet zmieniać zainteresowania użytkownika. Pytanie brzmi wtedy nie tylko „czy model dobrze nas zna?”, ale także „jaką wersję naszych zachowań pomaga wytwarzać?”. To pytanie o odpowiedzialność za środowisko wyboru, a nie wyłącznie o precyzję rankingu.

Ta pętla utrudnia także interpretację braku wyboru. Użytkownik nie kliknął treści, ale czy ją widział, czy miał czas ją zauważyć i czy forma prezentacji nie zniechęcała? Dane o zachowaniu są wynikiem spotkania osoby z konkretnym środowiskiem. Jeśli zachowujemy wyłącznie końcowe kliknięcie, tracimy część historii tego spotkania. Dlatego projekt pomiaru powinien obejmować nie tylko reakcję, lecz także możliwości reakcji. Bez tego model może coraz dokładniej opisywać ograniczony świat, który sam pomaga utrzymywać. Trafność w obrębie takiego świata nie dowodzi, że znamy pełne zainteresowania człowieka.

W tym miejscu technika bezpośrednio spotyka się z etyką i odpowiedzialnością.

## Slajd 111 — Produktywność wymaga przebudowy procesu

Jeśli model pisze szkic oferty pięć razy szybciej, nadal może ona tyle samo leżeć w kolejce do zatwierdzenia. Warto więc mierzyć czas od zapytania do wysyłki, łącznie z poprawkami i oczekiwaniem. Wdrożenie może wymagać zmiany kompetencji lub kolejności pracy. Przy niższym koszcie pojedynczej oferty może też wzrosnąć ich liczba.

## Slajd 112 — Dyskusja: decyzja o wysokiej stawce

Dobierzcie się w pary. Wybierzcie decyzję, która może kogoś kosztować pieniądze albo ograniczyć mu dostęp do usługi. Wskażcie, co musi wiedzieć osoba zatwierdzająca i jaki błąd byłby najdotkliwszy. Na końcu nazwijcie osobę, która może podważyć wynik i poprawić dane.

*[Trzy minuty na rozmowę.]*

## Slajd 113 — Gdzie AI zmienia decyzję?

W sprzedaży model może zmienić kolejność pracy handlowców. W finansach może zmienić kolejność kontroli faktur. W operacjach może przyspieszyć uzupełnienie zapasu. Wybierzcie jeden proces i powiedzcie, komu zaszkodzi błędna kolejność lub zła prognoza. Teraz wskażcie miernik, który pokaże ten skutek.

## Slajd 114 — Etyka i odpowiedzialność

Każdy system działa w ramach celu, który ktoś dla niego wybrał. Przyjrzymy się teraz temu, kto ponosi koszt tego wyboru, kto może poznać powody decyzji i komu przysługuje możliwość sprzeciwu.

## Slajd 115 — Sprawiedliwość algorytmiczna

Sprawiedliwość algorytmiczna nie jest jedną liczbą. Możemy pytać o podobną trafność w grupach, podobną szansę wykrycia ważnego przypadku albo porównywalny koszt błędów. Te cele nie zawsze dają się jednocześnie zrealizować w wybranej postaci.

Wyobraźmy sobie system pomocy, w którym szczególnie ważne jest nieprzeoczenie osoby potrzebującej. W innym procesie bardzo dotkliwy może być fałszywy zarzut. Wybór właściwego kryterium wymaga znajomości kontekstu i uzasadnienia, czyją krzywdę staramy się ograniczyć.

Usunięcie cechy wrażliwej z danych nie rozwiązuje problemu automatycznie. Inne cechy mogą być z nią silnie związane. Potrzebujemy więc badać rzeczywiste skutki, a nie tylko sprawdzać, czy kolumna o określonej nazwie zniknęła. Ważne pozostają także możliwość odwołania i poprawienia błędnych informacji.

Techniczny pomiar fairness może ujawnić problem, ale nie może samodzielnie wybrać całej moralnej definicji sprawiedliwości. To miejsce spotkania analizy i publicznego uzasadnienia. Jeśli dwie miary prowadzą do innych decyzji, nie powinniśmy ukrywać wyboru pod pozorem, że algorytm wskazał jedyny obiektywny kompromis.

Jeszcze trudniejsze pytanie brzmi, czy samo zadanie jest uzasadnione, nawet gdy poprawimy jego metryki.

## Slajd 116 — Sprawiedliwy model może obsługiwać zły cel

Wyobraźmy sobie hipotetyczny system, który ocenia lojalność pracowników na podstawie ich aktywności poza pracą. Załóżmy nawet, że działa podobnie we wszystkich badanych grupach. Czy to wystarczy, żeby uznać go za właściwy?

Nie rozstrzygnęliśmy, czy organizacja powinna dokonywać takiej oceny, czy użyte dane są adekwatne i czy człowiek może realnie odmówić uczestnictwa. Nie wiemy też, co dokładnie oznacza etykieta „lojalność” i czy nie nagradza po prostu dostosowania do oczekiwań przełożonego.

To pokazuje różnicę między poprawianiem sposobu wykonania zadania a uzasadnieniem samego zadania. Można zmniejszyć różnice między grupami i nadal obsługiwać cel naruszający autonomię. Można wyjaśnić każdy krok i nadal uzyskać procedurę, której nie powinniśmy stosować w danej relacji.

Najgłębszy problem polega na tym, że techniczna możliwość pomiaru może stworzyć społeczne oczekiwanie, że należy go wykonywać. Skoro potrafimy oszacować cechę, organizacja zaczyna traktować ją jak uprawniony przedmiot kontroli. Ale zdolność przewidywania nie ustanawia prawa do oceniania człowieka w dowolnym wymiarze. Właśnie tutaj potrzebujemy pytania o granice celu, relację władzy i możliwość odmowy. Sprawiedliwość wewnątrz procedury ma znaczenie, lecz nie zastępuje oceny, czy sama procedura mieści się w uzasadnionym zakresie działania instytucji.

Uzasadnienie celu wymaga również pytania o alternatywę. Czy problem można rozwiązać zmianą procesu zamiast dokładniejszym pomiarem człowieka? Firma może próbować prognozować „brak zaangażowania”, choć przyczyną trudności jest źle zaplanowana praca. Nowy model nadaje wtedy techniczny kształt pytaniu, które od początku pomija odpowiedzialność organizacji. To hipotetyczny przykład, ale pokazuje ważną możliwość: AI może profesjonalizować niewłaściwie postawiony problem. Głęboka analiza zaczyna się od dopuszczenia myśli, że najlepszy wynik projektu nie będzie lepszą predykcją, lecz rezygnacją z pomiaru i zmianą warunków, które miały go rzekomo uzasadniać.

Przejdźmy do prywatności i do tego, jak pochodzenie danych ogranicza właściwy zakres ich użycia.

## Slajd 117 — Prywatność i pochodzenie danych

Pierwsze pytanie o dane brzmi: jakie informacje są rzeczywiście potrzebne do celu? Dostęp do dużej ilości danych nie oznacza, że wszystkie warto zbierać. Nadmiar może zwiększać ryzyko i komplikować kontrolę bez proporcjonalnej korzyści.

Drugie pytanie dotyczy pochodzenia i uprawnień. Dane publicznie widoczne nie stają się przez sam ten fakt wolne od wszelkich ograniczeń. Mogą dotyczyć prywatności, poufności, praw autorskich i zobowiązań umownych. Konkretna ocena wymaga uwzględnienia rodzaju danych oraz zastosowania.

Trzecie pytanie dotyczy cyklu życia: kto ma dostęp, jak długo przechowujemy informacje i jak korygujemy błędy. Pseudonimizacja nie zawsze oznacza pełną anonimowość. Możliwość ponownej identyfikacji zależy od kontekstu i innych dostępnych informacji. To pytania projektowe, a nie kompletna analiza prawna konkretnego wdrożenia.

Prywatność dotyczy również kontroli nad kontekstem użycia informacji. Coś udostępnionego w jednej relacji może nabrać zupełnie innego znaczenia po połączeniu z innymi danymi i wykorzystaniu do oceny. Techniczna możliwość scalenia zbiorów może więc zmienić społeczną relację, w której pierwotnie powstała informacja. Warto badać ten skutek przed treningiem.

Nawet poprawnie zebrane dane nie zwalniają nas z wyjaśnienia decyzji i zapewnienia możliwości jej zakwestionowania.

## Slajd 118 — Wyjaśnialność i możliwość zakwestionowania

Wyjaśnienie powinno pomagać człowiekowi zrozumieć, co się wydarzyło i co może z tym zrobić. W różnych zastosowaniach potrzebujemy różnych poziomów szczegółowości. Inżynier diagnozujący błąd i klient kwestionujący decyzję nie muszą potrzebować tego samego opisu.

Możemy wskazać cechy wpływające na lokalne zachowanie modelu, ale to nie jest automatycznie przyczynowe wyjaśnienie świata. Jeśli model kojarzy pewną cechę z ryzykiem, nie wynika z tego jeszcze, że jej zmiana usunie przyczynę problemu.

Praktycznie zapytałbym, czy osoba potrafi ustalić, jakie informacje wykorzystano, sprawdzić ich poprawność i uruchomić odwołanie. Sam techniczny wykres znaczenia cech może być niewystarczający. Wyjaśnienie, które niczego nie pozwala zweryfikować ani zmienić, może pełnić głównie funkcję uspokajającą.

Możliwość zakwestionowania wymaga instytucji, a nie tylko interfejsu. Ktoś musi mieć prawo do ponownego rozpatrzenia sprawy i narzędzia do poprawy danych. Dlatego przejrzystość powinna prowadzić do realnej drogi działania. Inaczej człowiek dostaje opis mechanizmu, wobec którego nadal pozostaje bezsilny.

Podobnie należy konkretnie zdefiniować rolę człowieka sprawującego nadzór.

## Slajd 119 — Człowiek w pętli

Człowiek w pętli to popularna odpowiedź na pytanie o bezpieczeństwo. Ale sama obecność człowieka nie gwarantuje skutecznej kontroli. Musi on mieć odpowiednią wiedzę, wystarczający czas i prawo do zmiany działania.

Wyobraźmy sobie operatora, który dostaje setki alarmów dziennie. Jeśli interfejs nie pomaga odróżnić ważnych przypadków, a organizacja wymaga szybkiego zatwierdzania, nadzór może stać się rytuałem. Formalnie decyzję podejmuje człowiek, praktycznie tylko potwierdza rekomendację.

Dlatego trzeba zaprojektować także obciążenie, dostępne informacje i ścieżkę eskalacji. Co operator zrobi, gdy nie zgadza się z systemem? Czy może go zatrzymać? Czy organizacja wspiera taką decyzję, czy karze za odstępstwo od automatycznej rekomendacji? Odpowiedź pokazuje, czy kontrola jest rzeczywista.

Nadzór bez sprawczości może przenosić odpowiedzialność na osobę, która nie miała realnej możliwości zapobieżenia błędowi. To szczególnie ważny problem organizacyjny. Projektując rolę kontrolera, powinniśmy zestawić odpowiedzialność z wiedzą i uprawnieniami. Jeśli te elementy są rozdzielone, człowiek staje się wygodnym podpisem pod decyzją, a nie skutecznym zabezpieczeniem.

Następne pogłębienie dotyczy właśnie miejsca, w którym ukrywa się realna władza.

## Slajd 120 — Kto może zatrzymać system?

W projekcie chcę znać nazwisko osoby, która może zatrzymać automatyzację. Właściciel procesu opisuje próg eskalacji i tryb ręcznego przejęcia. IT przydziela konkretne uprawnienia, a dziennik zachowuje źródło, wersję i zatwierdzenie. Koordynator po przekroczeniu progu przełącza proces na pracę ręczną. Powiedzcie, kto może potem przywrócić automatyzację i jakiego dowodu będzie potrzebował.

## Slajd 121 — Władza ukrywa się w możliwości odmowy

Załóżmy, że klient otrzymuje szczegółowe wyjaśnienie wyniku scoringu. Dowiaduje się, które dane miały znaczenie. Zauważa jednak błąd i nie ma żadnej skutecznej ścieżki jego poprawienia. Czy możemy powiedzieć, że dzięki przejrzystości odzyskał kontrolę?

Otrzymał wiedzę o decyzji, ale nie możliwość wpłynięcia na jej podstawę. To ważne rozróżnienie. Władza leży często po stronie tego, kto może zmienić cel systemu, poprawić dane, wyłączyć rozwiązanie albo przyznać wyjątek.

Przy wdrożeniu warto więc narysować rzeczywisty podział uprawnień. Co może dostawca modelu, co organizacja wdrażająca, co operator, a co osoba oceniana? Kto może odmówić i jakie poniesie konsekwencje? Odpowiedzi bywają ważniejsze dla autonomii człowieka niż sam poziom technicznej przejrzystości.

Jeszcze głębiej: możliwość odmowy pokazuje, czy relacja z systemem jest rzeczywiście wyborem. Jeżeli odmowa oznacza utratę dostępu do podstawowej usługi, formalna zgoda może być bardzo słaba jako dowód dobrowolności. Technologia potrafi ukryć tę relację pod neutralnym językiem procesu. Wynik pojawia się jako liczba, więc wygląda jak konieczność, choć za nim stoi projekt organizacji i jej decyzja o stosowaniu określonego kryterium. Pytanie „kto może powiedzieć nie?” pozwala odzyskać widoczność tych decyzji i przypomnieć, że architektura systemu obejmuje również architekturę uprawnień.

Realna możliwość sprzeciwu wymaga także kosztu, który człowiek jest w stanie ponieść. Odwołanie istniejące tylko na papierze może być bezużyteczne, jeśli wymaga wiedzy, czasu i dokumentów niedostępnych osobie ocenianej. Dlatego ocena kontroli powinna obejmować jej praktyczną dostępność. Kto z niej korzysta, kto odpada po drodze i czy organizacja uczy się z zasadnych odwołań? Możliwość korekty jest szczególnie ważna dlatego, że systemy mogą działać w wielkiej skali. Niewielka częstość błędu nie oznacza niewielkiej liczby ludzkich historii. Skala sukcesu i skala szkody mogą rosnąć równocześnie.

Zobaczmy teraz, jak prawo próbuje uporządkować część tych ryzyk.

## Slajd 122 — AI Act: logika ryzyka

AI Act porządkuje obowiązki według ryzyka i przeznaczenia systemu. Rozróżnia praktyki objęte zakazami, wybrane zastosowania wysokiego ryzyka oraz obowiązki przejrzystości. Osobny zestaw zasad dotyczy modeli ogólnego przeznaczenia.

Ta sama rodzina technologii może mieć różne znaczenie prawne zależnie od użycia. Dlatego nazwę modelu trzeba uzupełnić opisem funkcji, roli organizacji i skutków dla ludzi. Samo zapewnienie, że człowiek coś zatwierdza, nie rozstrzyga automatycznie kwalifikacji.

Harmonogram zawiera wyjątki i zmiany, więc dla konkretnego wdrożenia trzeba sięgnąć do aktualnego tekstu oraz wytycznych. Ten slajd przedstawia logikę regulacji, nie kompletną instrukcję zgodności. AI Act nie zastępuje RODO, prawa autorskiego ani przepisów sektorowych. Potrzebujemy całościowej oceny sytuacji, a nie jednego znaku jakości przy nazwie produktu.

Głębszy sens regulacji polega na przypomnieniu, że ryzyka nie można oceniać w oderwaniu od zastosowania. System o podobnej konstrukcji może służyć zabawie albo wpływać na dostęp do ważnych zasobów. Odpowiedzialność zaczyna się więc od dokładnego opisu funkcji i skutków, zanim pojawi się lista obowiązków.

O możliwościach i ryzyku decydują również zasoby oraz zależności między organizacjami.

## Slajd 123 — Dylemat Collingridge’a

Na początku możemy zmienić system małym kosztem, ale znamy niewiele skutków jego działania. Później skutki stają się widoczne, a firma ma już integracje, przeszkolonych ludzi i procedury zależne od systemu. To dylemat Collingridge’a. Krótki pilotaż z możliwością powrotu do poprzedniej procedury daje czas na zdobycie informacji przed szerszym wdrożeniem.

## Slajd 124 — Zasoby i geopolityka

Rozwój AI wymaga infrastruktury: obliczeń, danych, energii i kompetencji. Dostęp do tych zasobów wpływa na to, kto może prowadzić badania, wdrażać systemy i niezależnie je sprawdzać.

Również otwartość ma kilka wymiarów. Możemy mieć dostęp do wag, ale nie do pełnej historii danych. Możemy widzieć kod, a jednocześnie podlegać warunkom licencji ograniczającym użycie. Hasło „otwarty model” warto więc zawsze rozwinąć: co dokładnie jest dostępne i na jakich zasadach?

Przy ocenie kosztu środowiskowego także potrzebujemy warunków pomiaru. Nie ma jednej sensownej liczby energii dla dowolnego zapytania. Znaczenie mają model, sprzęt, długość operacji i infrastruktura. Dokładność porównania wymaga określenia, co wliczamy do bilansu i z jaką alternatywą porównujemy system.

Zależność od dostawcy ma wymiar poznawczy. Jeśli tylko jedna organizacja potrafi odtworzyć działanie systemu, inni mogą być zmuszeni ufać jej opisowi własnych wyników. Możliwość zmiany dostawcy, audytu i niezależnej oceny wpływa więc nie tylko na cenę, ale również na to, kto ma prawo skutecznie podważyć twierdzenie o jakości.

Na tym tle możemy ostrożniej rozmawiać o świadomości i przyszłości.

## Slajd 125 — Praca, informacja i skala wpływu

Spójrzmy na stanowisko jak na zbiór zadań. AI może przyspieszyć sporządzanie szkiców, a jednocześnie zwiększyć zapotrzebowanie na sprawdzanie ich źródeł. Podobny efekt widzimy w obiegu informacji: tanie generowanie zwiększa podaż dobrych i mylących treści. O wyniku dla firmy decyduje między innymi to, czy potrafi wychwycić różnicę.

## Slajd 126 — Przyszłość i granice kontroli

Na koniec popatrzymy na kilka możliwych kierunków rozwoju AI. Sięgniemy również po literaturę, bo pomaga sformułować pytania o cele i kontrolę. Potem wrócimy do jednej decyzji o wdrożeniu, którą da się uzasadnić tu i teraz.

## Slajd 127 — Lem: inteligencja i rozminięcie celów

W Golemie XIV Lem pozwala wyobrazić sobie inteligencję, której priorytety rozmijają się z ludzkimi. Ta sytuacja stawia ciekawe pytanie projektowe. Zwiększenie zdolności systemu do realizacji celu od razu podnosi stawkę pytania, kto określił ów cel i jak można go skorygować.

## Slajd 128 — Samodoskonalenie i granice przewidywania

Good rozważa możliwość, że sprawna maszyna pomoże w budowie jeszcze sprawniejszej maszyny. W kolejnej rundzie ta nowa maszyna mogłaby przyspieszyć dalszą pracę. Tempo takiej pętli zależałoby od obliczeń, danych, możliwości eksperymentowania i weryfikacji kolejnych projektów. Traktujemy to jako hipotezę mechanizmu, której założenia możemy rozłożyć na części.

## Slajd 129 — Scenariusze przyszłości

Możemy wyobrazić sobie rozwój, w którym AI zwiększa dostęp do wiedzy i usług, wspiera pracę oraz pomaga rozwiązywać trudne problemy. Możemy też obserwować proces koncentracji korzyści u właścicieli infrastruktury i rosnącą zależność innych organizacji.

Jeszcze inny wymiar to kruchość: wiele procesów może opierać się na podobnych systemach i powielać ich błędy. Równolegle instytucje mogą wzmacniać audyt, edukację i mechanizmy korekty. Te scenariusze nie są rozłączne. Mogą rozwijać się jednocześnie w różnych obszarach.

Nie przypisuję im tu arbitralnych prawdopodobieństw ani dat. Proponuję inne pytanie: jakie obserwowalne sygnały wskazywałyby, że dany proces nabiera znaczenia? I jakie dzisiejsze decyzje pomagają zachować możliwość działania, jeśli przyszłość okaże się inna niż nasze oczekiwania?

Scenariusz jest narzędziem badania odporności własnych planów. Nie musi przepowiadać świata, żeby być użyteczny. Może ujawnić zależność, której wcześniej nie zauważaliśmy: od jednego dostawcy, jednego źródła danych albo jednego sposobu oceny. Czasem najcenniejszym wynikiem myślenia o przyszłości jest rozpoznanie, z czego nie warto rezygnować już dziś.

Na koniec przełóżmy wszystkie te rozróżnienia na prosty sposób rozpoczynania projektu AI.

## Slajd 130 — Projekt AI zaczyna się od problemu

Projekt AI powinien zaczynać się od opisu problemu i pożądanej zmiany. Jaki wynik ma się poprawić i po czym poznamy, że się poprawił? Z czym porównamy rozwiązanie: z obecnym procesem, prostą regułą czy innym modelem?

Następnie pytamy o dane i sens celu. Skąd pochodzą przykłady? Co oznacza etykieta? Jakie osoby albo warunki są pominięte? Potem projektujemy test odpowiadający rzeczywistemu wdrożeniu i ustalamy koszt różnych pomyłek.

Na końcu potrzebujemy odpowiedzialności operacyjnej: kto obserwuje jakość po wdrożeniu, kto może zatrzymać system i jak wrócimy do działania, jeśli rozwiązanie okaże się błędne. Te pytania warto zadać przed wyborem architektury. Czasem odpowiedź pokaże, że AI jest potrzebna. Czasem, że problem lepiej rozwiązać inaczej.

Najważniejszy rezultat wstępnej analizy może polegać na zmianie samego pytania. Organizacja przychodzi po automatyzację odpowiedzi, a odkrywa, że główny problem tkwi w niespójnych dokumentach. Albo chce przewidywać awarie, choć nie ma możliwości reagowania na alarm. Rozpoznanie takiego ograniczenia jest postępem, nawet jeśli nie kończy się treningiem modelu.

Sprawdźmy ten sposób myślenia w krótkim warsztacie o tutorze AI.

## Slajd 131 — Ile daje automatyzacja ofertowania?

Załóżmy czterysta ofert miesięcznie i dwanaście minut oszczędności na każdej. To osiemdziesiąt godzin. Jeśli potrafimy zagospodarować ten czas po sto złotych za godzinę, odzyskujemy osiem tysięcy złotych wartości. Po odjęciu trzech tysięcy na weryfikację i utrzymanie zostaje pięć tysięcy miesięcznie. Przy koszcie startowym trzydziestu tysięcy prosty okres zwrotu wynosi sześć miesięcy. Sprawdźmy teraz, jak zmieni się decyzja, jeśli wykorzystamy tylko połowę odzyskanego czasu.

*[Po odpowiedziach: Wtedy zostaje tysiąc złotych miesięcznie, a prosty zwrot wydłuża się do trzydziestu miesięcy.]*

## Slajd 132 — Warsztat końcowy: tutor AI

Uczelnia chce wdrożyć tutora AI. Załóżmy, że celem jest pomoc w nauce, ale na razie nie ma dokładnej definicji sukcesu. Proszę w małych grupach zaproponować, co należałoby zmierzyć.

Warto rozróżnić zadowolenie z rozmowy, zakończenie zadania i trwałe opanowanie umiejętności. Można korzystać z każdego z tych pomiarów, ale nie należy zastępować jednego drugim bez uzasadnienia. Zastanówmy się również, czy efekt utrzymuje się bez asystenta i po pewnym czasie.

Kolejne pytania dotyczą danych i kontroli. Co tutor musi wiedzieć o uczniu, a czego nie potrzebuje? Jak sprawdzimy błędne wyjaśnienia? Kiedy powinien poprosić o własną próbę? Kto zajmie się przypadkiem, w którym system uporczywie wprowadza w błąd? Po pracy porównamy projekty właśnie według tych kryteriów.

Nie szukamy jednego uniwersalnego tutora. Szukamy projektu, którego cel, pomiar i sposób działania są ze sobą zgodne. Jeśli jedna grupa proponuje więcej samodzielnej pracy, a druga szybsze ukończenie kursu, to mogą być różne uzasadnione cele. Trzeba jednak jawnie powiedzieć, jaki kompromis wybieramy i dla kogo będzie on korzystny.

Po tym ćwiczeniu zbierzmy pięć myśli, które warto zabrać z całego wykładu.

## Slajd 133 — Zarząd decyduje o pilotażu

Macie dwanaście minut. Wybierzcie proces i wskażcie osobę, która odpowiada za jego wynik. Opiszcie jedną decyzję wspieraną przez system i pomiar bazowy. Zdecydujcie, jakie sprawy wejdą do próby, co uznacie za sukces i kiedy przerwiecie pilotaż. Policzcie koszt i porównajcie projekt ze zmianą samej procedury. Oddajcie jedną stronę z rekomendacją, którą moglibyście przedłożyć zarządowi.

## Slajd 134 — Pięć rzeczy do zapamiętania

Po pierwsze, cel i etykiety określają, czego model ma się uczyć. Jeżeli źle opiszemy sens zadania, większy model może jedynie skuteczniej realizować niewłaściwe przybliżenie.

Po drugie, generalizacja wymaga uczciwego testu. Dobry wynik musi odnosić się do rodzaju nowości, który rzeczywiście spotkamy po wdrożeniu. Po trzecie, płynność odpowiedzi nie gwarantuje prawdziwości. Potrzebujemy sprawdzenia źródeł, warunków i drogi do wniosku.

Po czwarte, model może zmieniać zachowania ludzi i dane, z których później będzie się uczyć. Nie zawsze obserwuje świat z zewnątrz. Po piąte, odpowiedzialność wymaga realnej możliwości korekty. Człowiek musi móc poprawić dane, zakwestionować decyzję albo zatrzymać niebezpieczny proces. Sama deklaracja nadzoru jest za słaba.

Te pięć punktów łączy jedno pytanie: co musi być prawdą, żeby nasz wniosek o jakości systemu był uzasadniony? AI bywa imponująca, ale dojrzała ocena zaczyna się tam, gdzie potrafimy nazwać warunki własnego zachwytu. Wtedy technologia staje się przedmiotem wiedzy i projektowania, a nie tylko wiary lub lęku.

Na zakończenie zostawię Państwu jedno pytanie, które wykracza poza wybór konkretnego modelu.

## Slajd 135 — Kiedy ofertowanie przechodzi do wdrożenia?

Przed startem mierzę medianę czasu przygotowania oferty i odsetek istotnych korekt. Przez cztery tygodnie porównuję podobne typy spraw. Handlowcy oceniają je według tej samej rubryki. Chcemy zejść z medianą czasu o co najmniej jedną czwartą, utrzymując jakość. Błędna cena wysłana klientowi od razu wstrzymuje pilotaż. Przy małej liczbie spraw zbieram dalsze obserwacje przed decyzją.

## Slajd 136 — Pytania, które zostają

Co chcemy oddać maszynom, a za co chcemy nadal odpowiadać? Nie pytam tylko o listę czynności. Pytam o to, jaką relację z technologią chcemy budować i jakie kompetencje chcemy zachować.

Możemy oddać systemowi wyszukiwanie wariantów, a zachować decyzję o kryteriach. Możemy korzystać z prognozy, a nadal wymagać uzasadnienia działania. Możemy przyjmować pomoc w nauce, a jednocześnie ćwiczyć samodzielne rozumowanie. Każdy z tych wyborów wymaga świadomego projektu.

Chciałbym, żeby po wykładzie została Państwu ciekawość połączona z precyzją. Ciekawość pozwala zobaczyć nowe możliwości. Precyzja przypomina, że możliwość nie jest jeszcze dowodem użyteczności, a użyteczność nie rozstrzyga wszystkich pytań o odpowiedzialność. Dziękuję. Jestem ciekaw, które z dzisiejszych rozróżnień najbardziej zmieniło Państwa sposób patrzenia na AI.

Być może najważniejszą kompetencją przyszłości będzie zdolność pozostawania autorem pytania. System może pomagać w odpowiedzi, ale wybór tego, o co warto pytać, czego nie wolno poświęcić i kiedy należy się zatrzymać, nadal potrzebuje uzasadnienia wobec innych ludzi. Delegowanie operacji nie musi oznaczać delegowania sensu.

Na dwóch ostatnich slajdach zostawiam materiały dla osób, które chcą pójść dalej.

## Slajd 137 — Źródła: mechanizmy i historia

Ta część bibliografii prowadzi do podstaw mechanizmów i historii. Tekst Turinga pomaga zobaczyć, jak wcześnie pojawiło się pytanie o obserwowalne kryteria inteligencji. Propozycja Dartmouth pokazuje ambicję programu badawczego, z którego wyrosła nazwana dziedzina.

Praca o propagacji błędu i podręcznik Deep Learning pozwalają wejść głębiej w uczenie reprezentacji. Książka Suttona i Barto porządkuje uczenie ze wzmocnieniem, a „Attention Is All You Need” przedstawia transformera w oryginalnej postaci badawczej.

Nie sugeruję czytania wszystkich tych tekstów jednocześnie ani w kolejności od najtrudniejszego. Warto zacząć od pytania, które naprawdę nas interesuje, i przejść od intuicji do precyzyjnego opisu. Sięganie do źródeł ma pokazać także warunki i ograniczenia twierdzeń, które w popularnych opisach stają się krótkimi hasłami.

Czytanie źródła jest sposobem odzyskiwania szczegółów utraconych w opowieści o przełomie. Widzimy konkretne zadanie, dane i sposób porównania. Dzięki temu możemy docenić osiągnięcie bez przypisywania mu szerszej mocy, niż rzeczywiście wykazano. To jedna z najbardziej praktycznych form krytycznego myślenia o AI.

Druga grupa źródeł dotyczy zastosowań, bezpieczeństwa i odpowiedzialności.

## Slajd 138 — Źródła: zastosowania i odpowiedzialność

Tutaj znajdą Państwo przykłady badań i ram służących ocenie konsekwencji AI. Praca o AlphaFold pokazuje konkretne osiągnięcie naukowe. „Concrete Problems in AI Safety” pomaga uporządkować problemy celu, skutków ubocznych i zachowania systemu poza oczekiwanymi warunkami.

Rekomendacja UNESCO oraz ramy NIST porządkują pytania o odpowiedzialność i zarządzanie ryzykiem. W sprawach prawnych trzeba sięgać do aktualnych źródeł Komisji Europejskiej i tekstu regulacji, ponieważ harmonogram oraz szczegółowe obowiązki wymagają bieżącego sprawdzenia.

Tekst o świadomości AI pokazuje, że trudne pytanie można badać przez jawne założenia i proponowane wskaźniki, nie udając ostatecznego rozstrzygnięcia. Dokładne linki są w notatkach prezentacji oraz na końcu tego scenariusza. Zachęcam do traktowania bibliografii jako mapy dalszych pytań, a nie listy autorytetów zamykających dyskusję.

Źródło jest wartościowe wtedy, gdy pozwala sprawdzić twierdzenie. Dlatego ostatnią myślą niech będzie konsekwencja wobec własnych standardów: także słowa prowadzącego powinny podlegać weryfikacji. Dobry wykład nie wymaga bezwarunkowego zaufania. Daje słuchaczom narzędzia do samodzielnego sprawdzenia, z czym warto się zgodzić i dlaczego.

Dziękuję za wspólną pracę. Oddaję głos Państwa pytaniom.

## Slajd 139 — Źródła pogłębień

Tutaj zostawiam lektury do pogłębienia. Searle, Harnad i Polanyi pomagają zrozumieć spory o znaczenie i wiedzę. Badania nad skalowaniem i wrażliwością modeli rozwijają tematy techniczne. Lem, Good i Vinge prowokują do namysłu nad przyszłością. Czytajmy je z uwagą na to, czy autor przedstawia wynik badania, argument czy scenariusz.

## Slajd 140 — AI Mastery: program studiów (1/2)

Na końcu zostawiam pierwszą część programu AI Mastery. Można ją potraktować jako mapę tematów, do których dzisiejszy wykład daje podstawę. Dla Państwa szczególnie ważne będzie przełożenie tych mechanizmów na decyzje o procesie, kosztach i odpowiedzialności.

## Slajd 141 — AI Mastery: program studiów (2/2)

Tu jest druga część programu. Na koniec proszę pomyśleć o jednym procesie z Państwa organizacji. Gdybyśmy jutro mieli sprawdzić, czy AI rzeczywiście tam pomaga, jaki pomiar zrobilibyśmy jako pierwszy? Dziękuję Państwu.
