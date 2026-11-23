# Notatki prowadzącego: Historia AI, algorytmy ML i sieci neuronowe

Marcin Albiniak, Ph.D. | COMARCH | 23–26 listopada 2026

Notatki są także zapisane bezpośrednio w prezentacji PowerPoint.

## Slajd 01. Od idei inteligencji do sieci neuronowych

**Co mówić:**

Otwarcie. Na tym szkoleniu nie będziemy utożsamiać sztucznej inteligencji z jednym produktem, modelem językowym ani biblioteką. Zaczniemy od pytania, skąd wzięła się sama idea inteligentnych maszyn. Następnie przełożymy tę historię na działanie konkretnych algorytmów Machine Learning oraz sieci neuronowych. Zobaczymy, gdzie matematyka wyznacza granice generalizacji, a gdzie architektura sieci pozwala budować coraz bogatsze reprezentacje.

## Slajd 02. AI nie jest jednym algorytmem

**Co mówić:**

Zacznij od prostego ćwiczenia. Zapytaj grupę, czy program grający w szachy, system punktacji kredytowej oraz chatbot są podobną technologią. Wszystkie mogą być określane jako AI, ale działają inaczej. Dlatego definicja AI musi opisywać klasę systemów, a nie jeden trik.
PUNKTY DO ROZWINIĘCIA: Po 1: To samo zadanie można rozwiązać regułami, statystyką lub siecią.. Po 2: Nie każdy system AI jest modelem uczonym na danych.. Po 3: Nie każda poprawna odpowiedź dowodzi rozumienia.. Po 4: Warto oddzielać kompetencję, mechanizm i autonomię..
AKCENT DLA GRUPY: TEZA: OCENIAJ DZIAŁANIE, A NIE ETYKIETĘ „AI”.
Wskazówka dla trenera: Nie czytaj punktów. Zacznij od problemu, a potem skonfrontuj przykład z mechanizmem algorytmu.

## Slajd 03. Agenda: cztery filary rozumienia AI

**Co mówić:**

Wyjaśnij cel każdego bloku. Moduł pierwszy daje język i historię. Drugi odpowiada na pytanie, co znaczy uczyć się z danych. Trzeci pokazuje konkretne klasy algorytmów i zasady doboru. Czwarty otwiera czarną skrzynkę sieci neuronowych: od pojedynczej operacji sumy ważonej po backpropagation, konwolucję i uwagę. Materiał jest celowo niezależny od narzędzi instalacyjnych oraz konkretnych bibliotek.

## Slajd 04. Pięć pytań, które będziemy zadawać modelom

**Co mówić:**

Ta lista porządkuje całe szkolenie. Wiele prezentacji AI skupia się na możliwościach systemów, ale techniczne rozumienie zaczyna się od funkcji celu, reprezentacji i sposobu walidacji. Zachęć do notowania tych pięciu pytań. Wrócimy do nich przy regresji, SVM, drzewach i sieciach neuronowych.
PUNKTY DO ROZWINIĘCIA: Po 1: Jaki problem matematyczny rozwiązujemy?. Po 2: Co jest wejściem, a co przewidywanym wyjściem?. Po 3: Jak model tworzy reprezentację i dopasowuje parametry?. Po 4: Jak mierzymy błąd i jakość generalizacji?. Po 5: Kiedy wynik może być wiarygodny poza treningiem?.
AKCENT DLA GRUPY: WYNIK BEZ KONTROLI BŁĘDU TO TYLKO DEMONSTRACJA.
Wskazówka dla trenera: Nie czytaj punktów. Zacznij od problemu, a potem skonfrontuj przykład z mechanizmem algorytmu.

## Slajd 05. Jak powstała idea maszynowego wnioskowania i co dziś oznacza „inteligentne działanie”?

**Co mówić:**

Otwarcie modułu 1: Historia i natura AI. Jak powstała idea maszynowego wnioskowania i co dziś oznacza „inteligentne działanie”? Przeprowadź uczestników od intuicyjnego obrazu problemu do technicznego modelu. Zaznacz, że moduł ma wyraźny cel i będzie łączył historię, matematykę, metodę eksperymentalną oraz konsekwencje wdrożeniowe.

## Slajd 06. Co właściwie znaczy „sztuczna inteligencja”?

**Co mówić:**

Wspomnij definicję OECD i bliską jej logikę AI Act. Cechą istotną jest mechanizm inferencji oraz rodzaj wyniku, nie koniecznie imitowanie człowieka. Klasyczne systemy oparte na wiedzy również należą do historii AI. Model, system, aplikacja i agent to różne poziomy opisu. Źródło: https://oecd.ai/en/ai-principles
PUNKTY DO ROZWINIĘCIA: Po 1: System przyjmuje informacje o stanie świata lub zadaniu.. Po 2: Na podstawie modelu lub wiedzy wyprowadza rezultat.. Po 3: Rezultat może być predykcją, treścią, rekomendacją lub decyzją.. Po 4: Systemy różnią się autonomią i możliwością adaptacji..
AKCENT DLA GRUPY: DEFINICJA SYSTEMU ≠ TEZA O ŚWIADOMOŚCI.
Wskazówka dla trenera: Nie czytaj punktów. Zacznij od problemu, a potem skonfrontuj przykład z mechanizmem algorytmu.

## Slajd 07. Od percepcji do działania: pięć funkcji inteligencji

**Co mówić:**

Przedstaw schemat jako mapę funkcjonalną, nie biologiczną. Niektóre systemy AI tylko klasyfikują, inne generują plan, a jeszcze inne podejmują działania przez narzędzia. To, że system ma pięć modułów podobnych do funkcji poznawczych, nie oznacza, że posiada doświadczenie wewnętrzne. Najważniejszą kategorią jest sprawdzalny rezultat i proces jego powstania.
PUNKTY DO ROZWINIĘCIA: Po 1: Percepcja: rejestrowanie i kodowanie sygnałów.. Po 2: Reprezentacja: wybór cech, pojęć i zależności.. Po 3: Wnioskowanie: oszacowanie lub wyprowadzenie wniosku.. Po 4: Decyzja i działanie: wybór odpowiedzi pod ograniczeniami.. Po 5: Uczenie: korekta modelu po doświadczeniu lub informacji zwrotnej..
AKCENT DLA GRUPY: Zapytaj uczestników o zastosowanie, w którym to rozróżnienie ma znaczenie.
Wskazówka dla trenera: Nie czytaj punktów. Zacznij od problemu, a potem skonfrontuj przykład z mechanizmem algorytmu.

## Slajd 08. AI a zwykła automatyzacja

**Co mówić:**

Podaj system wystawiania faktury jako zwykłą automatyzację. Ekspercki system reguł diagnostycznych to przykład symbolicznego wnioskowania. Model wykrywający anomalię w transakcjach uczy się statystycznych wzorców. W praktyce granice bywają mieszane: hybrydowe systemy łączą uczenie oraz reguły biznesowe. Uwaga: nie upraszczaj do hasła, że AI zawsze musi się uczyć podczas pracy.
PUNKTY DO ROZWINIĘCIA: Po 1: Automatyzacja: krok A zawsze uruchamia dokładnie krok B.. Po 2: AI symboliczna: wniosek wyprowadzany z wiedzy i reguł.. Po 3: ML: parametry lub struktura powstają przez dopasowanie do danych.. Po 4: Generatywna AI: konstruuje nowe wyjścia z wyuczonego rozkładu..
AKCENT DLA GRUPY: JEŚLI SYSTEM TYLKO ODTWARZA RĘCZNIE OPISANE KROKI, NIE MUSI BYĆ AI.
Wskazówka dla trenera: Nie czytaj punktów. Zacznij od problemu, a potem skonfrontuj przykład z mechanizmem algorytmu.

## Slajd 09. Trzy wielkie tradycje sztucznej inteligencji

**Co mówić:**

Narysuj w wyobraźni trzy architektury. W AI symbolicznej człowiek wprowadza reguły, a maszyna wykonuje inferencję. W statystycznej definiujemy klasę modeli i funkcję straty, ucząc parametry z próbek. W neuronowej wielu lokalnym operacjom składania towarzyszy uczenie reprezentacji. Obecne wdrożenia często łączą te podejścia zamiast wyłącznie konkurować między nimi.
PUNKTY DO ROZWINIĘCIA: Po 1: Symboliczna: pojęcia, logika, relacje i reguły.. Po 2: Statystyczna: estymacja, prawdopodobieństwo i optymalizacja.. Po 3: Neuronowa: rozproszone reprezentacje i uczenie gradientowe.. Po 4: Hybrydowa: wiedza jawna połączona z modelami wyuczonymi..
AKCENT DLA GRUPY: Zapytaj uczestników o zastosowanie, w którym to rozróżnienie ma znaczenie.
Wskazówka dla trenera: Nie czytaj punktów. Zacznij od problemu, a potem skonfrontuj przykład z mechanizmem algorytmu.

## Slajd 10. AI, Machine Learning, Deep Learning, generatywność

**Co mówić:**

Użyj schematu jako przybliżonej mapy dzisiejszych technologii. Przykład: proste drzewo decyzyjne może być ML bez Deep Learning. CNN należy do Deep Learning. Transformer generujący tekst jest współczesnym przykładem generatywnej AI. Samo pojęcie „generatywność” jest jednak szersze, więc zbiory na diagramie trzeba rozumieć dydaktycznie, nie jako absolutną klasyfikację matematyczną.
PUNKTY DO ROZWINIĘCIA: Po 1: AI to najszersza rodzina technik i systemów.. Po 2: Machine Learning dotyczy uczenia z danych lub doświadczenia.. Po 3: Deep Learning uczy wielopoziomowe reprezentacje przez sieci.. Po 4: Generatywność opisuje zadanie wytwarzania wyjść, a nie jedną architekturę..
AKCENT DLA GRUPY: Zapytaj uczestników o zastosowanie, w którym to rozróżnienie ma znaczenie.
Wskazówka dla trenera: Nie czytaj punktów. Zacznij od problemu, a potem skonfrontuj przykład z mechanizmem algorytmu.

## Slajd 11. Czy zachowanie inteligentne oznacza rozumienie?

**Co mówić:**

Przeprowadź rozróżnienie między wynikiem działania a charakterem wewnętrznego doświadczenia. Test sprawności językowej może pokazywać kompetencję, ale nie rozwiązuje filozoficznego problemu świadomości. Zadaj pytanie o samolot: lata, lecz nie macha skrzydłami jak ptak. Analogicznie inteligentne działanie nie wymusza wiernego odtwarzania biologicznego mechanizmu.
PUNKTY DO ROZWINIĘCIA: Po 1: Funkcjonalnie: czy system potrafi wykonać zadanie?. Po 2: Poznawczo: jak reprezentuje informację i wykorzystuje kontekst?. Po 3: Fenomenalnie: czy istnieje subiektywne doświadczenie?. Po 4: Wysoka sprawność w zadaniu nie przesądza pozostałych poziomów..
AKCENT DLA GRUPY: KOMPETENCJA ≠ AUTOMATYCZNY DOWÓD ŚWIADOMOŚCI.
Wskazówka dla trenera: Nie czytaj punktów. Zacznij od problemu, a potem skonfrontuj przykład z mechanizmem algorytmu.

## Slajd 12. 1943: neuron jako układ logiczny

**Co mówić:**

W 1943 Warren McCulloch i Walter Pitts przedstawili formalny neuron. Podkreśl, że ich zadaniem było pytanie o moc obliczeniową sieci prostych elementów, a nie skuteczne trenowanie neuronów na ogromnych zbiorach obrazów. Współczesne neurony są różniczkowalne i uczą się wag. Źródło: https://bnaskrecki.faculty.wmi.amu.edu.pl/nnets/_build/html/part1_origins/ch01_mcculloch_pitts.html
PUNKTY DO ROZWINIĘCIA: Po 1: Wejścia są sumowane i porównywane z progiem.. Po 2: Połączenia elementów realizują funkcje logiczne.. Po 3: Powstaje formalny pomost między neuronem i obliczeniem.. Po 4: To model koncepcyjny; nie współczesne uczenie wielowarstwowe..
AKCENT DLA GRUPY: Zapytaj uczestników o zastosowanie, w którym to rozróżnienie ma znaczenie.
Wskazówka dla trenera: Nie czytaj punktów. Zacznij od problemu, a potem skonfrontuj przykład z mechanizmem algorytmu.

## Slajd 13. 1950: Alan Turing zmienia pytanie

**Co mówić:**

Wyjaśnij kontekst artykułu „Computing Machinery and Intelligence” z 1950 roku. Turing nie dostarczył definicji świadomości, lecz stworzył ramy praktycznego pytania, które można sprawdzać. Przytocz bez cytatu dosłownego istotę propozycji. Porównaj do dzisiejszego benchmarku: dobry wynik jest evidencją sprawności w pewnym protokole, a nie dowodem zrozumienia świata w każdym kontekście. Źródło: https://academic.oup.com/mind/article/LIX/236/433/986238
PUNKTY DO ROZWINIĘCIA: Po 1: Turing proponuje grę w naśladownictwo.. Po 2: Kryterium dotyczy jakości zachowania w określonych warunkach.. Po 3: Test nie rozstrzyga, z czego składa się wewnętrzny mechanizm.. Po 4: Dziś ocena AI wymaga wielu osobnych testów, nie jednej rozmowy..
AKCENT DLA GRUPY: Zapytaj uczestników o zastosowanie, w którym to rozróżnienie ma znaczenie.
Wskazówka dla trenera: Nie czytaj punktów. Zacznij od problemu, a potem skonfrontuj przykład z mechanizmem algorytmu.

## Slajd 14. 1956: Dartmouth i narodziny nazwy „AI”

**Co mówić:**

Wspomnij wniosek na Dartmouth Summer Research Project on Artificial Intelligence z 1955 i konferencję w 1956 roku. To ważny moment dla nazewnictwa dyscypliny, nie dosłownie pierwszy komputer wykonujący inteligentne zadanie. Zwróć uwagę na optymizm, który wróci potem w kolejnych falach AI. Źródło: https://www-formal.stanford.edu/jmc/history/dartmouth.pdf
PUNKTY DO ROZWINIĘCIA: Po 1: John McCarthy i współautorzy proponują letnie badania.. Po 2: Powstaje wspólna nazwa dla bardzo różnych ambicji badawczych.. Po 3: Optymizm zderza się z trudnością otwartego świata.. Po 4: Historia AI od początku jest historią hipotez i korekt..
AKCENT DLA GRUPY: Zapytaj uczestników o zastosowanie, w którym to rozróżnienie ma znaczenie.
Wskazówka dla trenera: Nie czytaj punktów. Zacznij od problemu, a potem skonfrontuj przykład z mechanizmem algorytmu.

## Slajd 15. 1958–1986: perceptron, kryzys i powrót uczenia

**Co mówić:**

Pokaż intuicję ograniczenia pojedynczej hiperpowierzchni liniowej. XOR jest prostym przykładem danych nieoddzielnych liniowo w surowej reprezentacji. Z jednej strony ograniczenia sprzętowe, z drugiej problemy optymalizacji hamowały postęp. W 1986 Rumelhart, Hinton i Williams spopularyzowali procedurę efektywnego liczenia gradientów w sieciach wielowarstwowych. Źródło: https://web.stanford.edu/~jurafsky/slp3/
PUNKTY DO ROZWINIĘCIA: Po 1: Perceptron Rosenblatta uczy się liniowej granicy decyzyjnej.. Po 2: Pojedyncza warstwa nie rozwiąże problemu XOR bez transformacji cech.. Po 3: Wielowarstwowość daje większą klasę funkcji.. Po 4: Backpropagation rozpowszechnia praktyczną naukę wag w sieciach..
AKCENT DLA GRUPY: Zapytaj uczestników o zastosowanie, w którym to rozróżnienie ma znaczenie.
Wskazówka dla trenera: Nie czytaj punktów. Zacznij od problemu, a potem skonfrontuj przykład z mechanizmem algorytmu.

## Slajd 16. Systemy eksperckie i zimy AI

**Co mówić:**

Wyjaśnij problem wąskiego zakresu i ręcznego utrzymania wiedzy. System może działać imponująco w ustalonym środowisku, ale źle reagować na nowe przypadki. To istotne ostrzeżenie dla współczesnych wdrożeń: bogata demonstracja produktu nie oznacza odpornego systemu. Wspomnij, że w historii AI występowały różne okresy spadku finansowania, a prace nad algorytmami trwały także poza nimi.
PUNKTY DO ROZWINIĘCIA: Po 1: Wiedza eksperta jest kodowana jako jawne reguły.. Po 2: Baza reguł staje się kosztowna i krucha przy wyjątkach.. Po 3: Oczekiwania biznesowe wyprzedzają rzeczywiste możliwości.. Po 4: „Zima AI” to spadek finansowania i wiary, nie brak badań..
AKCENT DLA GRUPY: Zapytaj uczestników o zastosowanie, w którym to rozróżnienie ma znaczenie.
Wskazówka dla trenera: Nie czytaj punktów. Zacznij od problemu, a potem skonfrontuj przykład z mechanizmem algorytmu.

## Slajd 17. 1997–2012: od wyszukiwania do głębokiego rozpoznawania

**Co mówić:**

Deep Blue z 1997 roku jest dobrym kontrprzykładem tezy, że każdy przełom AI wynika z sieci neuronowych. Później AlexNet, pokazany w konkursie ImageNet w 2012 roku, przyspieszył renesans Deep Learning, zwłaszcza w rozpoznawaniu obrazów. To różne narzędzia na inne problemy. Źródła: https://www.ibm.com/history/deep-blue oraz https://dl.acm.org/doi/10.1145/3065386
PUNKTY DO ROZWINIĘCIA: Po 1: Deep Blue wygrywa z Kasparowem dzięki wyszukiwaniu i ewaluacji pozycji.. Po 2: W 2012 AlexNet pokazuje siłę głębokiego CNN w klasyfikacji obrazów.. Po 3: Zmieniają się skala danych, obliczeń i techniki uczenia.. Po 4: Sukces w jednej domenie nie jest generalną inteligencją..
AKCENT DLA GRUPY: Zapytaj uczestników o zastosowanie, w którym to rozróżnienie ma znaczenie.
Wskazówka dla trenera: Nie czytaj punktów. Zacznij od problemu, a potem skonfrontuj przykład z mechanizmem algorytmu.

## Slajd 18. 2016–2017: AlphaGo i Transformer

**Co mówić:**

AlphaGo pokonał Lee Sedola w 2016 roku; system nie był tylko jedną siecią, lecz połączeniem uczenia i wyszukiwania. W 2017 zaproponowano architekturę Transformer, która w oryginalnej pracy obywa się bez rekurencji i konwolucji przy modelowaniu sekwencji. Zwróć uwagę na różnicę między zdolnością oceny stanu, przeszukiwaniem przyszłości i modelowaniem zależności między tokenami. Źródła: https://deepmind.google/research/alphago/ oraz https://research.google/pubs/attention-is-all-you-need/
PUNKTY DO ROZWINIĘCIA: Po 1: AlphaGo łączy sieci neuronowe z algorytmami wyszukiwania.. Po 2: Transformer opiera reprezentacje na mechanizmie uwagi.. Po 3: Trening na skali prowadzi do nowych klas zastosowań.. Po 4: Przełomy mają różne mechanizmy: search, gradient, attention..
AKCENT DLA GRUPY: Zapytaj uczestników o zastosowanie, w którym to rozróżnienie ma znaczenie.
Wskazówka dla trenera: Nie czytaj punktów. Zacznij od problemu, a potem skonfrontuj przykład z mechanizmem algorytmu.

## Slajd 19. Od 2022: modele fundamentalne, multimodalność i agenci

**Co mówić:**

Nie wprowadzaj mitologii, że system agentowy musi być świadomy lub posiadać własne cele. Agent to konfiguracja zdolna do kolejnych działań, korzystania z narzędzi i reagowania na wyniki. Obszar ten dynamicznie się rozwija, ale podlega tradycyjnym problemom błędów, uczenia z niewłaściwych danych i nieprzewidzianych interakcji. Nacisk jest na architekturę systemową i weryfikację.
PUNKTY DO ROZWINIĘCIA: Po 1: Modele fundamentalne można adaptować do wielu zadań.. Po 2: Multimodalność scala tekst, obraz, dźwięk i inne sygnały.. Po 3: Agenci łączą model, pamięć, narzędzia i sterowanie.. Po 4: Większa autonomia wymaga mocniejszej oceny ryzyka i procesu..
AKCENT DLA GRUPY: Zapytaj uczestników o zastosowanie, w którym to rozróżnienie ma znaczenie.
Wskazówka dla trenera: Nie czytaj punktów. Zacznij od problemu, a potem skonfrontuj przykład z mechanizmem algorytmu.

## Slajd 20. 80 lat AI: historia zmieniających się metod

**Co mówić:**

Zrób krótki spacer po osi czasu. Wyjaśnij, że rozwój AI nie był prostą linią ulepszania jednego algorytmu. W latach 50. ścierały się tradycje symboliczna i neuronowa. W latach 80. wróciło uczenie wielowarstwowe, a później większa moc obliczeniowa i dane umożliwiły praktyczne sukcesy. Deep Blue nie był współczesną głęboką siecią neuronową, a AlphaGo łączył sieci i wyszukiwanie. Dzisiejsza agentowość to organizacja modeli i narzędzi, nie automatyczny dowód ogólnej inteligencji.

## Slajd 21. Pięć lekcji historii AI

**Co mówić:**

To slajd podsumowania historii. Poproś uczestników o wskazanie podobieństw między obietnicami stawianymi AI w latach 60. a obecnymi wyobrażeniami o pełnej automatyzacji. Obie epoki pokazują, że łatwo uogólnić sprawność z jednego zadania. Główną lekcją jest odpowiedzialne rozdzielenie demonstracji, modelu i wdrożenia.
PUNKTY DO ROZWINIĘCIA: Po 1: Wąski sukces łatwo pomylić z uniwersalną kompetencją.. Po 2: Reprezentacja problemu bywa ważniejsza niż sam algorytm.. Po 3: Dane, sprzęt i architektura zmieniają się jednocześnie.. Po 4: Systemy hybrydowe nie są odstępstwem, tylko naturalnym kierunkiem.. Po 5: Walidacja w rzeczywistym świecie pozostaje niezbędna..
AKCENT DLA GRUPY: NAJWAŻNIEJSZA: REZULTAT TRZEBA UZASADNIĆ I ZMIERZYĆ.
Wskazówka dla trenera: Nie czytaj punktów. Zacznij od problemu, a potem skonfrontuj przykład z mechanizmem algorytmu.

## Slajd 22. Od danych i reprezentacji do funkcji celu, walidacji i uogólniania.

**Co mówić:**

Otwarcie modułu 2: Jak maszyna się uczy. Od danych i reprezentacji do funkcji celu, walidacji i uogólniania. Przeprowadź uczestników od intuicyjnego obrazu problemu do technicznego modelu. Zaznacz, że moduł ma wyraźny cel i będzie łączył historię, matematykę, metodę eksperymentalną oraz konsekwencje wdrożeniowe.

## Slajd 23. Uczenie nie oznacza zapamiętywania odpowiedzi

**Co mówić:**

Rozrysuj funkcję f(x; θ). x to cechy wejściowe, θ parametry modelu, a y przewidywana odpowiedź. W treningu poszukujemy parametrów minimalizujących funkcję straty. Samo zmniejszenie błędu treningowego nie oznacza, że model będzie użyteczny. Pokaż przypadek pamięciowego klasyfikatora, który perfekcyjnie zna znane przykłady, lecz myli się na nowych.
PUNKTY DO ROZWINIĘCIA: Po 1: Dane treningowe ograniczają przestrzeń możliwych hipotez.. Po 2: Algorytm dopasowuje parametry lub strukturę modelu.. Po 3: Funkcja straty mierzy niezgodność z celem.. Po 4: Test na nowych danych sprawdza uogólnianie, nie pamięć..
AKCENT DLA GRUPY: Zapytaj uczestników o zastosowanie, w którym to rozróżnienie ma znaczenie.
Wskazówka dla trenera: Nie czytaj punktów. Zacznij od problemu, a potem skonfrontuj przykład z mechanizmem algorytmu.

## Slajd 24. Nadzorowane, nienadzorowane i uczenie ze wzmocnieniem

**Co mówić:**

Nadzorowane uczenie dobrze reprezentuje klasyfikacja spamu i prognoza ceny. Nienadzorowane dotyczy na przykład grupowania klientów. Reinforcement Learning jest związany z działaniem sekwencyjnym i nagrodą opóźnioną; nie wolno utożsamiać go z prostą klasyfikacją. Self-supervised Learning stanowi kluczowy kontekst dla modeli fundamentalnych. Podkreśl, że wybór paradygmatu wynika z rodzaju dostępnej informacji.
PUNKTY DO ROZWINIĘCIA: Po 1: Nadzorowane: przykład wejścia ma etykietę lub wartość docelową.. Po 2: Nienadzorowane: szukamy struktury bez jawnych etykiet.. Po 3: Ze wzmocnieniem: uczymy politykę na podstawie nagrody.. Po 4: Self-supervised: cel treningowy wyprowadzamy z samych danych..
AKCENT DLA GRUPY: Zapytaj uczestników o zastosowanie, w którym to rozróżnienie ma znaczenie.
Wskazówka dla trenera: Nie czytaj punktów. Zacznij od problemu, a potem skonfrontuj przykład z mechanizmem algorytmu.

## Slajd 25. Reprezentacja cech określa, czego model może się nauczyć

**Co mówić:**

Omów przykład klientów opisanych tylko wiekiem i budżetem: może brakować informacji o wcześniejszych zakupach. Dobór cech może mieć większy wpływ niż zmiana modelu. W sieciach złożone reprezentacje powstają w kolejnych warstwach, ale nadal wynikają z danych i celu optymalizacji. Zwróć uwagę, że nie wolno dopuszczać do cech informacji dostępnych dopiero po decyzji.
PUNKTY DO ROZWINIĘCIA: Po 1: Cechy to liczbowy lub strukturalny opis obiektu.. Po 2: Złe cechy ukrywają istotną zależność, dobre ją ujawniają.. Po 3: Transformacja może zamienić problem nieliniowy w prostszy.. Po 4: Sieci neuronowe uczą wiele cech automatycznie, ale nie bez ograniczeń..
AKCENT DLA GRUPY: Zapytaj uczestników o zastosowanie, w którym to rozróżnienie ma znaczenie.
Wskazówka dla trenera: Nie czytaj punktów. Zacznij od problemu, a potem skonfrontuj przykład z mechanizmem algorytmu.

## Slajd 26. Trening, walidacja, test: trzy role danych

**Co mówić:**

Podaj prosty przykład przewidywania awarii urządzeń. Gdy pomieszamy dane z przyszłości i przeszłości, test może być sztucznie łatwy. W niektórych zadaniach dzielimy także według użytkownika, urządzenia lub lokalizacji, by uniknąć bliskich duplikatów. Zwróć uwagę, że hiperparametry dobrane na zbiorze testowym powodują jego „zużycie”.
PUNKTY DO ROZWINIĘCIA: Po 1: Trening: parametry modelu dostosowują się do danych.. Po 2: Walidacja: wybieramy hiperparametry i modele.. Po 3: Test: pojedyncza, niezależna ocena jakości rozwiązania.. Po 4: W szeregach czasowych zachowujemy kierunek czasu..
AKCENT DLA GRUPY: TESTOWANIE NA DANYCH TRENINGOWYCH TO NIE WALIDACJA.
Wskazówka dla trenera: Nie czytaj punktów. Zacznij od problemu, a potem skonfrontuj przykład z mechanizmem algorytmu.

## Slajd 27. Funkcja straty: jak model wie, że się pomylił?

**Co mówić:**

Rozdziel funkcję celu od wskaźnika operacyjnego. Sieć może uczyć się cross-entropy, a firma oceniać koszt fałszywie odrzuconych wniosków. W klasyfikacji nierównych klas accuracy bywa mylące. Omów matematyczną ideę gradientu i minimum funkcji, ale nie rozwijaj tu jeszcze szczegółów backpropagation. To zapowiedź modułu czwartego.
PUNKTY DO ROZWINIĘCIA: Po 1: Regresja: często minimalizujemy średni błąd kwadratowy.. Po 2: Klasyfikacja: często stosujemy log-loss / cross-entropy.. Po 3: Regularizacja karze złożoność lub rozmiar parametrów.. Po 4: Wartość straty służy uczeniu; metryka biznesowa może być inna..
AKCENT DLA GRUPY: Zapytaj uczestników o zastosowanie, w którym to rozróżnienie ma znaczenie.
Wskazówka dla trenera: Nie czytaj punktów. Zacznij od problemu, a potem skonfrontuj przykład z mechanizmem algorytmu.

## Slajd 28. Niedouczenie i przeuczenie

**Co mówić:**

Powiedz, że mniejszy błąd treningowy nie zawsze oznacza lepszy model. Uczestnicy mogą zrozumieć trade-off przez przykład wielomianu wysokiego stopnia dopasowanego do kilku punktów. Dyskusja o bias–variance to narzędzie interpretacyjne, a nie magiczna ścisła reguła dla każdej głębokiej sieci. Pokaż, dlaczego krzywe uczenia są pomocne.
PUNKTY DO ROZWINIĘCIA: Po 1: Underfitting: model nie ujmuje nawet struktury danych treningowych.. Po 2: Overfitting: uczy się także szumu i przypadkowych szczegółów.. Po 3: Walidacja pokazuje, czy wzrost złożoności pomaga.. Po 4: Prostota, regularizacja i dobór danych równoważą ryzyka..
AKCENT DLA GRUPY: Zapytaj uczestników o zastosowanie, w którym to rozróżnienie ma znaczenie.
Wskazówka dla trenera: Nie czytaj punktów. Zacznij od problemu, a potem skonfrontuj przykład z mechanizmem algorytmu.

## Slajd 29. Data leakage: błąd, który wygląda jak sukces

**Co mówić:**

Zastosuj przykład klasyfikacji opóźnionych płatności, gdzie cecha „data windykacji” zawiera informację z przyszłości. Innym przypadkiem jest ten sam pacjent lub urządzenie po obu stronach podziału. Podkreśl, że algorytm może być matematycznie poprawny, a cały eksperyment bezwartościowy. To jeden z najczęstszych powodów pozornie idealnych wyników.
PUNKTY DO ROZWINIĘCIA: Po 1: Cechy zawierają informację powstałą po przewidywanym zdarzeniu.. Po 2: Dane z jednego użytkownika trafiają równocześnie do treningu i testu.. Po 3: Normalizacja lub selekcja cech korzysta z całego zbioru przed podziałem.. Po 4: Wynik testowy przestaje odzwierciedlać prawdziwy scenariusz..
AKCENT DLA GRUPY: Zapytaj uczestników o zastosowanie, w którym to rozróżnienie ma znaczenie.
Wskazówka dla trenera: Nie czytaj punktów. Zacznij od problemu, a potem skonfrontuj przykład z mechanizmem algorytmu.

## Slajd 30. Algorytmy Machine Learning

**Co mówić:**

Otwarcie modułu 3: Algorytmy Machine Learning. Porównujemy mechanizmy, a nie nazwy. Co optymalizują i w jakich warunkach zawodzą? Przeprowadź uczestników od intuicyjnego obrazu problemu do technicznego modelu. Zaznacz, że moduł ma wyraźny cel i będzie łączył historię, matematykę, metodę eksperymentalną oraz konsekwencje wdrożeniowe.

## Slajd 31. Mapa klasycznego Machine Learning

**Co mówić:**

Pokaż różnicę między zadaniem, algorytmem i metryką. SVM to rodzina metod, którą można stosować między innymi do klasyfikacji lub regresji. Drzewa realizują oba typy zadania. K-means grupuje punkty, ale nie „wie”, co te grupy znaczą. Zaczynając od rodzaju wyniku i struktury danych, unikamy technologicznych mód.
PUNKTY DO ROZWINIĘCIA: Po 1: Regresja: przewidujemy wartość ciągłą.. Po 2: Klasyfikacja: wybieramy klasę lub prawdopodobieństwo.. Po 3: Klasteryzacja: odkrywamy grupy podobnych przykładów.. Po 4: Redukcja wymiarowości: zachowujemy istotną strukturę.. Po 5: Detekcja anomalii: identyfikujemy nietypowe przypadki..
AKCENT DLA GRUPY: Zapytaj uczestników o zastosowanie, w którym to rozróżnienie ma znaczenie.
Wskazówka dla trenera: Nie czytaj punktów. Zacznij od problemu, a potem skonfrontuj przykład z mechanizmem algorytmu.

## Slajd 32. Regresja liniowa: najprostszy model zaskakująco daleko sięga

**Co mówić:**

Wyjaśnij, że „liniowość” oznacza liniowość względem współczynników. Model może korzystać także z transformowanych cech, o ile pozostaje liniowy w parametrach. Podaj przykład ceny energii zależnej od kilku zmiennych. Nie interpretuj współczynników przy danych obserwacyjnych automatycznie jako skutków przyczynowych.
PUNKTY DO ROZWINIĘCIA: Po 1: Model: ŷ = β₀ + β₁x₁ + … + βₚxₚ.. Po 2: Parametry minimalizują błąd, zwykle sumę kwadratów odchyleń.. Po 3: Współczynniki pozwalają badać kierunki zależności.. Po 4: Ryzyka: odstające obserwacje, współliniowość i błędne założenia..
AKCENT DLA GRUPY: INTERPRETOWALNOŚĆ NIE JEST TOŻSAMA Z PRZYCZYNOWOŚCIĄ.
Wskazówka dla trenera: Nie czytaj punktów. Zacznij od problemu, a potem skonfrontuj przykład z mechanizmem algorytmu.

## Slajd 33. Regresja logistyczna: prawdopodobieństwo zamiast etykiety

**Co mówić:**

Podkreśl przewrotność nazwy: mimo nazwy regresja logistyczna zwykle służy klasyfikacji. Zmiana progu decyzyjnego zmienia kompromis między precision i recall. Przy ważnych decyzjach należy badać kalibrację prawdopodobieństw, a nie tylko samą trafność klas. Przedstaw przykład przewidywania rezygnacji klienta.
PUNKTY DO ROZWINIĘCIA: Po 1: Obliczamy z = w·x + b.. Po 2: Sigmoid przekształca z na zakres od 0 do 1.. Po 3: Próg decyzyjny zamienia prawdopodobieństwo w klasę.. Po 4: Regularizacja pomaga ograniczać nadmierne dopasowanie..
AKCENT DLA GRUPY: Zapytaj uczestników o zastosowanie, w którym to rozróżnienie ma znaczenie.
Wskazówka dla trenera: Nie czytaj punktów. Zacznij od problemu, a potem skonfrontuj przykład z mechanizmem algorytmu.

## Slajd 34. k-nearest neighbors: decyzja na podstawie otoczenia

**Co mówić:**

Wybór k zmienia elastyczność decyzji. Małe k powoduje dużą wrażliwość na pojedyncze punkty, duże może wygładzać strukturę. Ważny jest koszt predykcji na dużym zbiorze i pamięć potrzebna do przechowania próbek. Porównaj intuicyjnie kNN z regresją logistyczną: lokalna decyzja kontra globalna funkcja.
PUNKTY DO ROZWINIĘCIA: Po 1: Dla nowego punktu znajdujemy k najbliższych obserwacji.. Po 2: W klasyfikacji głosujemy; w regresji uśredniamy.. Po 3: Metryka odległości i skala cech są krytyczne.. Po 4: W wielu wymiarach „bliskość” traci intuicyjne znaczenie..
AKCENT DLA GRUPY: Zapytaj uczestników o zastosowanie, w którym to rozróżnienie ma znaczenie.
Wskazówka dla trenera: Nie czytaj punktów. Zacznij od problemu, a potem skonfrontuj przykład z mechanizmem algorytmu.

## Slajd 35. Drzewo decyzyjne: przestrzeń cięta pytaniami

**Co mówić:**

Zapisz jeden przykład w języku biznesowym: czy klient miał opóźnienia, a jeśli tak, czy jego obciążenie przekracza próg? Algorytm wybiera pytania na podstawie redukcji nieczystości. Drzewo jest relatywnie łatwe do wyjaśnienia, ale niewielka zmiana próbek może zmienić całą strukturę. To motywacja do budowy lasów losowych.
PUNKTY DO ROZWINIĘCIA: Po 1: Węzeł wybiera cechę i próg rozdzielający próbki.. Po 2: Dla klasyfikacji stosujemy np. Gini lub entropię.. Po 3: Dla regresji typowo minimalizujemy wariancję w liściach.. Po 4: Głębokie drzewa często przeuczają się na niestabilnych podziałach..
AKCENT DLA GRUPY: Zapytaj uczestników o zastosowanie, w którym to rozróżnienie ma znaczenie.
Wskazówka dla trenera: Nie czytaj punktów. Zacznij od problemu, a potem skonfrontuj przykład z mechanizmem algorytmu.

## Slajd 36. Random Forest: wiele drzew, stabilniejszy wynik

**Co mówić:**

Pokaż intuicję różnicy między jednym ekspertem a grupą wielu ekspertów o odmiennych doświadczeniach. W lesie nie chodzi o identyczne drzewa, lecz ich zróżnicowanie. Wyjaśnij bagging i losowanie cech jako dwa źródła różnorodności. Forest nie musi dominować w każdej sytuacji, zwłaszcza gdy kluczowa jest latencja lub interpretacja prostej reguły.
PUNKTY DO ROZWINIĘCIA: Po 1: Każde drzewo widzi losowaną próbkę obserwacji.. Po 2: Przy podziałach losujemy podzbiór dostępnych cech.. Po 3: Wynik powstaje przez głosowanie lub uśrednianie.. Po 4: Kosztem większej złożoności poprawiamy odporność predykcji..
AKCENT DLA GRUPY: Zapytaj uczestników o zastosowanie, w którym to rozróżnienie ma znaczenie.
Wskazówka dla trenera: Nie czytaj punktów. Zacznij od problemu, a potem skonfrontuj przykład z mechanizmem algorytmu.

## Slajd 37. Gradient Boosting: modele korygują wcześniejsze błędy

**Co mówić:**

Porównaj do Random Forest: las buduje wiele drzew niezależnie, boosting rozwija zespół etapami. Nazwa „gradient” bierze się z używania informacji o kierunku poprawy celu optymalizacji. W tablicowych danych biznesowych boosting bywa bardzo silny, ale wymaga rzetelnej walidacji hiperparametrów. Podaj przykład prognozowania prawdopodobieństwa szkody.
PUNKTY DO ROZWINIĘCIA: Po 1: Nowy składnik poprawia błąd aktualnego zespołu.. Po 2: Gradient wskazuje kierunek zmniejszania funkcji straty.. Po 3: Płytkie drzewa są częstymi modelami bazowymi.. Po 4: Learning rate, liczba drzew i głębokość regulują złożoność..
AKCENT DLA GRUPY: Zapytaj uczestników o zastosowanie, w którym to rozróżnienie ma znaczenie.
Wskazówka dla trenera: Nie czytaj punktów. Zacznij od problemu, a potem skonfrontuj przykład z mechanizmem algorytmu.

## Slajd 38. SVM: granica z największym marginesem

**Co mówić:**

Zwróć uwagę na wektory nośne: to punkty bliskie granicy, które decydują o separatorze. SVM dobrze pokazuje geometryczne myślenie o klasyfikacji. Kernel jest sposobem liczenia podobieństwa odpowiadającego przestrzeni o innym wymiarze, bez jej jawnego konstruowania. Parametr C wiąże się z tolerancją naruszeń marginesu.
PUNKTY DO ROZWINIĘCIA: Po 1: Dla liniowo separowalnych danych maksymalizujemy margines.. Po 2: Soft margin dopuszcza błędy, regulowane parametrem C.. Po 3: Kernel trick pozwala ująć nieliniowe granice.. Po 4: Wrażliwość na skalę i koszt obliczeń mogą ograniczać wdrożenie..
AKCENT DLA GRUPY: Zapytaj uczestników o zastosowanie, w którym to rozróżnienie ma znaczenie.
Wskazówka dla trenera: Nie czytaj punktów. Zacznij od problemu, a potem skonfrontuj przykład z mechanizmem algorytmu.

## Slajd 39. k-means: grupowanie przez centroidy

**Co mówić:**

Przedstaw k-means jako naprzemienną optymalizację dwóch rzeczy: przypisań i środków. Inicjalizacja wpływa na wynik, dlatego stosuje się dobre strategie inicjalizacji oraz kilka uruchomień. Istotna jest skala cech, metryka i wybór k. Klastry nie są automatycznie prawdziwymi segmentami rynku.
PUNKTY DO ROZWINIĘCIA: Po 1: Wybieramy liczbę klastrów k i inicjujemy centroidy.. Po 2: Powtarzamy przypisanie punktów oraz obliczenie środków.. Po 3: Minimalizujemy sumę kwadratowych odległości do centroidów.. Po 4: Algorytm preferuje klastry zbliżone do sferycznych..
AKCENT DLA GRUPY: Zapytaj uczestników o zastosowanie, w którym to rozróżnienie ma znaczenie.
Wskazówka dla trenera: Nie czytaj punktów. Zacznij od problemu, a potem skonfrontuj przykład z mechanizmem algorytmu.

## Slajd 40. DBSCAN: klastry jako obszary zagęszczenia

**Co mówić:**

Porównaj z k-means: DBSCAN potrafi wychwycić nieregularne kształty klastrów i oznaczyć szum, lecz jest wrażliwy na definicję odległości oraz zmieniającą się gęstość. Nie utożsamiaj każdego punktu szumu z oszustwem. Punkt odstający statystycznie nie zawsze jest błędem ani zagrożeniem biznesowym.
PUNKTY DO ROZWINIĘCIA: Po 1: Punkty rdzeniowe mają odpowiednio liczne sąsiedztwo.. Po 2: Klaster rośnie przez połączenie obszarów gęstych.. Po 3: Punkty nienależące do klastrów mogą być szumem.. Po 4: Trudność: zmienna gęstość oraz dobór eps i min_samples..
AKCENT DLA GRUPY: Zapytaj uczestników o zastosowanie, w którym to rozróżnienie ma znaczenie.
Wskazówka dla trenera: Nie czytaj punktów. Zacznij od problemu, a potem skonfrontuj przykład z mechanizmem algorytmu.

## Slajd 41. PCA: mniej wymiarów, zachowana wariancja

**Co mówić:**

Podkreśl, że PCA jest metodą nienadzorowaną: nie wykorzystuje etykiet y. Może pomóc w wizualizacji i kompresji danych, ale nie gwarantuje lepszej klasyfikacji. Gdy zmienna o małej wariancji jest kluczowa, odrzucenie jej może zepsuć jakość modelu. Przed PCA szczególnie istotne bywa skalowanie cech.
PUNKTY DO ROZWINIĘCIA: Po 1: PCA tworzy ortogonalne kierunki zmienności.. Po 2: Pierwsza składowa zachowuje najwięcej wariancji.. Po 3: Transformacja może ograniczyć szum i korelacje.. Po 4: Duża wariancja nie zawsze oznacza użyteczność predykcyjną..
AKCENT DLA GRUPY: Zapytaj uczestników o zastosowanie, w którym to rozróżnienie ma znaczenie.
Wskazówka dla trenera: Nie czytaj punktów. Zacznij od problemu, a potem skonfrontuj przykład z mechanizmem algorytmu.

## Slajd 42. Detekcja anomalii: szukamy tego, co nietypowe

**Co mówić:**

Podaj przykład zmiany temperatury maszyny po serwisie. Nietypowy sygnał niekoniecznie oznacza awarię; może wynikać z nowego trybu pracy. W danych z silną nierównowagą klas kluczowa jest użyteczność alertów dla operatora. Zbyt czuły model może być kosztowny, nawet jeśli teoretycznie wykrywa więcej nietypowych obserwacji.
PUNKTY DO ROZWINIĘCIA: Po 1: Przykłady: anomalie transakcyjne, awarie, odchylenia procesów.. Po 2: Algorytmy uczą normalności lub izolują rzadkie punkty.. Po 3: Rzadkość nie musi oznaczać błędu ani oszustwa.. Po 4: Ważne są koszty fałszywych alarmów i zmiany rozkładu danych..
AKCENT DLA GRUPY: Zapytaj uczestników o zastosowanie, w którym to rozróżnienie ma znaczenie.
Wskazówka dla trenera: Nie czytaj punktów. Zacznij od problemu, a potem skonfrontuj przykład z mechanizmem algorytmu.

## Slajd 43. Dlaczego accuracy potrafi wprowadzać w błąd?

**Co mówić:**

Przy 1% oszustw klasyfikator zawsze mówiący „brak oszustwa” osiąga 99% accuracy i jest bezużyteczny do wykrywania oszustw. Omów macierz pomyłek i koszt fałszywych alarmów. Precision ma znaczenie, gdy każde zgłoszenie kosztuje czas analityka; recall, gdy pominięcie zjawiska jest drogie. Warto obserwować również kalibrację prawdopodobieństw.
PUNKTY DO ROZWINIĘCIA: Po 1: Precision: jaka część wskazań pozytywnych jest trafna?. Po 2: Recall: jaką część prawdziwych przypadków wykryliśmy?. Po 3: F1: kompromis precision i recall, z ograniczeniami.. Po 4: PR-AUC, ROC-AUC i kalibracja odpowiadają na inne pytania..
AKCENT DLA GRUPY: Zapytaj uczestników o zastosowanie, w którym to rozróżnienie ma znaczenie.
Wskazówka dla trenera: Nie czytaj punktów. Zacznij od problemu, a potem skonfrontuj przykład z mechanizmem algorytmu.

## Slajd 44. Który algorytm wybrać? Nie ma zwycięzcy uniwersalnego

**Co mówić:**

Przypomnij, że jakość zależy od problemu i danych, a nie popularności algorytmu. Wybór modelu uwzględnia koszt inferencji, tempo aktualizacji, wyjaśnialność, odporność i ryzyko. Skomplikowany model jest uzasadniony wtedy, gdy poprawa ma znaczenie operacyjne. Dobrym standardem jest model bazowy i jasne kryteria akceptacji.
PUNKTY DO ROZWINIĘCIA: Po 1: Interpretowalność i nadzór: regresja, płytkie drzewa.. Po 2: Silna jakość na danych tabelarycznych: zespoły drzew.. Po 3: Granica w przestrzeni cech: SVM lub modele liniowe.. Po 4: Odkrywanie struktury: k-means, DBSCAN, PCA.. Po 5: Wysokowymiarowe obrazy, tekst i sygnały: często sieci głębokie..
AKCENT DLA GRUPY: ZAWSZE PORÓWNUJ Z PROSTYM MODELEM REFERENCYJNYM.
Wskazówka dla trenera: Nie czytaj punktów. Zacznij od problemu, a potem skonfrontuj przykład z mechanizmem algorytmu.

## Slajd 45. Studium przypadku: przewidujemy rezygnację klienta

**Co mówić:**

W tym zadaniu pokazujemy kompletną logikę projektu. Nie zaczynamy od modelu, lecz od działania, które firma podejmie po otrzymaniu wyniku. Trzeba wyznaczyć moment dostępności danych, osobno sprawdzić ryzyko leakage i określić koszt każdej decyzji. Może się okazać, że logistyczna jest wystarczająco dobra. To lepsza decyzja niż ślepe maksymalizowanie accuracy.
PUNKTY DO ROZWINIĘCIA: Po 1: Zdefiniuj zdarzenie, horyzont predykcji i możliwą akcję.. Po 2: Wybierz prostą regresję logistyczną jako punkt odniesienia.. Po 3: Porównaj las i boosting na walidacji czasowej.. Po 4: Dobierz próg według kosztu kontaktu i utraconej sprzedaży.. Po 5: Zaplanuj monitoring dryfu po wdrożeniu..
AKCENT DLA GRUPY: Zapytaj uczestników o zastosowanie, w którym to rozróżnienie ma znaczenie.
Wskazówka dla trenera: Nie czytaj punktów. Zacznij od problemu, a potem skonfrontuj przykład z mechanizmem algorytmu.

## Slajd 46. Od pojedynczego neuronu i geometrii wag po backpropagation, CNN i mechanizm uwagi.

**Co mówić:**

Otwarcie modułu 4: Sieci neuronowe. Od pojedynczego neuronu i geometrii wag po backpropagation, CNN i mechanizm uwagi. Przeprowadź uczestników od intuicyjnego obrazu problemu do technicznego modelu. Zaznacz, że moduł ma wyraźny cel i będzie łączył historię, matematykę, metodę eksperymentalną oraz konsekwencje wdrożeniowe.

## Slajd 47. Sieć neuronowa nie jest kopią mózgu

**Co mówić:**

Wyjaśnij, że pojedynczy sztuczny neuron wykonuje prostą operację matematyczną; nie jest mikrorepliką komórki nerwowej. Główną siłą sieci jest kompozycja takich operacji i możliwość dopasowania parametrów przez optymalizację. Relacja z neuronauką istnieje, ale współczesne architektury są projektowane głównie ze względów obliczeniowych i statystycznych.
PUNKTY DO ROZWINIĘCIA: Po 1: Jednostka wykonuje sumę ważoną i nieliniową aktywację.. Po 2: Warstwy składają proste operacje w złożoną funkcję.. Po 3: Wiedza modelu jest rozproszona między parametrami.. Po 4: Analogia biologiczna jest historyczna, lecz ograniczona..
AKCENT DLA GRUPY: Zapytaj uczestników o zastosowanie, w którym to rozróżnienie ma znaczenie.
Wskazówka dla trenera: Nie czytaj punktów. Zacznij od problemu, a potem skonfrontuj przykład z mechanizmem algorytmu.

## Slajd 48. Anatomia sztucznego neuronu: wejście, waga, bias, aktywacja

**Co mówić:**

Wypowiedz formułę powoli. Wagi określają kierunek i siłę wpływu wejścia, bias przesuwa próg aktywacji, a nieliniowa funkcja pozwala budować złożone granice. Bez nieliniowości złożenie wielu warstw liniowych nadal pozostaje transformacją liniową. Poproś grupę o zastanowienie się, co stanie się po ustawieniu wszystkich wag na zero.
PUNKTY DO ROZWINIĘCIA: Po 1: Każde wejście xᵢ otrzymuje wagę wᵢ.. Po 2: Obliczamy potencjał z = Σ wᵢxᵢ + b.. Po 3: Funkcja φ(z) daje aktywację następnej warstwy.. Po 4: Wagi i bias są parametrami dostosowywanymi podczas treningu..
AKCENT DLA GRUPY: Zapytaj uczestników o zastosowanie, w którym to rozróżnienie ma znaczenie.
Wskazówka dla trenera: Nie czytaj punktów. Zacznij od problemu, a potem skonfrontuj przykład z mechanizmem algorytmu.

## Slajd 49. Perceptron: granica decyzyjna ma geometrię

**Co mówić:**

Narysuj dwuwymiarowy układ z dwiema klasami. Prosta w₁x₁ + w₂x₂ + b = 0 jest granicą decyzyjną. Ta geometria pomaga zrozumieć SVM i regresję logistyczną. Dopiero złożenie warstw i nieliniowości pozwala modelowi konstruować wiele połączonych obszarów decyzji.
PUNKTY DO ROZWINIĘCIA: Po 1: Wektor wag określa normalną do hiperpłaszczyzny.. Po 2: Bias przesuwa granicę bez zmiany jej orientacji.. Po 3: Przy dobrze reprezentowanych danych prosta granica może wystarczyć.. Po 4: XOR wymaga nieliniowości lub transformacji reprezentacji..
AKCENT DLA GRUPY: Zapytaj uczestników o zastosowanie, w którym to rozróżnienie ma znaczenie.
Wskazówka dla trenera: Nie czytaj punktów. Zacznij od problemu, a potem skonfrontuj przykład z mechanizmem algorytmu.

## Slajd 50. MLP: jak powstaje sieć wielowarstwowa?

**Co mówić:**

Nie mów, że każda warstwa automatycznie odkrywa coraz bardziej semantyczną wiedzę. Można taką hierarchię często obserwować, szczególnie w sieciach przetwarzających obraz, ale zależy to od architektury i zadania. W pełni połączonej sieci każdy neuron warstwy zwykle otrzymuje sygnał od wszystkich jednostek poprzedniej warstwy.
PUNKTY DO ROZWINIĘCIA: Po 1: Wejście: numeryczna reprezentacja obiektu.. Po 2: Warstwy ukryte: uczenie kompozycji cech.. Po 3: Wyjście: wynik dostosowany do zadania.. Po 4: Liczba warstw i neuronów zwiększa pojemność modelu..
AKCENT DLA GRUPY: Zapytaj uczestników o zastosowanie, w którym to rozróżnienie ma znaczenie.
Wskazówka dla trenera: Nie czytaj punktów. Zacznij od problemu, a potem skonfrontuj przykład z mechanizmem algorytmu.

## Slajd 51. ReLU, sigmoid i tanh: po co sieci funkcja aktywacji?

**Co mówić:**

Narysuj intuicję pochodnych. Funkcje o silnym nasyceniu dają małe gradienty w szerokich obszarach; ReLU zwykle zachowuje prostszą propagację sygnału dla dodatnich aktywacji. ReLU ma także problem martwych jednostek. Pokaż, że aktywacja warstwy ukrytej i aktywacja wyjścia pełnią inne role.
PUNKTY DO ROZWINIĘCIA: Po 1: ReLU(x) = max(0, x): prosta i często skuteczna.. Po 2: Sigmoid mapuje liczbę na (0,1), przydatna m.in. na wyjściu binarnym.. Po 3: tanh mapuje na (−1,1), ale może się nasycać.. Po 4: Wybór aktywacji wpływa na gradient i stabilność treningu..
AKCENT DLA GRUPY: Zapytaj uczestników o zastosowanie, w którym to rozróżnienie ma znaczenie.
Wskazówka dla trenera: Nie czytaj punktów. Zacznij od problemu, a potem skonfrontuj przykład z mechanizmem algorytmu.

## Slajd 52. Forward pass: od sygnału do predykcji

**Co mówić:**

Pokazuj kolejne warstwy jedną po drugiej. Każdy neuron składa liniową transformację i nieliniową aktywację. Macierz W opisuje wszystkie połączenia między dwoma warstwami. Zawartość aktywacji nie jest deklarowaną regułą zapisanych w słowach, lecz wektorem liczb, których znaczenie wynika z całego wyuczonego modelu.
PUNKTY DO ROZWINIĘCIA: Po 1: Warstwa 1: a¹ = φ(W¹x + b¹).. Po 2: Warstwa 2: a² = φ(W²a¹ + b²).. Po 3: Warstwa wyjściowa: ŷ = g(W³a² + b³).. Po 4: Na końcu mamy wynik, ale jeszcze nie wiemy, jak bardzo dobry..
AKCENT DLA GRUPY: Zapytaj uczestników o zastosowanie, w którym to rozróżnienie ma znaczenie.
Wskazówka dla trenera: Nie czytaj punktów. Zacznij od problemu, a potem skonfrontuj przykład z mechanizmem algorytmu.

## Slajd 53. Animacja: sygnał płynie do przodu, błąd wraca

**Co mówić:**

Włącz pokaz slajdów, aby uruchomić zapętloną animację GIF. Najpierw pokaż intuicyjny ruch sygnału przez warstwy. Następnie odwróć interpretację: informacja o tym, jak zmiana wagi wpływa na błąd, jest obliczana od wyjścia ku wejściu. Sygnał błędu nie płynie biologicznym aksonem, lecz jest obliczeniem reguły łańcuchowej. To precyzyjna, ale uproszczona metafora.
PUNKTY DO ROZWINIĘCIA: Po 1: Faza niebieska: propagacja aktywacji od wejścia do wyjścia.. Po 2: Porównanie predykcji z celem daje sygnał błędu.. Po 3: Faza złota: propagacja gradientu w kierunku wejścia.. Po 4: Rzeczywisty backprop używa pochodnych, nie fizycznego „cofania informacji”..
AKCENT DLA GRUPY: ANIMACJA JEST SCHEMATEM IDEOWYM, NIE ZAPISEM PRAWDZIWEGO TRENINGU.
Wskazówka dla trenera: Nie czytaj punktów. Zacznij od problemu, a potem skonfrontuj przykład z mechanizmem algorytmu.

## Slajd 54. Funkcja straty mówi, co poprawić

**Co mówić:**

Rozróżnij cel matematyczny od sensu biznesowego. Cross-entropy mocno karze bardzo pewne, błędne predykcje. MSE silnie reaguje na duże błędy. W obydwu przypadkach minimalizacja na treningu nie gwarantuje odporności na inne rozkłady, dlatego potrzebujemy zbioru walidacyjnego i monitoringu po wdrożeniu.
PUNKTY DO ROZWINIĘCIA: Po 1: Dla regresji możemy stosować MSE.. Po 2: Dla klas: cross-entropy łączy wyjście probabilistyczne z etykietą.. Po 3: Strata jest funkcją wielu wag i biasów.. Po 4: Dobra funkcja straty nie zastępuje oceny na nowych danych..
AKCENT DLA GRUPY: Zapytaj uczestników o zastosowanie, w którym to rozróżnienie ma znaczenie.
Wskazówka dla trenera: Nie czytaj punktów. Zacznij od problemu, a potem skonfrontuj przykład z mechanizmem algorytmu.

## Slajd 55. Gradient: w którą stronę zmienić każdą wagę?

**Co mówić:**

Pokaż prosty obraz krajobrazu straty. Każda waga ma swój kierunek lokalnego wzrostu błędu, więc poruszamy się przeciwnie do gradientu. Nie oznacza to pewności znalezienia optimum globalnego, szczególnie w złożonej sieci. Learning rate zbyt duży może powodować oscylacje, zbyt mały spowalniać uczenie.
PUNKTY DO ROZWINIĘCIA: Po 1: ∂L/∂w mówi, jak mała zmiana w wpływa na stratę.. Po 2: Gradient jest wektorem pochodnych dla wszystkich parametrów.. Po 3: Gradient descent: θ ← θ − η∇L(θ).. Po 4: Learning rate η kontroluje długość kroku aktualizacji..
AKCENT DLA GRUPY: Zapytaj uczestników o zastosowanie, w którym to rozróżnienie ma znaczenie.
Wskazówka dla trenera: Nie czytaj punktów. Zacznij od problemu, a potem skonfrontuj przykład z mechanizmem algorytmu.

## Slajd 56. Backpropagation: reguła łańcuchowa w skali sieci

**Co mówić:**

To najważniejszy slajd matematyczny. Podaj zależność ∂L/∂w = (∂L/∂a)(∂a/∂z)(∂z/∂w). Każdy fragment jest lokalny, co pozwala obliczać gradienty efektywnie i ponownie używać wyników. Backpropagation jest mechanizmem liczenia pochodnych, natomiast SGD, Adam lub inny optymalizator wybiera sposób zmiany parametrów. Te pojęcia często błędnie się utożsamia.
PUNKTY DO ROZWINIĘCIA: Po 1: Obliczamy aktywacje i zapamiętujemy wartości pośrednie.. Po 2: Wyznaczamy pochodną straty względem wyjścia.. Po 3: Przez kolejne warstwy liczymy pochodne z reguły łańcuchowej.. Po 4: Optymalizator aktualizuje parametry na podstawie gradientów..
AKCENT DLA GRUPY: BACKPROPAGATION ≠ GRADIENT DESCENT: PIERWSZE LICZY, DRUGIE AKTUALIZUJE.
Wskazówka dla trenera: Nie czytaj punktów. Zacznij od problemu, a potem skonfrontuj przykład z mechanizmem algorytmu.

## Slajd 57. Jedna iteracja uczenia w ruchu

**Co mówić:**

Zatrzymaj uwagę uczestników na tym, że to ta sama sieć przed i po korekcie, lecz z nieco innymi wagami. W praktyce uczenie odbywa się na batchach, a niekoniecznie pojedynczych obserwacjach. Schemat pokazuje oba kierunki obliczeń, lecz nie przedstawia rozmiarów rzeczywistych pochodnych. To okazja do zadania pytania, dlaczego zbyt mała lub zbyt duża aktualizacja może szkodzić.
PUNKTY DO ROZWINIĘCIA: Po 1: Przód: aktywacje budują predykcję z bieżących wag.. Po 2: Porównanie: obliczamy loss względem odpowiedzi docelowej.. Po 3: Tył: pochodne rozchodzą się przez architekturę.. Po 4: Aktualizacja: parametry zmieniają się przed następną iteracją..
AKCENT DLA GRUPY: W POWTARZANYCH ITERACJACH ZMIENIA SIĘ MODEL, NIE SAMA DEFINICJA ZADANIA.
Wskazówka dla trenera: Nie czytaj punktów. Zacznij od problemu, a potem skonfrontuj przykład z mechanizmem algorytmu.

## Slajd 58. Przykład: jeden neuron i jeden krok gradientowy

**Co mówić:**

To prosty rachunek, którego uczestnicy mogą dokonać na kartce. Wyjaśnij, że model ma wagę 0,5, więc dla wejścia 2 przewiduje 1, podczas gdy cel wynosi 2. Z gradientu -2 i learning rate 0,1 otrzymujemy wzrost wagi do 0,7. Przy niezmienionym biasie nowa predykcja to 1,4, bliższa celowi. Przykład jest celowo liniowy; daje fundament przed sieciami wielowarstwowymi.
PUNKTY DO ROZWINIĘCIA: Po 1: Predykcja liniowa: ŷ = wx + b = 1.. Po 2: Strata: L = ½(ŷ − y)² = 0,5.. Po 3: Pochodna: ∂L/∂w = (ŷ − y)·x = −2.. Po 4: Dla η = 0,1: nowa waga w = 0,7 (gdy b nie aktualizujemy)..
AKCENT DLA GRUPY: PO JEDNYM KROKU PREDYKCJA ROŚNIE Z 1 DO 1,4.
Wskazówka dla trenera: Nie czytaj punktów. Zacznij od problemu, a potem skonfrontuj przykład z mechanizmem algorytmu.

## Slajd 59. Epoch, batch, learning rate: rytm uczenia

**Co mówić:**

Warto pokazać różnicę między batch gradient descent, SGD i mini-batch. Mniejsze porcje wprowadzają szum do estymacji gradientu, który bywa praktycznie użyteczny, ale nie jest zawsze korzystny. Ilość danych, budżet obliczeniowy i pamięć ograniczają ustawienia. Monitoruj nie tylko loss treningowy, lecz także walidacyjny.
PUNKTY DO ROZWINIĘCIA: Po 1: Epoch: jedno przejście przez cały zbiór treningowy.. Po 2: Batch: porcja przykładów użyta do obliczenia gradientu.. Po 3: Learning rate: wielkość aktualizacji parametrów.. Po 4: Optymalizator i harmonogram wpływają na stabilność..
AKCENT DLA GRUPY: Zapytaj uczestników o zastosowanie, w którym to rozróżnienie ma znaczenie.
Wskazówka dla trenera: Nie czytaj punktów. Zacznij od problemu, a potem skonfrontuj przykład z mechanizmem algorytmu.

## Slajd 60. Dlaczego głęboka sieć może się nie uczyć?

**Co mówić:**

Pokaż intuicję mnożenia wielu pochodnych w regule łańcuchowej. Gdy ich wartości są małe, sygnał może zanikać w głębokiej sieci; gdy duże, może eksplodować. ReLU, normalizacja i połączenia rezydualne są jednymi z narzędzi ograniczania tych problemów. Nie ma jednej techniki gwarantującej stabilność każdego modelu.
PUNKTY DO ROZWINIĘCIA: Po 1: Nasycające aktywacje osłabiają pochodne.. Po 2: Zła inicjalizacja powoduje niekorzystną skalę sygnału.. Po 3: Normalizacja i połączenia rezydualne ułatwiają trening.. Po 4: Zbyt duży learning rate destabilizuje aktualizacje..
AKCENT DLA GRUPY: Zapytaj uczestników o zastosowanie, w którym to rozróżnienie ma znaczenie.
Wskazówka dla trenera: Nie czytaj punktów. Zacznij od problemu, a potem skonfrontuj przykład z mechanizmem algorytmu.

## Slajd 61. Dropout, early stopping i regularizacja wag

**Co mówić:**

Wytłumacz, że dropout jest procedurą treningową, a w typowym wnioskowaniu nie wyłącza się losowo neuronów w ten sam sposób. Early stopping korzysta z walidacji jako sygnału do zatrzymania treningu, ale nie zastępuje niezależnego testu. Regularizacja to kontrola złożoności i odporności; nie jeden uniwersalny parametr.
PUNKTY DO ROZWINIĘCIA: Po 1: Dropout losowo dezaktywuje część aktywacji podczas treningu.. Po 2: Weight decay ogranicza duże wartości parametrów.. Po 3: Early stopping przerywa trening po pogorszeniu walidacji.. Po 4: Więcej danych i augmentacja mogą być skuteczniejsze od większej sieci..
AKCENT DLA GRUPY: Zapytaj uczestników o zastosowanie, w którym to rozróżnienie ma znaczenie.
Wskazówka dla trenera: Nie czytaj punktów. Zacznij od problemu, a potem skonfrontuj przykład z mechanizmem algorytmu.

## Slajd 62. CNN: dlaczego konwolucja działa na obrazach?

**Co mówić:**

Wyobraź sobie filtr wykrywający pionowe krawędzie. Ten sam zestaw wag stosujemy w różnych miejscach obrazu. Dzięki temu model wykorzystuje względną niezmienniczość pozycji cech i lepiej radzi sobie z pikselami niż zwykłe pełne połączenie o podobnej liczbie parametrów. CNN uczy się filtrów w procesie treningu; nie trzeba ręcznie programować detektora nosa czy koła.
PUNKTY DO ROZWINIĘCIA: Po 1: Filtr przesuwa się po obrazie i reaguje na lokalny wzór.. Po 2: Współdzielone parametry zmniejszają liczbę wag.. Po 3: Kolejne warstwy łączą krawędzie, tekstury i fragmenty obiektów.. Po 4: Pooling lub stride redukują rozdzielczość cech..
AKCENT DLA GRUPY: Zapytaj uczestników o zastosowanie, w którym to rozróżnienie ma znaczenie.
Wskazówka dla trenera: Nie czytaj punktów. Zacznij od problemu, a potem skonfrontuj przykład z mechanizmem algorytmu.

## Slajd 63. Od pikseli do reprezentacji: hierarchia cech w CNN

**Co mówić:**

Zaznacz, że „warstwa rozpoznaje oko” jest intuicyjnym opisem, nie niezmiennym prawem o wszystkich sieciach. Rzeczywiste reprezentacje bywają rozproszone i zależne od danych. W analizie obrazu należy uważać na skróty: model potrafi opierać decyzję na tle zdjęcia, a nie istotnym obiekcie. To kolejny argument za walidacją na nowych warunkach.
PUNKTY DO ROZWINIĘCIA: Po 1: Warstwy początkowe reagują na lokalne zmiany jasności.. Po 2: Warstwy środkowe łączą tekstury i kształty.. Po 3: Późniejsze reprezentacje są dostosowane do celu zadania.. Po 4: Wyjaśnialność nadal wymaga testów i ostrożności..
AKCENT DLA GRUPY: Zapytaj uczestników o zastosowanie, w którym to rozróżnienie ma znaczenie.
Wskazówka dla trenera: Nie czytaj punktów. Zacznij od problemu, a potem skonfrontuj przykład z mechanizmem algorytmu.

## Slajd 64. Attention: modelowanie zależności między elementami

**Co mówić:**

Pokaż zdanie, w którym znaczenie jednego słowa zależy od słowa odległego o kilka pozycji. Samoattention wylicza zależności między tokenami. Odmiennie niż klasyczna CNN, Transformer bardzo bezpośrednio modeluje relacje między pozycjami, choć wymaga odpowiedniego kodowania pozycji. Wagi attention nie są prostym, pełnym wyjaśnieniem wszystkich decyzji modelu.
PUNKTY DO ROZWINIĘCIA: Po 1: Każdy token otrzymuje reprezentację wektorową.. Po 2: Query, key i value służą wyznaczaniu wag uwagi.. Po 3: Mechanizm miesza informacje według kontekstu.. Po 4: Uwaga nie jest tożsama z ludzką świadomością uwagi..
AKCENT DLA GRUPY: Zapytaj uczestników o zastosowanie, w którym to rozróżnienie ma znaczenie.
Wskazówka dla trenera: Nie czytaj punktów. Zacznij od problemu, a potem skonfrontuj przykład z mechanizmem algorytmu.

## Slajd 65. Embedding: znaczenie zamienione w geometrię

**Co mówić:**

Wyjaśnij embedding przez analogię do mapy: obiekty o podobnym kontekście mogą zajmować podobne obszary. Jednak nie ma jednej „prawdziwej osi znaczenia”, a geometria zależy od modelu. Embedding jest przydatny w wyszukiwaniu semantycznym, rekomendacjach i klasteryzacji. Kładziemy nacisk na wyuczoną reprezentację, nie konkretne biblioteki.
PUNKTY DO ROZWINIĘCIA: Po 1: Słowo, obraz lub obiekt staje się wektorem liczb.. Po 2: Bliskość w przestrzeni może odzwierciedlać podobieństwo.. Po 3: Reprezentacja zależy od celu i danych treningowych.. Po 4: Nie każda odległość geometryczna ma proste znaczenie semantyczne..
AKCENT DLA GRUPY: Zapytaj uczestników o zastosowanie, w którym to rozróżnienie ma znaczenie.
Wskazówka dla trenera: Nie czytaj punktów. Zacznij od problemu, a potem skonfrontuj przykład z mechanizmem algorytmu.

## Slajd 66. Czego sieci neuronowe nie gwarantują?

**Co mówić:**

Na zakończenie pogłębionej części technicznej wróć do historii AI: każda nowa architektura zwiększa możliwości, ale nie anuluje problemu generalizacji. Pokaż przykład klasyfikatora obrazów, który działa gorzej po zmianie oświetlenia, oraz modelu językowego tworzącego przekonującą, ale fałszywą odpowiedź. Ocena musi być powiązana z realnym procesem.
PUNKTY DO ROZWINIĘCIA: Po 1: Zmiana rozkładu danych może pogorszyć wyniki.. Po 2: Model może nauczyć się korelacji pozornych lub stronniczości danych.. Po 3: Generowane wyniki mogą być błędne mimo płynnej formy.. Po 4: Potrzebna jest kontrola, testy odporności i monitoring..
AKCENT DLA GRUPY: SIEĆ JEST MODELEM ZJAWISKA, NIE SAMYM ZJAWISKIEM.
Wskazówka dla trenera: Nie czytaj punktów. Zacznij od problemu, a potem skonfrontuj przykład z mechanizmem algorytmu.

## Slajd 67. Od formalnego neuronu do modeli fundamentalnych

**Co mówić:**

Zepnij całość w jeden łańcuch przyczynowy: pojedynczy neuron ma niewielką moc wyrazu, złożona sieć potrafi modelować skomplikowane funkcje, trening nadaje parametrom wartości, a wdrożenie dopiero zamienia model w część systemu. Kluczowym błędem jest utożsamienie możliwości modelu z niezawodnością systemu.
PUNKTY DO ROZWINIĘCIA: Po 1: Neuron: transformacja sygnału i nieliniowość.. Po 2: Sieć: składanie transformacji w reprezentację.. Po 3: Uczenie: gradient i korekta parametrów względem celu.. Po 4: System: model, dane, procedury kontroli, narzędzia, użytkownik..
AKCENT DLA GRUPY: Zapytaj uczestników o zastosowanie, w którym to rozróżnienie ma znaczenie.
Wskazówka dla trenera: Nie czytaj punktów. Zacznij od problemu, a potem skonfrontuj przykład z mechanizmem algorytmu.

## Slajd 68. Co warto zapamiętać po całym wykładzie?

**Co mówić:**

Podsumuj cztery bloki. Historia AI pokazuje różnorodność metod. Machine Learning definiujemy przez zdolność uczenia parametrów lub struktury na podstawie danych. W Deep Learning bardzo istotna jest kompozycja reprezentacji i efektywne liczenie gradientów. Na poziomie systemowym potrzebujemy dodatkowo procedur nadzoru, weryfikacji jakości i odpowiedzialności. Powtórz pięć pytań z początku wykładu.

## Slajd 69. Źródła i dalsza lektura

**Co mówić:**

Bibliografia celowo obejmuje pierwotne teksty historyczne oraz oficjalne opisy głównych przełomów. Podkreśl, że definicje AI ewoluują, a szczegóły techniczne algorytmów należy weryfikować w konkretnych pracach naukowych. Materiał ma charakter edukacyjny i nie jest instrukcją instalacji ani kursowym przeglądem bibliotek.

## Slajd 70. Czy model nauczył się świata?

**Co mówić:**

Pytanie otwarte do dyskusji. Nie sugeruj jednoznacznego rozstrzygnięcia filozoficznego. Wracamy do rozróżnienia kompetencji w zadaniu, struktury modelu i doświadczenia świata. Współczesne modele potrafią skutecznie aproksymować zależności, ale dopiero rzetelne testy pokazują granice ich generalizacji.
