# Sposób poprowadzenia przykładów

## 01. Sprzedaż i paliwo

„To są moje pliki dydaktyczne z wcześniejszego repozytorium. Najpierw ustalamy, co oznacza wiersz. line_id identyfikuje pozycję, więc z samej jego liczby nie policzymy liczby zamówień. Oryginał ma 720 pozycji. Na potrzeby tego ćwiczenia dodałem do kopii cztery powtórzenia i cztery zmiany. Chcę, żebyście wykryli je regułami i umieli powiedzieć, co stało się z populacją po wykluczeniu.”

„Nie zakładajcie, że ujemna marża jest błędem technicznym. Może być prawidłowo policzonym niekorzystnym wynikiem. Pokażcie dowód, a nie samą ocenę.”

„W paliwie jeden rekord ma zerowy dystans. Wskaźnik litrów na sto kilometrów jest wtedy niezdefiniowany. Pokażcie go osobno. Potem porównajcie średnią wyników tras z ilorazem sum. Oba rachunki odpowiadają innym wagom. Nie usuwajcie wysokich odczytów tylko dlatego, że są niewygodne.”

Klucz: 724 wejściowe pozycje, 720 unikalnych line_id, 8 wierszy oznaczonych (4 kopie oraz 4 zmienione rekordy), 716 w analizie według zadanej reguły. Liczby flag mogą się nakładać. W paliwie 120 rekordów, z nich 119 z dodatnim dystansem. Dokładne kwoty i wskaźniki: WYNIKI_I_KLUCZ.md.

## 02. Duży CSV

„To kontynuacja mojego generatora pięciu milionów rekordów. Dziś dostajecie mniejszy, gotowy plik. Nie będziemy czekać na generowanie setek megabajtów. Zasada pozostaje ta sama: czytamy partię, aktualizujemy stan, przechodzimy dalej. Ostatnia partia ma inną liczebność. Jeśli uśrednicie średnie partii bez wag, zmienicie wynik.”

„Kwoty w tym zbiorze przechowujemy w całkowitych groszach. Osobno policzymy zwykłą średnią cen pozycji oraz cenę ważoną sztukami. Średnia partii, średnia pozycji i średnia ważona ilością wymagają różnych mianowników.”

„Próbka pięciu tysięcy wierszy opisuje dokładnie tę próbkę. Sumę całego pliku policzymy, przechodząc przez cały plik. Samo nrows nie jest analizą wszystkich danych.”

Pełny wariant 5 mln uruchom po zajęciach przez --n 5000000. Oryginalny analizator znajduje się w narzedzia. Ma pełniejszą walidację, dokładne kwantyle i pamięć zależną również od bitmapy ID i histogramu cen. Krótsza funkcja dydaktyczna ma mniejszy zakres kontroli.

## 03. Dane do modelu

„Ten fragment pochodzi z mojego pipeline transakcji. Skupimy się na danych, bez trenowania lasu losowego. Wcześniejszy kod wyznaczał próg kwoty na całym df, jeszcze przed podziałem. Tutaj próg jest częścią fit na treningu. Nowe dane przechodzą tylko przez transform.”

„Moment decyzji ma znaczenie. Przy autoryzacji transakcji znamy jej bieżącą kwotę. Przy wejściu do sklepu nie znamy jeszcze końcowej kwoty zakupów. Ta sama nazwa kolumny może być dopuszczalna w jednym zadaniu i niedopuszczalna w drugim. Późniejszy zwrot jest wyłączony z cech.”

„Zmienimy test na skrajny i sprawdzimy, czy próg oraz mediany pozostały niezmienione. Nie oceniamy tu skuteczności modelu. Sprawdzamy poprawność procedury przygotowania danych.”

## Kryteria odpowiedzi

Jednostka i mianowniki 2 pkt, kontrola jakości z jawną regułą 2 pkt, agregacje i zgodność partii z kontrolą 3 pkt, granice interpretacji i dostępność cech 2 pkt, czytelny wniosek 1 pkt. To proponowana ocena ćwiczenia, nie zmiana formalnego regulaminu zaliczenia.
