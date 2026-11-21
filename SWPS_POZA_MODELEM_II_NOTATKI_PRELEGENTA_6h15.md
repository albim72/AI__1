# POZA MODELEM · CZĘŚĆ II — KOMPLETNE NOTATKI PRELEGENTA

SWPS, Wstęp do sztucznej inteligencji · 21.11.2026 · dr Marcin Albiniak
Dokładny czas dydaktyczny: **375 minut (6 h 15 min)**. Przerwy poza planem.


## MODUŁ 1: MODELE OD ŚRODKA (55 minut)

**Slajd otwierający (2 min)**: wprowadź pytanie przewodnie.


### SLAJD 2: Model to funkcja, nie magia (3 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: MODELE OD ŚRODKA | SLAJD: 2 | CZAS: 3 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Zacznij od oddzielenia modelu matematycznego od kompletnego produktu. Symbol f z parametrami theta oznacza regułę wyuczoną na danych. Ten sam model może działać poprawnie w jednym kontekście i zawodzić w innym. W praktyce rezultat zależy też od transformacji danych, progu decyzji i uprawnień.

ROZWINIĘCIE PLANSZY:
Punkt 1: x: dane i kontekst. Punkt 2: fθ: wyuczone parametry. Punkt 3: y: predykcja, ranking lub rozkład. Punkt 4: system: reguły poza modelem.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PYTANIE DO SALI: Która część systemu naprawdę podpisuje decyzję?
Omów co najmniej dwie możliwe odpowiedzi, wskazując ich warunki i konsekwencje.

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 3: Mapa rodzin modeli (3 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: MODELE OD ŚRODKA | SLAJD: 3 | CZAS: 3 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Wyjaśnij, że wybór modelu powinien wynikać z rodzaju problemu i kosztu pomyłki. Prognoza opóźnienia to inne zadanie niż wyszukiwanie podobnego dokumentu. Nawet w projekcie „AI-first” wiele podzadań lepiej realizuje SQL, reguła czy prosty model.

ROZWINIĘCIE PLANSZY:
Punkt 1: Regresja / drzewa: predykcja liczby. Punkt 2: Klasyfikatory: wykrywanie klas. Punkt 3: Embedding / ranking: wyszukiwanie. Punkt 4: Generatywne / multimodalne: tworzenie.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PYTANIE DO SALI: Czy do faktury potrzebny jest model generatywny?
Omów co najmniej dwie możliwe odpowiedzi, wskazując ich warunki i konsekwencje.

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 4: Regresja i klasyfikacja (3 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: MODELE OD ŚRODKA | SLAJD: 4 | CZAS: 3 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Pokaż różnicę między prognozą liczbową, prawdopodobieństwem a decyzją. Model kredytowy może zwrócić wynik ryzyka, ale polityka firmy określa próg. Kalibracja oznacza zgodność deklarowanego poziomu ufności z częstością zdarzeń w odpowiednich warunkach.

ROZWINIĘCIE PLANSZY:
Punkt 1: Regresja: ile?. Punkt 2: Klasyfikacja: czy / która klasa?. Punkt 3: Próg: kiedy zamienić wynik w działanie?. Punkt 4: Kalibracja: czy 0,8 znaczy 80%?.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 5: Drzewa, boosting, sieci (3 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: MODELE OD ŚRODKA | SLAJD: 5 | CZAS: 3 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Na tablicy narysuj proste drzewo decyzji z warunkami na danych. Następnie wskaż boosting jako kolejne modele poprawiające błędy poprzedników. Sieć neuronowa jest elastyczna, ale wyjaśnienie i koszt utrzymania są inne. Algorytm trzeba porównać na tej samej walidacji.

ROZWINIĘCIE PLANSZY:
Punkt 1: Drzewo: czytelne podziały. Punkt 2: Gradient boosting: zespoły drzew. Punkt 3: Sieć: warstwy i reprezentacje. Punkt 4: Cena: dane, tuning, utrzymanie.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 6: Dane trenujące to nie rzeczywistość (3 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: MODELE OD ŚRODKA | SLAJD: 6 | CZAS: 3 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Wyjaśnij wyciek danych na przykładzie prognozy rezygnacji klienta: etykieta „rezygnował” nie może być podpowiadana przez status utworzony po rezygnacji. W prawdziwym projekcie trzeba mieć rozdzielone okresy czasu i klientów. Wynik laboratoryjny nie gwarantuje poprawnej generalizacji.

ROZWINIĘCIE PLANSZY:
Punkt 1: Próba ≠ populacja. Punkt 2: Leakage: informacja z przyszłości. Punkt 3: Drift: rozkład zmienia się po wdrożeniu. Punkt 4: Test: podział czasowy i podgrupowy.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 7: Neuron, warstwa, optymalizacja (3 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: MODELE OD ŚRODKA | SLAJD: 7 | CZAS: 3 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Zamiast antropomorfizować neuron, pokaż proste przekształcenie matematyczne. Model reguluje wagi, minimalizując uzgodnioną stratę. Strata treningowa nie jest celem biznesowym; możemy ją obniżać, a pogarszać działanie w świecie. Wymień regularizację i wczesne zatrzymanie.

ROZWINIĘCIE PLANSZY:
Punkt 1: Suma ważona i nieliniowość. Punkt 2: Funkcja straty mierzy odchylenie. Punkt 3: Gradient kieruje aktualizacją. Punkt 4: Epoki i batch definiują proces.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 8: Transformer: mechanizm uwagi (3 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: MODELE OD ŚRODKA | SLAJD: 8 | CZAS: 3 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Zaproponuj eksperyment: słowo „bank” w zdaniu o rzece i finansach. Uwaga pomaga warstwom uwzględniać otoczenie, lecz nie jest intencją ani przeżywaniem. Kluczowy element: macierze zapytań, kluczy i wartości, normalizacja wag i przekształcenia.

ROZWINIĘCIE PLANSZY:
Punkt 1: Tokeny → wektory reprezentacji. Punkt 2: Attention: relacje między pozycjami. Punkt 3: Warstwy: przekształcenia kontekstu. Punkt 4: Predykcja następnego tokenu.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

ŹRÓDŁO / KONTEKST: https://arxiv.org/abs/1706.03762

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 9: Embedding: geometria znaczenia (3 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: MODELE OD ŚRODKA | SLAJD: 9 | CZAS: 3 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Przykład: „faktura została opłacona” i „faktura nie została opłacona” mają wiele wspólnych słów i mogą być blisko semantycznie. Wyszukiwarka musi więc rozróżniać podobieństwo tematu od poprawności logicznej. Stąd potrzeba metadanych, ontologii i reguł.

ROZWINIĘCIE PLANSZY:
Punkt 1: Dokument ↔ wektor. Punkt 2: Cosine similarity. Punkt 3: Top-k i reranking. Punkt 4: Granica: podobne zdania mogą być sprzeczne.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 10: Tokenizacja i okno kontekstu (3 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: MODELE OD ŚRODKA | SLAJD: 10 | CZAS: 3 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Wyjaśnij tokenizację na nazwisku, jednostce medycznej i identyfikatorze. Nawet duże okno nie gwarantuje, że model idealnie wykorzysta każdy fragment. Praktycznie ważniejsze bywają selekcja dowodów, cytowanie fragmentów i test długich kontekstów niż samo zwiększanie liczby tokenów.

ROZWINIĘCIE PLANSZY:
Punkt 1: Token nie musi być wyrazem. Punkt 2: Kontekst ma ograniczoną pojemność. Punkt 3: Koszt / latencja / dokładność. Punkt 4: Lost-in-the-middle i selekcja informacji.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 11: Od logitów do odpowiedzi (3 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: MODELE OD ŚRODKA | SLAJD: 11 | CZAS: 3 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Przejdź przez przykład, w którym następny token ma trzy możliwe wybory. Obniżenie temperatury koncentruje rozkład, lecz nie dodaje wiedzy. W systemie produkcyjnym parametry generowania pomagają powtarzalności, ale potrzebne są jeszcze format wyjścia, walidacja i narzędzia.

ROZWINIĘCIE PLANSZY:
Punkt 1: Logity i rozkład prawdopodobieństwa. Punkt 2: Softmax i parametry dekodowania. Punkt 3: Top-p / top-k / temperatura. Punkt 4: Stabilność ≠ poprawność merytoryczna.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 12: Pretraining → dostrojenie → preferencje (3 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: MODELE OD ŚRODKA | SLAJD: 12 | CZAS: 3 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Rozdziel cztery rzeczy: wiedzę, zdolność rozwiązywania zadań, styl i ograniczenia zachowania. Model dostrojony do rozmowy nie staje się źródłem prawdy o firmie. Informacje o firmie wymagają danych zewnętrznych, a procesy biznesowe wymagają kontroli wykonania.

ROZWINIĘCIE PLANSZY:
Punkt 1: Pretraining: wzorce na dużych zbiorach. Punkt 2: SFT: demonstracje zadań. Punkt 3: Uczenie preferencji: odpowiedzi akceptowane. Punkt 4: Nie myl polityki zachowania z wiedzą.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 13: RAG czy fine-tuning? (3 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: MODELE OD ŚRODKA | SLAJD: 13 | CZAS: 3 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Pytanie decyzyjne: czy brakuje modelowi danych o stanie świata, czy system źle wykonuje konkretną klasę zadań? RAG zwykle lepiej obsługuje dynamiczne dokumenty. Dostrajanie może pomagać dla powtarzalnego formatu i specyficznych zadań, ale nie zastąpi aktualizacji wiedzy.

ROZWINIĘCIE PLANSZY:
Punkt 1: RAG: aktualne, sprawdzalne źródła. Punkt 2: Fine-tuning: specjalizacja zachowania. Punkt 3: Prompt: struktura zadania. Punkt 4: Reguły: bezpieczne warunki działania.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 14: LoRA, adaptery i kwantyzacja (3 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: MODELE OD ŚRODKA | SLAJD: 14 | CZAS: 3 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Rozpocznij od kosztu pamięci wag w formatach o różnej liczbie bitów, bez obietnicy idealnej oszczędności, bo dochodzi cache i narzut systemu. LoRA dostraja niskowymiarowe przyrosty, a kwantyzacja zmienia reprezentację wag. Obydwa rozwiązania wymagają testów regresji.

ROZWINIĘCIE PLANSZY:
Punkt 1: Wagi pełne vs małe adaptacje. Punkt 2: Kwantyzacja zmniejsza precyzję zapisu. Punkt 3: VRAM / przepustowość / batch. Punkt 4: Jakość i latencję trzeba zmierzyć.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 15: Mixture of Experts (3 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: MODELE OD ŚRODKA | SLAJD: 15 | CZAS: 3 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
MoE rozdziela pojemność modelu od liczby operacji na pojedynczym tokenie, lecz infrastruktura może pozostać złożona. Wytłumacz routing i ryzyka: nierówne obciążenie ekspertów, komunikacja między urządzeniami i wpływ jakości routingu na wyniki.

ROZWINIĘCIE PLANSZY:
Punkt 1: Router wybiera ekspertów. Punkt 2: Nie wszystkie parametry pracują naraz. Punkt 3: Koszt pamięci nadal ma znaczenie. Punkt 4: Balansowanie obciążenia i routing.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 16: Multimodalność: wspólna przestrzeń (3 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: MODELE OD ŚRODKA | SLAJD: 16 | CZAS: 3 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Pokaż przykład odczytu skanu faktury: OCR może przekręcić kwotę, model może dobrze zinterpretować przekręcony tekst, a wykonanie API formalnie się powiedzie. Wniosek: ocena powinna obejmować cały łańcuch, a nie tylko jakość modelu językowego.

ROZWINIĘCIE PLANSZY:
Punkt 1: Encoder obrazu / dźwięku. Punkt 2: Fuzja reprezentacji. Punkt 3: Generacja odpowiedzi lub działania. Punkt 4: Błędy mogą przenosić się między modalnościami.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 17: Kompozycja modeli (3 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: MODELE OD ŚRODKA | SLAJD: 17 | CZAS: 3 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
To ważny antymit: jeden wielki model nie musi wykonywać wszystkiego. Architekturę można rozbić na komponenty o jawnych kompetencjach i własnych testach. W efekcie oszczędzamy koszt, skracamy opóźnienie i łatwiej lokalizujemy awarię.

ROZWINIĘCIE PLANSZY:
Punkt 1: Model A rozpoznaje typ sprawy. Punkt 2: Retriever wskazuje wiarygodne źródła. Punkt 3: LLM tworzy propozycję. Punkt 4: Silnik reguł i człowiek zatwierdzają.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 18: LAB: dobierz architekturę do problemu (5 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: MODELE OD ŚRODKA | SLAJD: 18 | CZAS: 5 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Rozdaj trzy scenariusze. Przez cztery minuty zespoły wybierają architekturę oraz opisują, czego modelowi nie wolno ustalać samodzielnie. Po jednej minucie prezentacji na grupę wskaż, że w należnościach stan rozliczenia powinien wynikać z systemu źródłowego, nie z deklaracji w mailu.

ROZWINIĘCIE PLANSZY:
Punkt 1: Zespół A: prognoza zapotrzebowania. Punkt 2: Zespół B: streszczenie umów. Punkt 3: Zespół C: status rozliczenia. Punkt 4: Każdy: dane, model, metryka, próg działania.

PROWADZENIE I PRZYKŁAD:
Praca z salą: najpierw przedstaw scenariusz i rozdziel role. Następnie daj grupom czas na zapisanie odpowiedzi na kartce, niech nie wybierają od razu narzędzia. Obejdź zespoły i pytaj o źródło danych, semantykę stanów, wyjątki oraz właściciela decyzji. Zaproś co najmniej dwa zespoły do przedstawienia odmiennego rozwiązania; omów kontrargumenty i podsumuj warunki zatrzymania wdrożenia. 

PYTANIE DO SALI: W którym zadaniu model jest najmniej potrzebny?
Omów co najmniej dwie możliwe odpowiedzi, wskazując ich warunki i konsekwencje.

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


## MODUŁ 2: BIG DATA: OD ZDARZENIA DO WIEDZY (75 minut)

**Slajd otwierający (2 min)**: wprowadź pytanie przewodnie.


### SLAJD 20: Big Data bez marketingu (4 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: BIG DATA: OD ZDARZENIA DO WIEDZY | SLAJD: 20 | CZAS: 4 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Big Data staje się problemem architektonicznym, kiedy proste, scentralizowane sposoby przetwarzania przestają spełniać wymagania czasu, skali, bezpieczeństwa lub kosztu. Pięć V jest heurystyką, nie definicją naukową.

ROZWINIĘCIE PLANSZY:
Punkt 1: Volume: skala. Punkt 2: Velocity: tempo. Punkt 3: Variety: różnorodność. Punkt 4: Veracity / Value: jakość i użyteczność.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 21: Dane ≠ informacja ≠ wiedza (4 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: BIG DATA: OD ZDARZENIA DO WIEDZY | SLAJD: 21 | CZAS: 4 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
W dowolnej organizacji surowe liczby nie wystarczają. Liczba 4350 nic nie oznacza bez jednostki, daty, typu dokumentu i źródła. Przechodząc do wiedzy, potrzebujemy semantyki: co oznacza „należne”, a co „zapłacone”.

ROZWINIĘCIE PLANSZY:
Punkt 1: Dane: 4350. Punkt 2: Informacja: kwota czynszu za miesiąc. Punkt 3: Wiedza: skąd wynika należność. Punkt 4: Decyzja: kiedy i komu przypomnieć.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 22: Jedna organizacja. Siedem strumieni (4 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: BIG DATA: OD ZDARZENIA DO WIEDZY | SLAJD: 22 | CZAS: 4 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Porozmawiaj o przedsiębiorstwie, które ma sto sposobów zapisu jednej sprawy. Z perspektywy systemu AI nie ma jednej prawdy, tylko fragmenty. Pierwsza decyzja architektoniczna to identyfikacja systemów źródłowych i właścicieli danych.

ROZWINIĘCIE PLANSZY:
Punkt 1: Źródła transakcyjne: ERP / CRM. Punkt 2: Semi-structured: JSON / logi. Punkt 3: Nieustrukturyzowane: PDF / wiadomości. Punkt 4: Strumienie: czujniki / zdarzenia.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 23: Pipeline danych (4 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: BIG DATA: OD ZDARZENIA DO WIEDZY | SLAJD: 23 | CZAS: 4 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Narysuj przepływ surowych danych. Każda transformacja powinna być odtwarzalna, a różnice między surowym rekordem i informacją używaną do decyzji widoczne. Bez tego trudno wskazać, skąd wzięło się błędne rozliczenie.

ROZWINIĘCIE PLANSZY:
Punkt 1: Ingest: przechwycenie. Punkt 2: Transform: oczyszczanie i mapowanie. Punkt 3: Store: surowe i gotowe warstwy. Punkt 4: Serve: analityka, model, agent.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 24: ETL kontra ELT (4 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: BIG DATA: OD ZDARZENIA DO WIEDZY | SLAJD: 24 | CZAS: 4 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Nie chodzi o wybór religii danych. W ETL transformacja poprzedza docelowe składowanie, w ELT źródło trafia najpierw do platformy, na której jest przetwarzane. Każde podejście potrzebuje walidacji i kontrolowania jakości.

ROZWINIĘCIE PLANSZY:
Punkt 1: ETL: przekształć przed zapisem. Punkt 2: ELT: zapisz, a potem przekształcaj. Punkt 3: Strefa raw ≠ zaufana tabela. Punkt 4: Wybór zależy od platformy i wymagań.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 25: Batch i streaming (4 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: BIG DATA: OD ZDARZENIA DO WIEDZY | SLAJD: 25 | CZAS: 4 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Zapytaj: czy raport o sprzedaży musi mieć aktualność sekundy? Jeśli nie, batch może być prostszy i tańszy. Jeśli uruchamiamy detekcję awarii urządzenia, opóźnienie może być częścią ryzyka. Nie każdy strumień wymaga niskiej latencji.

ROZWINIĘCIE PLANSZY:
Punkt 1: Batch: harmonogram i okno. Punkt 2: Streaming: zdarzenia napływają stale. Punkt 3: Near-real-time: kompromis. Punkt 4: SLA opóźnienia wyznacza architekturę.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 26: Zdarzenie jako podstawowa jednostka (4 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: BIG DATA: OD ZDARZENIA DO WIEDZY | SLAJD: 26 | CZAS: 4 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Event-sourcing pokazuje różnicę między zapisem zdarzeń a bieżącą projekcją stanu. „Autoryzowano” nie jest równoznaczne z „rozliczono”. Jeżeli system generuje event „Sprawa zamknięta” z obietnicy, samo odtwarzanie go nie naprawi błędnej semantyki.

ROZWINIĘCIE PLANSZY:
Punkt 1: OrderCreated. Punkt 2: PaymentAuthorized. Punkt 3: PaymentSettled. Punkt 4: CaseClosed.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 27: Kafka: log zdarzeń, nie magiczna szyna (3 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: BIG DATA: OD ZDARZENIA DO WIEDZY | SLAJD: 27 | CZAS: 3 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Wytłumacz pojęcie klucza partycji, np. invoice_id. Zdarzenia tej faktury mogą zachować kolejność w ramach jednej partycji, lecz nie oznacza to globalnego porządku całego systemu. Konsument może się zatrzymać i wznowić od offsetu.

ROZWINIĘCIE PLANSZY:
Punkt 1: Producent publikuje zdarzenie. Punkt 2: Topic dzieli się na partycje. Punkt 3: Consumer group rozdziela pracę. Punkt 4: Porządek jest gwarantowany w partycji.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

ŹRÓDŁO / KONTEKST: https://kafka.apache.org/documentation.html

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 28: Exactly-once? Uważaj na zakres gwarancji (3 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: BIG DATA: OD ZDARZENIA DO WIEDZY | SLAJD: 28 | CZAS: 3 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Nazwą exactly-once bywa określona gwarancja przetwarzania w środowisku i z konkretnym sinkiem. Nie wolno automatycznie przekładać jej na skutek zewnętrzny w dowolnym API. Dla operacji finansowej dodaj idempotency key i odczyt stanu po operacji.

ROZWINIĘCIE PLANSZY:
Punkt 1: At-most-once: możliwa utrata. Punkt 2: At-least-once: możliwe powtórzenia. Punkt 3: Exactly-once: określony zakres semantyki. Punkt 4: API płatności wymaga idempotencji.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 29: Spark: przetwarzanie rozproszone (3 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: BIG DATA: OD ZDARZENIA DO WIEDZY | SLAJD: 29 | CZAS: 3 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Rozkładając obliczenie na maszyny, zyskujemy równoległość, lecz płacimy za komunikację, pamięć i nierównomierność danych. Wyjaśnij shuffle na agregacji po kliencie i pokaż, dlaczego nieprawidłowe partycjonowanie może zabijać wydajność.

ROZWINIĘCIE PLANSZY:
Punkt 1: DataFrame dzieli dane na partycje. Punkt 2: Transformacje tworzą plan. Punkt 3: Action uruchamia wykonanie. Punkt 4: Shuffle oznacza koszt wymiany.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

ŹRÓDŁO / KONTEKST: https://spark.apache.org/docs/latest/

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 30: MapReduce: historyczna intuicja (3 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: BIG DATA: OD ZDARZENIA DO WIEDZY | SLAJD: 30 | CZAS: 3 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Przykład: liczenie liczby zdarzeń na klienta. Map emituje pary klient i 1, shuffle grupuje, reduce sumuje. Choć współczesne silniki są bogatsze, ten model pomaga zobaczyć koszt przesuwania danych.

ROZWINIĘCIE PLANSZY:
Punkt 1: Map: przekształć rekord. Punkt 2: Shuffle: pogrupuj po kluczu. Punkt 3: Reduce: zagreguj. Punkt 4: Spark rozwija ideę poza prosty schemat.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 31: Okna czasu i spóźnione zdarzenia (3 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: BIG DATA: OD ZDARZENIA DO WIEDZY | SLAJD: 31 | CZAS: 3 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
W logistyce czujnik może wysłać pakiet po pięciu minutach offline. Jeżeli sumujemy zdarzenia według czasu przyjścia, raport będzie fałszywy. Wprowadź pojęcie watermarks jako reguły obsługi spóźnień i opisz trade-off między aktualnością a kompletnością.

ROZWINIĘCIE PLANSZY:
Punkt 1: Event time: kiedy zaszło. Punkt 2: Processing time: kiedy przetworzono. Punkt 3: Watermark: tolerancja opóźnienia. Punkt 4: Okno i korekty wyników.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

ŹRÓDŁO / KONTEKST: https://spark.apache.org/docs/latest/streaming/index.html

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 32: Warehouse, lake, lakehouse (3 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: BIG DATA: OD ZDARZENIA DO WIEDZY | SLAJD: 32 | CZAS: 3 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Porównaj schema-on-write, schema-on-read oraz warstwy table format w lakehouse. Zwróć uwagę, że słowa nie zastąpią projektu bezpieczeństwa, katalogowania i właściwego zapisu zmian. Nie każde przedsiębiorstwo potrzebuje tej samej platformy.

ROZWINIĘCIE PLANSZY:
Punkt 1: Warehouse: modelowane dane analityczne. Punkt 2: Lake: różnorodne dane i pliki. Punkt 3: Lakehouse: tablice na plikach z metadanymi. Punkt 4: Nie ma jednej odpowiedzi na wszystkie potrzeby.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 33: Parquet, partycje i kolumny (3 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: BIG DATA: OD ZDARZENIA DO WIEDZY | SLAJD: 33 | CZAS: 3 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Przykład tabeli z 100 kolumnami i raportu używającego trzech. Format kolumnowy pozwala nie czytać każdej wartości. Uporządkuj temat partycjonowania: jeżeli partycji jest za dużo lub mają nierówną wielkość, pojawią się kolejne problemy.

ROZWINIĘCIE PLANSZY:
Punkt 1: Columnar: odczyt potrzebnych kolumn. Punkt 2: Kompresja: typy i powtarzalność. Punkt 3: Partition pruning: mniej plików. Punkt 4: Small files: koszt metadanych.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 34: Iceberg / Delta: tabele na plikach (3 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: BIG DATA: OD ZDARZENIA DO WIEDZY | SLAJD: 34 | CZAS: 3 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Zwróć uwagę, że pliki w obiekcie storage nie tworzą jeszcze spójnej bazy transakcyjnej. Format tabeli opisuje ich wspólny stan. Pozwala ewoluować schemat, czytać snapshoty i uniknąć szeregu problemów z równoległym zapisem.

ROZWINIĘCIE PLANSZY:
Punkt 1: Pliki danych + metadane. Punkt 2: Snapshot: stan logiczny tabeli. Punkt 3: Schema evolution. Punkt 4: Transakcje i historyczność zależą od implementacji.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

ŹRÓDŁO / KONTEKST: https://iceberg.apache.org/spec/

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 35: Data quality jako infrastruktura zaufania (3 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: BIG DATA: OD ZDARZENIA DO WIEDZY | SLAJD: 35 | CZAS: 3 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Niech studenci wymienią jeden błąd danych, który mógłby zmienić decyzję. Brak faktury, duplikat płatności, sprzeczne identyfikatory czy nieaktualne stawki to nie kosmetyka. Testy jakości powinny być uruchamiane automatycznie i mieć właściciela.

ROZWINIĘCIE PLANSZY:
Punkt 1: Completeness. Punkt 2: Validity. Punkt 3: Uniqueness. Punkt 4: Timeliness / consistency.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 36: Data lineage i pochodzenie (3 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: BIG DATA: OD ZDARZENIA DO WIEDZY | SLAJD: 36 | CZAS: 3 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Przeprowadź ścieżkę „raport pokazuje 4 350 zł” wstecz do wpisu w umowie, wzoru waloryzacji i stanu rozliczenia. Gdy model podejmuje decyzje, każda wartość powinna mieć drogę powrotu do dowodów.

ROZWINIĘCIE PLANSZY:
Punkt 1: Źródło rekordów. Punkt 2: Transformacje i wersje. Punkt 3: Autor / system / czas. Punkt 4: Powtarzalność i audyt.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

ŹRÓDŁO / KONTEKST: https://www.w3.org/TR/prov-o/

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 37: Katalog danych i uprawnienia (3 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: BIG DATA: OD ZDARZENIA DO WIEDZY | SLAJD: 37 | CZAS: 3 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Podkreśl różnicę między operacyjną kontrolą dostępu a podstawą prawną i celem przetwarzania. Dane osobowe czy informacje handlowe nie stają się bezpieczne dlatego, że trafiły do chmury. Odpowiedzialność obejmuje całą ścieżkę.

ROZWINIĘCIE PLANSZY:
Punkt 1: Właściciel zbioru. Punkt 2: Klasyfikacja danych. Punkt 3: Polityka dostępu i retencja. Punkt 4: Pseudonimizacja nie zawsze anonimizuje.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 38: Feature store, vector store, knowledge graph (3 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: BIG DATA: OD ZDARZENIA DO WIEDZY | SLAJD: 38 | CZAS: 3 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
To klucz do połączenia Big Data z AI. Feature store pilnuje spójnych cech trenowania i inferencji, vector store szuka podobnych fragmentów, a graf opisuje relacje obiektów. Trzy różne potrzeby i trzy różne możliwości pomyłki.

ROZWINIĘCIE PLANSZY:
Punkt 1: Feature store: cechy dla modeli. Punkt 2: Vector store: podobieństwo. Punkt 3: Graph: relacje i tożsamość. Punkt 4: Łączenie, nie bezmyślna zamiana.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 39: Big Data → AI: zasilanie modelu (3 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: BIG DATA: OD ZDARZENIA DO WIEDZY | SLAJD: 39 | CZAS: 3 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Zbierz całość na jednej architekturze. Model językowy nie powinien przeliczać systemu finansowego z kopii maili, jeśli istnieje system transakcyjny. Dobrze zbudowana warstwa danych czyni działanie modeli sprawdzalnym.

ROZWINIĘCIE PLANSZY:
Punkt 1: Zdarzenia → lakehouse. Punkt 2: Jakość i mapowanie encji. Punkt 3: Indeks / cechy / graf. Punkt 4: Model + walidacja + człowiek.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 40: LAB BIG DATA: awaria raportu (6 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: BIG DATA: OD ZDARZENIA DO WIEDZY | SLAJD: 40 | CZAS: 6 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Daj pięć minut na diagnozę. Uczestnicy mają wypisać trzy hipotezy i trzy testy. Odpowiedzi: różne momenty cyklu zamówienia, duplikacja zdarzeń, brak rozliczenia, różne klucze i daty. Nie wolno bezmyślnie policzyć średniej z trzech liczb.

ROZWINIĘCIE PLANSZY:
Punkt 1: CRM ma 500 zamówień. Punkt 2: ERP ma 480 faktur. Punkt 3: Broker zdarzeń pokazuje 510 eventów. Punkt 4: Zadanie: co jest zdarzeniem, a co stanem?.

PROWADZENIE I PRZYKŁAD:
Praca z salą: najpierw przedstaw scenariusz i rozdziel role. Następnie daj grupom czas na zapisanie odpowiedzi na kartce, niech nie wybierają od razu narzędzia. Obejdź zespoły i pytaj o źródło danych, semantykę stanów, wyjątki oraz właściciela decyzji. Zaproś co najmniej dwa zespoły do przedstawienia odmiennego rozwiązania; omów kontrargumenty i podsumuj warunki zatrzymania wdrożenia. 

PYTANIE DO SALI: Jaką metrykę biznesową liczymy i z którego stanu?
Omów co najmniej dwie możliwe odpowiedzi, wskazując ich warunki i konsekwencje.

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


## MODUŁ 3: ONTOLOGIE: ŚWIAT PRZED ALGORYTMEM (65 minut)

**Slajd otwierający (2 min)**: wprowadź pytanie przewodnie.


### SLAJD 42: Ontologia: co system uznaje za istniejące (4 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: ONTOLOGIE: ŚWIAT PRZED ALGORYTMEM | SLAJD: 42 | CZAS: 4 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Nawiąż wprost do wystąpienia w Warszawie 19 listopada. Ontologia nie jest poetycką dekoracją AI, lecz jawnym opisem świata, w którym system ma działać. Bez niej napis „zamknięte” może znaczyć koniec rozmowy, zapłatę faktury albo zakończenie zadania.

ROZWINIĘCIE PLANSZY:
Punkt 1: Obiekty. Punkt 2: Relacje. Punkt 3: Właściwości i ograniczenia. Punkt 4: Zdarzenia, czas, źródła.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

ŹRÓDŁO / KONTEKST: Wystąpienie autora „System, który wszedł do świata”, Warszawa, 19.11.2026

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 43: Ontologia filozoficzna a informatyczna (4 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: ONTOLOGIE: ŚWIAT PRZED ALGORYTMEM | SLAJD: 43 | CZAS: 4 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Powiedz studentom, że model pojęciowy może być celowo niekompletny. Wybieramy rozróżnienia istotne dla zadań systemu. Pytanie filozoficzne o naturę faktu jest głębsze, ale system praktycznie wymaga operacyjnych definicji i reguł identyfikacji.

ROZWINIĘCIE PLANSZY:
Punkt 1: Filozofia: co istnieje i czym jest?. Punkt 2: Informatyka: jakie kategorie reprezentujemy?. Punkt 3: Ontologia domenowa jest decyzją projektową. Punkt 4: Model pojęciowy nie jest światem.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 44: Klient, faktura, obietnica, wpłata (4 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: ONTOLOGIE: ŚWIAT PRZED ALGORYTMEM | SLAJD: 44 | CZAS: 4 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
To przykład przewodni warszawskiej konferencji. Obietnica nie jest wpłatą. Instrukcja „zamknij sprawę” nie daje uprawnienia do dokonania rozliczenia. Jeżeli model językowy wyłuska prawidłowe słowa, ale przypisze niewłaściwe typy bytów, cały system podejmie złą decyzję.

ROZWINIĘCIE PLANSZY:
Punkt 1: Klient C-17: tożsamość. Punkt 2: Faktura F-42: zobowiązanie. Punkt 3: Obietnica P-8: deklaracja. Punkt 4: Wpłata W-5: zdarzenie potwierdzone.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 45: TBox i ABox (3 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: ONTOLOGIE: ŚWIAT PRZED ALGORYTMEM | SLAJD: 45 | CZAS: 3 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
TBox mówi, że istnieją faktury i klienci, oraz jakie relacje są dopuszczalne. ABox stwierdza, że konkretny klient ma daną fakturę. Bez tego oddzielenia łatwo pomieszać założenia systemowe z danymi o pojedynczym przypadku.

ROZWINIĘCIE PLANSZY:
Punkt 1: TBox: definicje klas i relacji. Punkt 2: ABox: konkretne instancje. Punkt 3: Klient ≠ konkretna osoba. Punkt 4: Spójność typów i instancji.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 46: Identyfikatory, a nie podobne napisy (3 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: ONTOLOGIE: ŚWIAT PRZED ALGORYTMEM | SLAJD: 46 | CZAS: 3 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Zadaj pytanie: co zrobić z dwoma rekordami tej samej firmy w CRM i ERP? Podobieństwo nazwy nie wystarcza do scalenia. Potrzebujemy reguły tożsamości, źródeł i mechanizmu rozstrzygania kolizji.

ROZWINIĘCIE PLANSZY:
Punkt 1: „ABC sp. z o.o.” vs „ABC”. Punkt 2: NIP / ID / numer źródłowy. Punkt 3: Alias to nie nowy obiekt. Punkt 4: Błędne scalenie może być groźne.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 47: RDF: wiedza jako trójki (3 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: ONTOLOGIE: ŚWIAT PRZED ALGORYTMEM | SLAJD: 47 | CZAS: 3 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Pokaż, jak zapis w RDF tworzy graf, nie gotową tabelę w Excelu. Każda relacja ma znaczenie. Węzły są identyfikowalne, a predykat opisuje rolę połączenia. Wytłumacz też znaczenie URI jako identyfikatora zasobu.

ROZWINIĘCIE PLANSZY:
Punkt 1: Klient_C17 → posiada → Faktura_F42. Punkt 2: Faktura_F42 → maStan → Otwarta. Punkt 3: Obietnica_P8 → dotyczy → Faktura_F42. Punkt 4: Wpłata_W5 → rozlicza → Faktura_F42.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

ŹRÓDŁO / KONTEKST: https://www.w3.org/TR/rdf11-concepts/

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 48: Graf wiedzy: reprezentacja relacji (3 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: ONTOLOGIE: ŚWIAT PRZED ALGORYTMEM | SLAJD: 48 | CZAS: 3 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Zbuduj narrację od relacji do faktu. Jedna wpłata może rozliczać kilka faktur, jedna faktura może mieć kilka wpłat. Graf pozwala wyrazić takie zależności jawnie, ale jakość grafu nadal zależy od poprawności danych i modelowania.

ROZWINIĘCIE PLANSZY:
Punkt 1: Klient → Umowa → Faktura. Punkt 2: Faktura ← Obietnica. Punkt 3: Faktura ← Alokacja ← Wpłata. Punkt 4: Sprawa → maStan → Otwarta.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 49: OWL 2 i wnioskowanie (3 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: ONTOLOGIE: ŚWIAT PRZED ALGORYTMEM | SLAJD: 49 | CZAS: 3 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
OWL nadaje formalną semantykę ontologii. Jeżeli określimy, że każda faktura jest dokumentem finansowym, system może wnioskować o klasie dokumentu. To nie jest magia LLM, tylko konsekwencja aksjomatów. Uwaga: brak jawnej sprzeczności nie musi oznaczać kompletności danych.

ROZWINIĘCIE PLANSZY:
Punkt 1: Klasy i podklasy. Punkt 2: Domena / zakres relacji. Punkt 3: Ograniczenia logiczne. Punkt 4: Reasoner sprawdza wnioski i sprzeczności.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

ŹRÓDŁO / KONTEKST: https://www.w3.org/TR/owl-overview/

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 50: Open World vs Closed World (3 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: ONTOLOGIE: ŚWIAT PRZED ALGORYTMEM | SLAJD: 50 | CZAS: 3 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Przykład: jeśli graf nie zawiera wpłaty, nie znaczy to, że klient nie zapłacił. Może brakować synchronizacji. Silnik reguł dla naliczania odsetek powinien sprawdzić autorytatywny rejestr, nie tylko brak trójki w grafie.

ROZWINIĘCIE PLANSZY:
Punkt 1: OWL: brak faktu nie oznacza zaprzeczenia. Punkt 2: Baza transakcyjna często stosuje logikę zamkniętą. Punkt 3: Nieobecność wpłaty nie dowodzi, że jej nie było. Punkt 4: Do działania potrzebna polityka i źródło rozstrzygające.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 51: SHACL: reguły poprawności danych (3 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: ONTOLOGIE: ŚWIAT PRZED ALGORYTMEM | SLAJD: 51 | CZAS: 3 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
SHACL pozwala opisać ograniczenia strukturalne, których dane mają przestrzegać. Użyj przykładu faktury bez waluty albo z dwoma sprzecznymi statusami. SHACL nie rozstrzyga całej prawdy, ale bardzo dobrze wykrywa część nieprawidłowych rekordów.

ROZWINIĘCIE PLANSZY:
Punkt 1: Faktura wymaga identyfikatora. Punkt 2: Kwota jest typu liczbowego. Punkt 3: Termin ma poprawny format. Punkt 4: Stan rozliczenia spełnia kontrakt.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

ŹRÓDŁO / KONTEKST: https://www.w3.org/TR/shacl/

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 52: Ontologia czasu (3 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: ONTOLOGIE: ŚWIAT PRZED ALGORYTMEM | SLAJD: 52 | CZAS: 3 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Na konferencji mówiłeś, że czas zmienia znaczenie faktu. Zrób z tego model temporalny: „ma być opłacone w piątek” to informacja o przyszłości, a „zostało opłacone w piątek” to twierdzenie o zdarzeniu. System nie może tego zlać w jedno.

ROZWINIĘCIE PLANSZY:
Punkt 1: Zdarzenie: PaymentSettled. Punkt 2: Stan: faktura opłacona. Punkt 3: Przedział ważności stanu. Punkt 4: Warunek zmiany i źródło potwierdzenia.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 53: Bitemporalność danych (3 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: ONTOLOGIE: ŚWIAT PRZED ALGORYTMEM | SLAJD: 53 | CZAS: 3 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Wyjaśnij bitemporalność na opóźnionej informacji o wpłacie. Płatność miała miejsce o 15:00, ale system dowiedział się o niej o 16:30. Historia powinna pozwalać odtworzyć oba fakty, bo oceniając decyzję agenta sprawdzamy także dostępne wówczas dane.

ROZWINIĘCIE PLANSZY:
Punkt 1: Valid time: czas świata. Punkt 2: Transaction time: czas zapisu. Punkt 3: Korekta z datą wsteczną. Punkt 4: Audyt stanu wiedzy w chwili decyzji.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 54: Pochodzenie wiedzy: PROV-O (3 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: ONTOLOGIE: ŚWIAT PRZED ALGORYTMEM | SLAJD: 54 | CZAS: 3 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Pokaż łańcuch: wiadomość klienta, ekstrakcja deklaracji, zapis do CRM, decyzja systemu. Samo stwierdzenie „dane są w bazie” nie wyjaśnia, dlaczego uznajemy je za prawdziwe. W standardzie PROV-O opisujemy pochodzenie i udział podmiotów.

ROZWINIĘCIE PLANSZY:
Punkt 1: Entity: dokument, rekord, raport. Punkt 2: Activity: transformacja, obliczenie. Punkt 3: Agent: osoba lub system. Punkt 4: wasDerivedFrom / wasGeneratedBy.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

ŹRÓDŁO / KONTEKST: https://www.w3.org/TR/prov-o/

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 55: Ontologia kontra embedding (3 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: ONTOLOGIE: ŚWIAT PRZED ALGORYTMEM | SLAJD: 55 | CZAS: 3 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Powtórz dwa pozornie podobne zdania: „klient zapłacił” i „klient nie zapłacił”. Retrieval może zwrócić oba. Dopiero sprawdzenie zaufanego stanu, typu zdarzenia oraz daty pozwala podjąć odpowiedzialną decyzję.

ROZWINIĘCIE PLANSZY:
Punkt 1: Embedding: podobne teksty blisko. Punkt 2: Graf: jawne typy i relacje. Punkt 3: Reguła: wymóg dowodowy. Punkt 4: W praktyce łączymy trzy metody.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 56: GraphRAG: od dokumentu do struktury (3 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: ONTOLOGIE: ŚWIAT PRZED ALGORYTMEM | SLAJD: 56 | CZAS: 3 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
GraphRAG to rodzina wzorców, a nie magiczny przycisk. Wspomaga pytania o relacje między zdarzeniami, aktorami i dokumentami. Trzeba jednak walidować ekstrakcję grafu i pochodzenie relacji, bo model może stworzyć błędne połączenia.

ROZWINIĘCIE PLANSZY:
Punkt 1: Dokumenty → encje i relacje. Punkt 2: Graf → ścieżki i kontekst. Punkt 3: Wyszukiwanie → dowód ze źródeł. Punkt 4: Odpowiedź → cytaty i ograniczenia.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 57: Ontologiczny kontrakt działania (3 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: ONTOLOGIE: ŚWIAT PRZED ALGORYTMEM | SLAJD: 57 | CZAS: 3 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Pokaż kontrakt jako zestaw warunków wstępnych, uprawnień i warunków końcowych. Sama predykcja modelu nie powinna przepisywać stanów finansowych. To właśnie moment przejścia od generowania języka do zmiany rzeczywistości, centralny dla wystąpienia warszawskiego.

ROZWINIĘCIE PLANSZY:
Punkt 1: Typy: zamknięcie sprawy ≠ rozliczenie. Punkt 2: Dowód: płatność w rejestrze. Punkt 3: Prawo: użytkownik ma uprawnienie. Punkt 4: Skutek: stan potwierdzony po API.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 58: Ontologia organizacji (3 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: ONTOLOGIE: ŚWIAT PRZED ALGORYTMEM | SLAJD: 58 | CZAS: 3 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Semantyczne konflikty istnieją nawet wtedy, gdy integracja API działa idealnie. Pracownicy często nauczyli się tych różnic przez doświadczenie. Agent nie ma tego kontekstu, dopóki nie przedstawimy go jawnie w modelu domeny i polityce działania.

ROZWINIĘCIE PLANSZY:
Punkt 1: CRM „zamknięte” = obsłużona rozmowa. Punkt 2: ERP „zamknięte” = rozliczony dokument. Punkt 3: HR „zweryfikowany” = zakończony etap. Punkt 4: Agent musi znać zakres pojęcia.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 59: Ontologia celów wielu agentów (3 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: ONTOLOGIE: ŚWIAT PRZED ALGORYTMEM | SLAJD: 59 | CZAS: 3 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Przedstaw dwa agentowe KPI, które ze sobą walczą. Jeden zamyka sprawę, drugi ją otwiera. Jeśli nie uzgodnimy semantyki stanów oraz hierarchii celów, automatyzacja zamieni organizację w system konfliktujących optymalizatorów.

ROZWINIĘCIE PLANSZY:
Punkt 1: Agent obsługi: zamknij jak najwięcej. Punkt 2: Agent należności: pilnuj otwartych. Punkt 3: Agent jakości: minimalizuj błędy. Punkt 4: Cel systemu: spójny wynik organizacji.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 60: LAB: stwórz ontologię jednej sprawy (6 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: ONTOLOGIE: ŚWIAT PRZED ALGORYTMEM | SLAJD: 60 | CZAS: 6 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Warsztat. Podziel salę na zespoły. Daj sześć minut na schemat grafu i dwa na wskazanie konsekwencji. Sprawdź, czy powstały oddzielne klasy PaymentPromise i PaymentSettlement. Następnie pytaj, skąd system wie, że rozliczenie nastąpiło.

ROZWINIĘCIE PLANSZY:
Punkt 1: Zdefiniuj 6 klas i 8 relacji. Punkt 2: Oznacz zdarzenie, stan, deklarację. Punkt 3: Dodaj źródła i dwa czasy. Punkt 4: Zapisz 3 warunki bezpiecznego działania.

PROWADZENIE I PRZYKŁAD:
Praca z salą: najpierw przedstaw scenariusz i rozdziel role. Następnie daj grupom czas na zapisanie odpowiedzi na kartce, niech nie wybierają od razu narzędzia. Obejdź zespoły i pytaj o źródło danych, semantykę stanów, wyjątki oraz właściciela decyzji. Zaproś co najmniej dwa zespoły do przedstawienia odmiennego rozwiązania; omów kontrargumenty i podsumuj warunki zatrzymania wdrożenia. 

PYTANIE DO SALI: Co musi się wydarzyć, zanim agent zamknie należność?
Omów co najmniej dwie możliwe odpowiedzi, wskazując ich warunki i konsekwencje.

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


## MODUŁ 4: SYSTEM, KTÓRY WSZEDŁ DO ŚWIATA (60 minut)

**Slajd otwierający (2 min)**: wprowadź pytanie przewodnie.


### SLAJD 62: Od odpowiedzi do operacji (4 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: SYSTEM, KTÓRY WSZEDŁ DO ŚWIATA | SLAJD: 62 | CZAS: 4 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Nawiąż do tezy konferencyjnej, ale rozwiń ją na konkretnych interfejsach. Dotąd AI mogła głównie doradzać, teraz coraz częściej wywołuje narzędzia i zmienia stany. Nie oznacza to, że wcześniej nie było automatyki: zmienia się sposób delegowania celu i kontekstowej selekcji działań.

ROZWINIĘCIE PLANSZY:
Punkt 1: Model proponuje interpretację. Punkt 2: Planner wybiera operację. Punkt 3: Narzędzie zapisuje zmianę. Punkt 4: Organizacja ponosi skutek.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

ŹRÓDŁO / KONTEKST: Wystąpienie autora „System, który wszedł do świata”, Warszawa, 19.11.2026

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 63: Deklaracja, obserwacja, hipoteza, potwierdzenie (4 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: SYSTEM, KTÓRY WSZEDŁ DO ŚWIATA | SLAJD: 63 | CZAS: 4 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
To, że LLM mówi pełnym zdaniem, nie oznacza pewności epistemicznej. Naucz odróżniać, skąd bierze się każda informacja. Jeśli status deklaracji zostanie zamieniony na potwierdzenie, firma może przerwać prawidłowy proces windykacyjny.

ROZWINIĘCIE PLANSZY:
Punkt 1: Deklaracja: „zapłacimy”. Punkt 2: Obserwacja: dane z systemu. Punkt 3: Hipoteza: „prawdopodobnie”. Punkt 4: Potwierdzenie: dowód rozliczenia.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 64: Pętla agenta: perceive → plan → act → observe (4 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: SYSTEM, KTÓRY WSZEDŁ DO ŚWIATA | SLAJD: 64 | CZAS: 4 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Przejdź cykl dwukrotnie: najpierw w hipotetycznym sukcesie, potem w awarii API. Agentowi nie wolno zakładać wykonania tylko na podstawie wysłanego żądania. Każdy cykl wymaga kryterium zatrzymania.

ROZWINIĘCIE PLANSZY:
Punkt 1: Perceive: odczytaj zaufany stan. Punkt 2: Plan: zaproponuj krok. Punkt 3: Act: sprawdź uprawnienia. Punkt 4: Observe: potwierdź stan.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 65: Różnica między workflow a agentem (4 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: SYSTEM, KTÓRY WSZEDŁ DO ŚWIATA | SLAJD: 65 | CZAS: 4 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Zestaw powtarzalne księgowanie z nieustrukturyzowaną obsługą zapytania. Tam, gdzie kroki są znane, zwykła automatyzacja może być bardziej kontrolowalna. Agent jest zasadny, kiedy zmieniający się kontekst wymaga wyboru drogi.

ROZWINIĘCIE PLANSZY:
Punkt 1: Workflow: kroki zapisane z góry. Punkt 2: Agent: dobiera kroki do kontekstu. Punkt 3: Oba potrzebują testów i logowania. Punkt 4: Nie każdemu procesowi warto dawać autonomię.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 66: Contract-first agent (4 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: SYSTEM, KTÓRY WSZEDŁ DO ŚWIATA | SLAJD: 66 | CZAS: 4 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Ułóż na tablicy kontrakt dla operacji close_case(case_id). Przed wykonaniem sprawdzamy, czy stan jest zgodny, jaka jest wersja rekordu i czy odpowiednia rola autoryzuje akcję. Po wykonaniu ponownie odczytujemy stan, zapisując dowód.

ROZWINIĘCIE PLANSZY:
Punkt 1: Input contract / schema. Punkt 2: Preconditions. Punkt 3: Authorization. Punkt 4: Postcondition i rollback plan.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 67: Policy engine poza LLM (4 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: SYSTEM, KTÓRY WSZEDŁ DO ŚWIATA | SLAJD: 67 | CZAS: 4 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Powiedz jasno: model może zaproponować działanie, ale polityka jest egzekwowana poza nim. Przykładowo zapis oferty na 20 000 zł lub wysłanie odpowiedzi prawnej wymaga innych uprawnień niż samo streszczenie dokumentu.

ROZWINIĘCIE PLANSZY:
Punkt 1: RBAC / ABAC. Punkt 2: Allowlist narzędzi. Punkt 3: Granice finansowe. Punkt 4: Approval dla operacji nieodwracalnych.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 68: Idempotencja i ponowienie operacji (4 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: SYSTEM, KTÓRY WSZEDŁ DO ŚWIATA | SLAJD: 68 | CZAS: 4 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
W rozproszonym świecie sieć może przerwać połączenie po wykonaniu operacji. Agent nie wie wtedy, czy sukces nastąpił. Ponowienie tego samego przelewu bez zabezpieczeń jest ryzykowne. Idempotencja i kontrola stanu są odpowiedzią architektoniczną.

ROZWINIĘCIE PLANSZY:
Punkt 1: Idempotency key. Punkt 2: Retry with backoff. Punkt 3: Read-after-write. Punkt 4: Deduplikacja efektu.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 69: Kompensacje i saga (4 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: SYSTEM, KTÓRY WSZEDŁ DO ŚWIATA | SLAJD: 69 | CZAS: 4 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Niektóre operacje są rozproszone pomiędzy CRM, ERP i pocztą. Jeśli wysłaliśmy wiadomość, nie możemy jej „odwysłać”. Możemy jednak uruchomić zaplanowaną kompensację lub eskalację. Omów mechanizm saga jako wzorzec przepływu, a nie gwarancję odwracalności świata.

ROZWINIĘCIE PLANSZY:
Punkt 1: Seria kroków w wielu systemach. Punkt 2: Częściowe wykonanie. Punkt 3: Akcja kompensująca. Punkt 4: Audyt wyjątków i eskalacja.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 70: Pamięć agenta z datą ważności (4 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: SYSTEM, KTÓRY WSZEDŁ DO ŚWIATA | SLAJD: 70 | CZAS: 4 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Zacytuj hipotetyczną pamięć: „klient obiecał wpłatę w piątek”. Bez daty i źródła system może użyć jej po miesiącu. To nie błąd lingwistyczny, lecz błąd ontologii pamięci. Dobry system ma politykę wygaśnięcia i odświeżania danych.

ROZWINIĘCIE PLANSZY:
Punkt 1: Treść i pochodzenie. Punkt 2: Data / czas ważności. Punkt 3: Warunek unieważnienia. Punkt 4: Źródło autorytatywne.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 71: Multi-agent to nie spotkanie botów (3 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: SYSTEM, KTÓRY WSZEDŁ DO ŚWIATA | SLAJD: 71 | CZAS: 3 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Pokazuję system trzech agentów: planista proponuje, wykonawca obsługuje narzędzie, recenzent ocenia dowód. Jeśli każdy działa na innej kopii danych, narasta ryzyko konfliktu. Architektura powinna określać arbiter i reguły synchronizacji.

ROZWINIĘCIE PLANSZY:
Punkt 1: Planner / executor / reviewer. Punkt 2: Wspólna tożsamość obiektów. Punkt 3: Granice przekazania uprawnień. Punkt 4: Jedno źródło decyzji końcowej.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 72: Obserwowalność: trace jednej decyzji (3 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: SYSTEM, KTÓRY WSZEDŁ DO ŚWIATA | SLAJD: 72 | CZAS: 3 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Przejdź przez pojedynczy trace. Potrzebujemy identyfikatora sprawy, wersji instrukcji, źródeł, weryfikacji polityki i efektu, ale nie oznacza to logowania niepotrzebnych danych osobowych. Obserwowalność jest częścią odpowiedzialności.

ROZWINIĘCIE PLANSZY:
Punkt 1: Input / wersja danych. Punkt 2: Wywołanie modelu i narzędzia. Punkt 3: Policy decision. Punkt 4: Efekt i finalny stan.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 73: Human-in-the-loop: pozór i rzeczywistość (3 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: SYSTEM, KTÓRY WSZEDŁ DO ŚWIATA | SLAJD: 73 | CZAS: 3 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Zadaj pytanie: czy osoba klikająca akceptację ma czas i możliwość sprawdzenia? Jeśli nie widzi oryginalnego dokumentu, ani tego, co system zamierza zmienić, kontrola jest iluzoryczna. Czasem lepiej ograniczyć autonomię niż udawać nadzór.

ROZWINIĘCIE PLANSZY:
Punkt 1: Dowód i kontekst przed decyzją. Punkt 2: Prawo sprzeciwu i czas. Punkt 3: Jasny właściciel decyzji. Punkt 4: Ślad audytowy bez nadmiernego gromadzenia.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 74: Pięć awarii ontologicznych (3 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: SYSTEM, KTÓRY WSZEDŁ DO ŚWIATA | SLAJD: 74 | CZAS: 3 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
To rozwinięcie warszawskiej listy awarii. Każdą potraktuj jak test: jakie dane wejściowe wytworzyły błąd, które prawo operacyjne mogło go zatrzymać, jaki dowód zobaczymy po wykonaniu? Dla studentów to wzorzec myślenia o bezpieczeństwie biznesowym.

ROZWINIĘCIE PLANSZY:
Punkt 1: Sprzeczne światy CRM / ERP. Punkt 2: Dryf znaczenia statusów. Punkt 3: Konflikt lokalnych celów. Punkt 4: Błędna klasyfikacja zdarzenia. Punkt 5: Luka odpowiedzialności.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 75: CASE: mail o płatności (4 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: SYSTEM, KTÓRY WSZEDŁ DO ŚWIATA | SLAJD: 75 | CZAS: 4 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Pokaż, że każde wywołanie API mogłoby być formalnie poprawne, a rezultat biznesowy fałszywy. Rozłóż błąd na poziom danych, semantyki, uprawnień i skutku. Następnie pokaż minimalny kontrakt, który blokuje automatyczne zamknięcie.

ROZWINIĘCIE PLANSZY:
Punkt 1: Ekstrakcja: jest obietnica. Punkt 2: Rejestr: brak potwierdzonej wpłaty. Punkt 3: Decyzja: nie zamykać należności. Punkt 4: Działanie: zapisać deklarację, zaplanować kontrolę.

PROWADZENIE I PRZYKŁAD:
Prowadzenie studium przypadku: nazwij aktorów, źródła danych, możliwe decyzje i koszt błędu. Wskaż konkretny moment, w którym interpretacja modelu może stać się operacją systemową. Poproś o alternatywną architekturę opartą na regułach lub prostszym modelu. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 76: DEBATA: kto jest winny? (6 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: SYSTEM, KTÓRY WSZEDŁ DO ŚWIATA | SLAJD: 76 | CZAS: 6 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Podziel studentów na cztery role. Każda ma obronić swój zakres odpowiedzialności, ale bez fikcji, że winę można przerzucić na model. Po sześciu minutach poproś o jedno narzędzie prewencyjne dla każdej roli i jedno kryterium eskalacji.

ROZWINIĘCIE PLANSZY:
Punkt 1: Scenariusz: błędne zamknięcie sprawy. Punkt 2: Role: architekt / product owner / auditor. Punkt 3: Dowody: log, kontrakt, źródło. Punkt 4: Wniosek: odpowiedzialność nie „wyparowuje”.

PROWADZENIE I PRZYKŁAD:
Praca z salą: najpierw przedstaw scenariusz i rozdziel role. Następnie daj grupom czas na zapisanie odpowiedzi na kartce, niech nie wybierają od razu narzędzia. Obejdź zespoły i pytaj o źródło danych, semantykę stanów, wyjątki oraz właściciela decyzji. Zaproś co najmniej dwa zespoły do przedstawienia odmiennego rozwiązania; omów kontrargumenty i podsumuj warunki zatrzymania wdrożenia. 

PYTANIE DO SALI: Co musi zostać w organizacji, nawet jeśli agent wykonuje 90% operacji?
Omów co najmniej dwie możliwe odpowiedzi, wskazując ich warunki i konsekwencje.

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


## MODUŁ 5: WDROŻENIA: OD DEMO DO PRODUKCJI (70 minut)

**Slajd otwierający (2 min)**: wprowadź pytanie przewodnie.


### SLAJD 78: Dlaczego większość demo jest za łatwa (4 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: WDROŻENIA: OD DEMO DO PRODUKCJI | SLAJD: 78 | CZAS: 4 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Zacznij od pytania, czy w pięciominutowej demonstracji pojawiają się sprzeczne dokumenty, brak danych, timeout lub błędne uprawnienia. Udany pokaz jest hipotezą o wartości, którą trzeba przetestować w produkcyjnej rzeczywistości.

ROZWINIĘCIE PLANSZY:
Punkt 1: Przykłady są wybrane. Punkt 2: Dane są oczyszczone. Punkt 3: Użytkownik zna zadanie. Punkt 4: Wyjątki są pomijane.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 79: Pięć etapów wdrożenia (4 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: WDROŻENIA: OD DEMO DO PRODUKCJI | SLAJD: 79 | CZAS: 4 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Wytłumacz różnicę między eksperymentem a pilotażem. PoC sprawdza czy metoda może działać. Pilot sprawdza czy integracja z procesem poprawia wynik. Wdrożenie skalowalne wymaga właściciela, wskaźników, obsługi wyjątków i finansowania.

ROZWINIĘCIE PLANSZY:
Punkt 1: Discovery: problem / odpowiedzialność. Punkt 2: PoC: wykonalność techniczna. Punkt 3: Pilot: proces i ludzie. Punkt 4: Scale: monitoring i utrzymanie.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 80: Problem statement na jedną stronę (4 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: WDROŻENIA: OD DEMO DO PRODUKCJI | SLAJD: 80 | CZAS: 4 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Nie akceptuj celu „wdrożyć AI”. Wymagaj konkretu: skrócić o 20% czas przygotowania oferty przy niepogorszonej liczbie reklamacji. Wyznacz też punkt odniesienia, bo bez baseline trudno wykazać jakąkolwiek poprawę.

ROZWINIĘCIE PLANSZY:
Punkt 1: Stan obecny i wąskie gardło. Punkt 2: Decyzja / czynność do wsparcia. Punkt 3: Koszt błędu i czasu. Punkt 4: Kryterium sukcesu mierzalne.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 81: Macierz doboru use case (4 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: WDROŻENIA: OD DEMO DO PRODUKCJI | SLAJD: 81 | CZAS: 4 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Przeprowadź szybkie porównanie trzech projektów. Asystent wiedzy może mieć mały próg wejścia, agent płatności znacznie większe ryzyko, a prognoza popytu wymaga historii dobrej jakości. Wynik macierzy to decyzja o kolejności inwestycji.

ROZWINIĘCIE PLANSZY:
Punkt 1: Dane: dostępność i jakość. Punkt 2: Integracja: nakład. Punkt 3: Ryzyko: pomyłka i prywatność. Punkt 4: Korzyść: oszczędność / jakość.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 82: Architektura wdrożenia: SaaS, API, on-prem (4 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: WDROŻENIA: OD DEMO DO PRODUKCJI | SLAJD: 82 | CZAS: 4 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Wybór nie powinien zależeć od mody. Zbierz wymagania dotyczące danych, kosztów, opóźnień, izolacji, dostępności i regulacji. Offline bywa droższe w utrzymaniu, a chmura nie zwalnia z odpowiedzialności za ochronę danych.

ROZWINIĘCIE PLANSZY:
Punkt 1: SaaS: szybkość i gotowe procesy. Punkt 2: API: elastyczność integracji. Punkt 3: On-prem: kontrola i odpowiedzialność. Punkt 4: Hybryda: mieszanka ról.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 83: Architektura referencyjna AI w firmie (3 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: WDROŻENIA: OD DEMO DO PRODUKCJI | SLAJD: 83 | CZAS: 3 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
To jedna z najważniejszych plansz całego dnia. Zwróć uwagę na oddzielenie płaszczyzny semantycznej od modelowej oraz płaszczyzny kontroli. Można zmienić dostawcę LLM i zachować politykę, model domeny i ślad audytowy.

ROZWINIĘCIE PLANSZY:
Punkt 1: Data plane: ERP / dokumenty. Punkt 2: Semantic plane: encje / reguły. Punkt 3: Model plane: retrieval / inference. Punkt 4: Control plane: auth / eval / logging.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 84: Koszt wdrożenia: TCO (3 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: WDROŻENIA: OD DEMO DO PRODUKCJI | SLAJD: 84 | CZAS: 3 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Na przykładzie asystenta ofertowego wypisz koszty, które znikają z marketingowej kalkulacji: etykietowanie, wydobycie dokumentów, review prawne, monitorowanie i integracje. Oszczędność tokenów nie zrównoważy złej jakości procesu.

ROZWINIĘCIE PLANSZY:
Punkt 1: Projekt / dane / integracje. Punkt 2: Inferencja i infrastruktura. Punkt 3: Ewaluacja i bezpieczeństwo. Punkt 4: Obsługa incydentów i zmian.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 85: ROI vs pozorna oszczędność (3 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: WDROŻENIA: OD DEMO DO PRODUKCJI | SLAJD: 85 | CZAS: 3 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Użyj prostego modelu hipotetycznego bez obiecywania konkretnych procentów. Jeśli 100 ofert miesięcznie trwa krócej, ale połowa wymaga dodatkowej kontroli, oszczędność może stopnieć. ROI to miernik projektu, nie reklama modelu.

ROZWINIĘCIE PLANSZY:
Punkt 1: Czas × koszt pracy. Punkt 2: Liczba poprawek. Punkt 3: Koszt błędu. Punkt 4: Efekt wdrożenia i adopcji.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 86: Zbiór testowy od początku (3 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: WDROŻENIA: OD DEMO DO PRODUKCJI | SLAJD: 86 | CZAS: 3 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Testy nie mogą być wyłącznie tymi przykładami, na których dostrajaliśmy prompt. Wyznacz osobny zestaw zadań, scenariusze krytyczne i progi akceptacji. Szczególną uwagę skieruj na przypadki rzadkie, ale kosztowne.

ROZWINIĘCIE PLANSZY:
Punkt 1: Happy path. Punkt 2: Edge cases. Punkt 3: Błędne dane i prompt injection. Punkt 4: Testy regresji po aktualizacji.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 87: MLOps / LLMOps: cykl życia (3 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: WDROŻENIA: OD DEMO DO PRODUKCJI | SLAJD: 87 | CZAS: 3 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Model to nie jednorazowy plik. Zmieniają się dokumenty, dostawcy, instrukcje i użytkownicy. Potrzebujemy procesu wydań podobnego do DevOps, z dodatkiem pomiaru zachowania modeli i ciągłości źródeł danych.

ROZWINIĘCIE PLANSZY:
Punkt 1: Versioning danych i promptów. Punkt 2: Evaluation / deployment gate. Punkt 3: Monitoring zmian. Punkt 4: Rollback lub wyłączenie.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 88: Ewaluacja offline i online (3 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: WDROŻENIA: OD DEMO DO PRODUKCJI | SLAJD: 88 | CZAS: 3 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Podkreśl etap shadow mode, w którym system proponuje decyzję, ale jeszcze jej nie wykonuje. Porównujemy wtedy propozycje z działaniami ludzi. Dopiero potem włączamy ograniczony ruch produkcyjny i jasne warunki wycofania.

ROZWINIĘCIE PLANSZY:
Punkt 1: Offline: testy na zbiorze. Punkt 2: Shadow mode: bez działań. Punkt 3: Canary: mały procent ruchu. Punkt 4: Online: skutki i feedback.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 89: Mierniki systemowe i SLO (3 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: WDROŻENIA: OD DEMO DO PRODUKCJI | SLAJD: 89 | CZAS: 3 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Nie pokazuj tylko accuracy. W asystencie klienta ważne jest, czy odpowiedź ma dowody i przychodzi w czasie akceptowalnym przez biznes. W agencie istotna jest liczba błędnych skutków i odsetek sytuacji skierowanych do człowieka.

ROZWINIĘCIE PLANSZY:
Punkt 1: P95 / P99 latency. Punkt 2: Availability. Punkt 3: Task success / groundedness. Punkt 4: Incidents and human overrides.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 90: Obserwowalność vs prywatność (3 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: WDROŻENIA: OD DEMO DO PRODUKCJI | SLAJD: 90 | CZAS: 3 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
W logach potrzebujemy dowodów działania, ale nie powinniśmy gromadzić kompletnej zawartości prywatnych dokumentów bez konieczności. Pokaż politykę minimalizacji i kontrolowania dostępu do telemetrii.

ROZWINIĘCIE PLANSZY:
Punkt 1: Trace ID, wersja systemu. Punkt 2: Minimalizacja danych. Punkt 3: Redakcja PII. Punkt 4: Role i retencja logów.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 91: Security red teaming (3 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: WDROŻENIA: OD DEMO DO PRODUKCJI | SLAJD: 91 | CZAS: 3 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Wyjaśnij różnicę pomiędzy atakiem na tekst a atakiem na operację. Przykładowo instrukcja w dokumencie każe asystentowi wysłać plik do nieautoryzowanej domeny. Zabezpieczenie musi działać na granicach uprawnień, a nie tylko w samym promptcie.

ROZWINIĘCIE PLANSZY:
Punkt 1: Prompt injection w dokumencie. Punkt 2: Eksfiltracja przez narzędzie. Punkt 3: Niewłaściwy zakres uprawnień. Punkt 4: Wywołanie API niezgodne z intencją.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 92: NIST AI RMF w praktyce (3 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: WDROŻENIA: OD DEMO DO PRODUKCJI | SLAJD: 92 | CZAS: 3 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
NIST to framework zarządzania ryzykiem, nie certyfikat jednego modelu. Przełóż cztery funkcje na projekt studencki: kto odpowiada, jaki jest kontekst, jak badamy błędy, co robimy, jeśli ryzyko przekracza próg.

ROZWINIĘCIE PLANSZY:
Punkt 1: GOVERN: role i zasady. Punkt 2: MAP: kontekst i ryzyka. Punkt 3: MEASURE: testy i dowody. Punkt 4: MANAGE: decyzje i reakcje.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

ŹRÓDŁO / KONTEKST: https://airc.nist.gov/airmf-resources/airmf/5-sec-core/

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 93: AI Act: oceniamy zastosowanie (3 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: WDROŻENIA: OD DEMO DO PRODUKCJI | SLAJD: 93 | CZAS: 3 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Przypomnij, że zakres obowiązków i kalendarz stosowania zależą od statusu systemu i roli organizacji. Na listopad 2026 harmonogram przejściowy jest rozbudowany; nie zastępuj analizy prawnej sloganem „wszystko obowiązuje od sierpnia”.

ROZWINIĘCIE PLANSZY:
Punkt 1: Rola: provider / deployer. Punkt 2: Przeznaczenie i kontekst. Punkt 3: Wymogi zależne od kategorii. Punkt 4: Aktualne terminy trzeba sprawdzać.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

ŹRÓDŁO / KONTEKST: https://ai-act-service-desk.ec.europa.eu/en/ai-act/eu-ai-act-implementation-timeline

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 94: Zarządzanie zmianą (3 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: WDROŻENIA: OD DEMO DO PRODUKCJI | SLAJD: 94 | CZAS: 3 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Wyjaśnij, że nawet perfekcyjny model nie tworzy automatycznie nowej praktyki organizacyjnej. Potrzebujemy zmiany odpowiedzialności, ergonomii procesu, szkolenia i mechanizmu feedbacku. Niech studenci nazwą opór wynikający z niejasnych ról, a nie tylko z „niechęci do AI”.

ROZWINIĘCIE PLANSZY:
Punkt 1: Właściciel procesu. Punkt 2: Szkolenie i kompetencje. Punkt 3: Praktyczna ścieżka eskalacji. Punkt 4: Adopcja mierzona w pracy.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 95: Model odpowiedzialności RACI (3 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: WDROŻENIA: OD DEMO DO PRODUKCJI | SLAJD: 95 | CZAS: 3 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Wpisz role w RACI dla wdrożenia agenta. Product owner nie może ukryć się za dostawcą, a administrator techniczny nie powinien sam definiować interpretacji faktur. Nazwanie odpowiedzialności jest formą architektury organizacji.

ROZWINIĘCIE PLANSZY:
Punkt 1: Responsible: wykonuje. Punkt 2: Accountable: odpowiada za rezultat. Punkt 3: Consulted: doradza. Punkt 4: Informed: otrzymuje informację.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 96: Pilotaż: decyzja GO / NO-GO (3 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: WDROŻENIA: OD DEMO DO PRODUKCJI | SLAJD: 96 | CZAS: 3 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Na zakończenie pilotażu nie pytaj tylko, czy uczestnikom podobał się chatbot. Pytaj o skuteczność, błędy krytyczne, prywatność, koszt na zadanie i możliwość audytu. Poważny system wymaga też planu wyłączenia.

ROZWINIĘCIE PLANSZY:
Punkt 1: Jakość ponad ustalonym progiem. Punkt 2: Brak krytycznych luk. Punkt 3: Koszt w budżecie. Punkt 4: Procedura eskalacji działa.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 97: LAB: karta wdrożenia w 12 minut (6 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: WDROŻENIA: OD DEMO DO PRODUKCJI | SLAJD: 97 | CZAS: 6 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Warsztat. Zespoły mają narysować system ofertowy: pliki PDF, cennik, CRM, LLM i człowiek. Każdy zapisuje kryteria stop, dwa ryzyka oraz właściciela decyzji. Liczba 30 jest demonstracyjną liczbą przypadków, nie standardem statystycznym.

ROZWINIĘCIE PLANSZY:
Punkt 1: Cel i miernik biznesowy. Punkt 2: Architektura danych i uprawnień. Punkt 3: PoC: testy na 30 przykładach (hipotetycznie). Punkt 4: Pilot: shadow mode + właściciel.

PROWADZENIE I PRZYKŁAD:
Praca z salą: najpierw przedstaw scenariusz i rozdziel role. Następnie daj grupom czas na zapisanie odpowiedzi na kartce, niech nie wybierają od razu narzędzia. Obejdź zespoły i pytaj o źródło danych, semantykę stanów, wyjątki oraz właściciela decyzji. Zaproś co najmniej dwa zespoły do przedstawienia odmiennego rozwiązania; omów kontrargumenty i podsumuj warunki zatrzymania wdrożenia. 

PYTANIE DO SALI: Jaki błąd zatrzyma pilotaż, nawet jeśli średnia jakość będzie bardzo dobra?
Omów co najmniej dwie możliwe odpowiedzi, wskazując ich warunki i konsekwencje.

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


## MODUŁ 6: STUDIA PRZYPADKÓW: Z SYSTEMEM W ŚWIECIE (50 minut)

**Slajd otwierający (2 min)**: wprowadź pytanie przewodnie.


### SLAJD 99: Case 1: analityka i decyzje (4 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: STUDIA PRZYPADKÓW: Z SYSTEMEM W ŚWIECIE | SLAJD: 99 | CZAS: 4 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Przedstaw hipotetyczny system prognozujący popyt. Samej prognozy nie należy mylić z optymalną decyzją cenową. Wymagane są ograniczenia biznesowe, doświadczenie zespołu i mechanizm obserwacji zmian.

ROZWINIĘCIE PLANSZY:
Punkt 1: Źródła: sezonowość, kalendarz, sprzedaż. Punkt 2: Model: prognoza szeregów. Punkt 3: Decyzja: obsada i ceny. Punkt 4: Miara: błąd + koszt decyzji.

PROWADZENIE I PRZYKŁAD:
Prowadzenie studium przypadku: nazwij aktorów, źródła danych, możliwe decyzje i koszt błędu. Wskaż konkretny moment, w którym interpretacja modelu może stać się operacją systemową. Poproś o alternatywną architekturę opartą na regułach lub prostszym modelu. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 100: Case 2: repozytorium dokumentów (4 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: STUDIA PRZYPADKÓW: Z SYSTEMEM W ŚWIECIE | SLAJD: 100 | CZAS: 4 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
To studium przypadku oparte na typowym wyzwaniu firm z archiwum PDF, bez ujawniania poufnych danych. Samo zindeksowanie 15 lat plików nie daje wiarygodnego cennika na dziś. Kluczowe stają się daty obowiązywania i status oferty.

ROZWINIĘCIE PLANSZY:
Punkt 1: OCR i ekstrakcja tabel. Punkt 2: Metadane: data, produkt, klient. Punkt 3: RAG i wyszukiwanie hybrydowe. Punkt 4: Kontrola aktualności i poufności.

PROWADZENIE I PRZYKŁAD:
Prowadzenie studium przypadku: nazwij aktorów, źródła danych, możliwe decyzje i koszt błędu. Wskaż konkretny moment, w którym interpretacja modelu może stać się operacją systemową. Poproś o alternatywną architekturę opartą na regułach lub prostszym modelu. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 101: Case 3: ofertowanie techniczne (4 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: STUDIA PRZYPADKÓW: Z SYSTEMEM W ŚWIECIE | SLAJD: 101 | CZAS: 4 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Pokaż ofertowanie instalacji. Wyliczenie kwoty powinno opierać się na jawnych tabelach, jednostkach i regułach, a nie wolnej generacji języka. Model może prowadzić rozmowę i rozpoznać brak danych, ale rachunek i zatwierdzenie muszą być kontrolowane.

ROZWINIĘCIE PLANSZY:
Punkt 1: Baza parametrów i cen. Punkt 2: Reguły technologiczne. Punkt 3: LLM porządkuje wymagania. Punkt 4: Człowiek akceptuje wycenę.

PROWADZENIE I PRZYKŁAD:
Prowadzenie studium przypadku: nazwij aktorów, źródła danych, możliwe decyzje i koszt błędu. Wskaż konkretny moment, w którym interpretacja modelu może stać się operacją systemową. Poproś o alternatywną architekturę opartą na regułach lub prostszym modelu. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 102: Case 4: monitoring i IoT (4 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: STUDIA PRZYPADKÓW: Z SYSTEMEM W ŚWIECIE | SLAJD: 102 | CZAS: 4 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Przykład hipotetyczny z flotą urządzeń. Sygnał anomalii nie powinien automatycznie zamieniać się w kosztowną akcję bez oceny fałszywych alarmów. Pokazuje to praktyczne spotkanie Big Data, modeli i kontraktów działania.

ROZWINIĘCIE PLANSZY:
Punkt 1: Czujniki → broker. Punkt 2: Windowing i anomalie. Punkt 3: Alert → diagnoza. Punkt 4: Akcja serwisowa z potwierdzeniem.

PROWADZENIE I PRZYKŁAD:
Prowadzenie studium przypadku: nazwij aktorów, źródła danych, możliwe decyzje i koszt błędu. Wskaż konkretny moment, w którym interpretacja modelu może stać się operacją systemową. Poproś o alternatywną architekturę opartą na regułach lub prostszym modelu. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 103: Case 5: agent badań naukowych (3 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: STUDIA PRZYPADKÓW: Z SYSTEMEM W ŚWIECIE | SLAJD: 103 | CZAS: 3 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Dla uczestników SWPS to przykład szczególnie istotny. Asystent może pomóc w mapowaniu literatury, ale nie może wymyślać badań ani zastępować metodologicznej oceny. Ustal politykę cytatów i filtrowania dokumentów.

ROZWINIĘCIE PLANSZY:
Punkt 1: Repozytorium publikacji. Punkt 2: Cyfrowa tożsamość cytatów. Punkt 3: Streszczenie z dowodami. Punkt 4: Nie fabrykuj wyników naukowych.

PROWADZENIE I PRZYKŁAD:
Prowadzenie studium przypadku: nazwij aktorów, źródła danych, możliwe decyzje i koszt błędu. Wskaż konkretny moment, w którym interpretacja modelu może stać się operacją systemową. Poproś o alternatywną architekturę opartą na regułach lub prostszym modelu. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 104: Case 6: AlphaFold jako infrastruktura badań (3 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: STUDIA PRZYPADKÓW: Z SYSTEMEM W ŚWIECIE | SLAJD: 104 | CZAS: 3 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
AlphaFold ilustruje zmianę skali w badaniach dzięki modelom oraz dystrybucji wyników. Współczesna baza zawiera ponad 200 milionów przewidywanych struktur. Nie interpretuj tego jako 200 milionów potwierdzonych obserwacji laboratoryjnych.

ROZWINIĘCIE PLANSZY:
Punkt 1: Predykcja struktur białkowych. Punkt 2: Baza publicznych przewidywań. Punkt 3: Dostęp dla środowiska badawczego. Punkt 4: Predykcja nie zastępuje walidacji eksperymentalnej.

PROWADZENIE I PRZYKŁAD:
Prowadzenie studium przypadku: nazwij aktorów, źródła danych, możliwe decyzje i koszt błędu. Wskaż konkretny moment, w którym interpretacja modelu może stać się operacją systemową. Poproś o alternatywną architekturę opartą na regułach lub prostszym modelu. 

ŹRÓDŁO / KONTEKST: https://alphafold.ebi.ac.uk/

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 105: Case 7: dane publiczne (3 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: STUDIA PRZYPADKÓW: Z SYSTEMEM W ŚWIECIE | SLAJD: 105 | CZAS: 3 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Użyj przykładu automatycznej segmentacji zgłoszeń. Nawet model wykazujący wysoką trafność może mieć nierówną jakość dla różnych grup. Ważne są kontekst, człowiek i proces naprawy skutków.

ROZWINIĘCIE PLANSZY:
Punkt 1: Cel i podstawa przetwarzania. Punkt 2: Transparentność modelu. Punkt 3: Test wpływu na grupy. Punkt 4: Prawo do kontroli i korekty.

PROWADZENIE I PRZYKŁAD:
Prowadzenie studium przypadku: nazwij aktorów, źródła danych, możliwe decyzje i koszt błędu. Wskaż konkretny moment, w którym interpretacja modelu może stać się operacją systemową. Poproś o alternatywną architekturę opartą na regułach lub prostszym modelu. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 106: Case 8: graf + RAG + decyzja (3 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: STUDIA PRZYPADKÓW: Z SYSTEMEM W ŚWIECIE | SLAJD: 106 | CZAS: 3 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Zestaw wszystkie koncepcje w jednym miejscu. Dokument może potwierdzać treść deklaracji, graf pokazuje, którego zobowiązania dotyczy, a ERP rozstrzyga status wpłaty. Dopiero potem system może proponować działanie, nie odwrotnie.

ROZWINIĘCIE PLANSZY:
Punkt 1: PDF: dowód w tekście. Punkt 2: Graf: relacje i tożsamość. Punkt 3: ERP: stan transakcyjny. Punkt 4: Agent: decyzja w ramach kontraktu.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 107: Benchmark wdrożeń: co porównywać? (3 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: STUDIA PRZYPADKÓW: Z SYSTEMEM W ŚWIECIE | SLAJD: 107 | CZAS: 3 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Wyobraź sobie porównanie trzech dostawców. Najlepszy model na publicznym benchmarku może być droższy, mniej stabilny lub gorzej integrować się z danymi. Organizacja kupuje rezultat procesu, nie rekord w rankingu.

ROZWINIĘCIE PLANSZY:
Punkt 1: Jakość konkretnego procesu. Punkt 2: Opóźnienie i dostępność. Punkt 3: Koszt całkowity. Punkt 4: Ślad dowodowy i kontrola.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 108: Pokusa AGI vs realne zadania (3 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: STUDIA PRZYPADKÓW: Z SYSTEMEM W ŚWIECIE | SLAJD: 108 | CZAS: 3 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Rozdziel pytania o przyszłe zdolności od obecnej praktyki wdrożeń. Nawet jeśli system stanie się bardziej autonomiczny, nadal będzie potrzebował rozstrzygnięcia tożsamości faktury, daty obowiązywania i prawa do operacji.

ROZWINIĘCIE PLANSZY:
Punkt 1: Możliwości modeli rosną. Punkt 2: Ontologie nadal są potrzebne. Punkt 3: Dane nadal mogą być błędne. Punkt 4: Odpowiedzialność nie znika.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 109: Kompletna architektura 2026 (3 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: STUDIA PRZYPADKÓW: Z SYSTEMEM W ŚWIECIE | SLAJD: 109 | CZAS: 3 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
To syntetyczny model architektury. Nie stanowi standardu formalnego, lecz porządkuje główne funkcje. Każdy komponent można rozwijać niezależnie, a między warstwami definiować kontrakty. W ten sposób unikamy monolitu i niejasnego miejsca odpowiedzialności.

ROZWINIĘCIE PLANSZY:
Punkt 1: Zdarzenie i źródło. Punkt 2: Wiedza i ontologia. Punkt 3: Model i narzędzia. Punkt 4: Polityka / monitoring / audit.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 110: FINAŁOWY LAB: rada wdrożeniowa (5 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: STUDIA PRZYPADKÓW: Z SYSTEMEM W ŚWIECIE | SLAJD: 110 | CZAS: 5 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Dziesięć minut pracy grupowej. Każda grupa ma narysować pipeline danych, minimalną ontologię i warunki akceptacji. Podczas omówienia poproś o jedno ryzyko systemowe, którego nie naprawi lepszy prompt. To sprawdzenie całości materiału.

ROZWINIĘCIE PLANSZY:
Punkt 1: Problem: firma chce autonomicznie zamykać sprawy. Punkt 2: Zaprojektuj źródła i ontologię. Punkt 3: Zaproponuj model i trzy testy. Punkt 4: Wskaż moment wymagający człowieka.

PROWADZENIE I PRZYKŁAD:
Praca z salą: najpierw przedstaw scenariusz i rozdziel role. Następnie daj grupom czas na zapisanie odpowiedzi na kartce, niech nie wybierają od razu narzędzia. Obejdź zespoły i pytaj o źródło danych, semantykę stanów, wyjątki oraz właściciela decyzji. Zaproś co najmniej dwa zespoły do przedstawienia odmiennego rozwiązania; omów kontrargumenty i podsumuj warunki zatrzymania wdrożenia. 

PYTANIE DO SALI: Co jest ważniejsze: 99% trafności czy brak nieodwracalnej pomyłki?
Omów co najmniej dwie możliwe odpowiedzi, wskazując ich warunki i konsekwencje.

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 111: Dwanaście pytań do każdej AI (3 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: STUDIA PRZYPADKÓW: Z SYSTEMEM W ŚWIECIE | SLAJD: 111 | CZAS: 3 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Zadaj te pytania w szybkim rytmie. Czy jest dobry baseline? Czy dane są aktualne? Kto jest właścicielem procesu? Co znaczy sukces? Jakie są wyjątki? Czy można przerwać i odtworzyć działanie? Ten zestaw pytań ma zostać studentom na późniejsze projekty.

ROZWINIĘCIE PLANSZY:
Punkt 1: Jaki problem i jaka decyzja?. Punkt 2: Skąd dowód, jaka tożsamość?. Punkt 3: Jakie ryzyko i ograniczenia?. Punkt 4: Kto zatwierdza i jak weryfikujemy skutek?.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


### SLAJD 112: Teza na drogę (3 min)

NOTATKI PRELEGENTA • CZĘŚĆ II / SWPS 2026–2027
MODUŁ: STUDIA PRZYPADKÓW: Z SYSTEMEM W ŚWIECIE | SLAJD: 112 | CZAS: 3 min (wliczony w plan 6 h 15 min)

TEKST DO WYGŁOSZENIA:
Zamknij odwołaniem do pierwszej prezentacji „Poza modelem” i wykładu w Warszawie. Model może być spektakularny, ale organizacja odpowiada za to, jaki świat został mu powierzony, jakie działania może wykonać i jak sprawdzimy rzeczywisty skutek.

ROZWINIĘCIE PLANSZY:
Punkt 1: MODEL: zdolność. Punkt 2: DANE: dowód. Punkt 3: ONTOLOGIA: znaczenie. Punkt 4: ODPOWIEDZIALNOŚĆ: granica.

PROWADZENIE I PRZYKŁAD:
Prowadzenie: wskaż na wizualizacji kolejne elementy od lewej do prawej albo od centrum ku krawędzi. Przy każdym elemencie opowiedz, jak można go przetestować oraz co stanie się, gdy zadziała błędnie. Utrzymuj rozróżnienie między zdolnością modelu, stanem danych, interpretacją i działaniem organizacji. 

PRZEJŚCIE: Dopiero po ustaleniu ograniczeń i dowodów przejdź do następnego slajdu. Dodatkowe 30–60 sekund możesz wykorzystać na pytanie kontrolne, tak by zachować rozkład czasowy całego wykładu.


## ŹRÓDŁA

- W3C OWL 2: https://www.w3.org/TR/owl-overview/
- W3C RDF 1.1: https://www.w3.org/TR/rdf11-concepts/
- W3C SHACL: https://www.w3.org/TR/shacl/
- W3C PROV-O: https://www.w3.org/TR/prov-o/
- Apache Kafka: https://kafka.apache.org/documentation.html
- Apache Spark Streaming: https://spark.apache.org/docs/latest/streaming/index.html
- Apache Iceberg: https://iceberg.apache.org/spec/
- NIST AI RMF: https://airc.nist.gov/airmf-resources/airmf/5-sec-core/
- AI Act Service Desk: https://ai-act-service-desk.ec.europa.eu/en/ai-act/eu-ai-act-implementation-timeline
- EMBL-EBI AlphaFold: https://alphafold.ebi.ac.uk/
- Vaswani et al. 2017: https://arxiv.org/abs/1706.03762
- Marcin Albiniak: System, który wszedł do świata: Wystąpienie konferencyjne, Warszawa, 19 listopada 2026