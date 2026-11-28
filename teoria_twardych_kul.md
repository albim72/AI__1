# Teoria twardych kul
### Prezentacja dla studentów · 8 slajdów + notatki prowadzącego

> Format każdego slajdu: **NA SLAJDZIE** (to, co widzą studenci) i **DLA CIEBIE** (co mówić, puenty, pytania do sali).
> Czas: ok. 20–25 min.

---

## Slajd 1 · Najprostszy model materii, jaki da się pomyśleć

**NA SLAJDZIE**
- Cząsteczka = **twarda, idealnie sprężysta kula** o średnicy *d*
- Potencjał oddziaływania:

  $$U(r) = \begin{cases} \infty & r < d \\ 0 & r \ge d \end{cases}$$

- Nie ma przyciągania ani miękkiego odpychania. Jest tylko **zakaz przenikania**.
- Pytanie przewodnie: *ile fizyki da się wyciągnąć z samej geometrii?*

**DLA CIEBIE**
- Zacznij od prowokacji: „To model tak głupi, że powinien nic nie przewidywać. A przewiduje gazy, ciecze, krystalizację i dał początek symulacjom komputerowym.”
- Podkreśl, że w tym modelu **nie ma energii potencjalnej** poza nieskończoną ścianą. Wszystko, co się dzieje, wynika z **entropii i geometrii**. To jest główna myśl całego wykładu i warto do niej wrócić na końcu.
- Analogia dla sali: kule bilardowe na stole bez tarcia.

---

## Slajd 2 · Gaz twardych kul: zderzenia i droga swobodna

**NA SLAJDZIE**
- **Przekrój czynny** na zderzenie: $\sigma = \pi d^2$
- **Średnia droga swobodna**:

  $$\lambda = \frac{1}{\sqrt{2}\, n\, \sigma} = \frac{k_B T}{\sqrt{2}\, \pi d^2\, p}$$

- **Częstość zderzeń**: $z = \sqrt{2}\, n \sigma \langle v \rangle$, gdzie $\langle v \rangle = \sqrt{8 k_B T / \pi m}$
- Przykład: powietrze w warunkach normalnych → λ ≈ 70 nm, około **5 mld zderzeń na sekundę** na cząsteczkę

**DLA CIEBIE**
- Wyprowadź σ obrazowo: kula o średnicy *d* „zamiata” walec o promieniu *d*, bo dwie kule zderzają się, gdy ich środki zbliżą się na odległość *d*, a nie *d/2*. To częsty błąd studentów.
- Skąd √2: liczy się **prędkość względna** cząsteczek, a nie prędkość jednej z nich. Średnia prędkość względna jest √2 razy większa.
- Na tej podstawie Maxwell i Boltzmann policzyli **lepkość, przewodnictwo cieplne i dyfuzję** gazów. Zaskoczenie Maxwella: lepkość gazu **nie zależy od ciśnienia**. Eksperyment to potwierdził i był to jeden z pierwszych mocnych dowodów na istnienie cząsteczek.

---

## Slajd 3 · Równanie stanu: gdy kule zajmują miejsce

**NA SLAJDZIE**
- Gaz doskonały: $pV = Nk_BT$. Cząsteczki są punktami.
- Kule mają **objętość własną** i odbierają sobie przestrzeń.
- Kluczowy parametr to **ułamek upakowania**:

  $$\eta = \frac{\pi}{6}\, n\, d^3$$

- Równanie **Carnahana–Starlinga** (1969):

  $$Z = \frac{pV}{Nk_BT} = \frac{1 + \eta + \eta^2 - \eta^3}{(1-\eta)^3}$$

**DLA CIEBIE**
- Pokaż, że przy η → 0 wraca gaz doskonały (Z → 1).
- Człon odpychający w **równaniu van der Waalsa** (*V − Nb*) to właśnie twarde kule w najprostszym przybliżeniu. Van der Waals = twarde kule + słabe przyciąganie.
- Carnahan–Starling to w połowie zgadywanka: autorzy zauważyli, że współczynniki wirialne są bliskie liczbom całkowitym, i zsumowali szereg. Działa świetnie dla fazy ciekłej. Dobra lekcja: **dobra heurystyka bywa warta więcej niż ścisłe wyprowadzenie**.

---

## Slajd 4 · Upakowanie: od Keplera do losowego stosu

**NA SLAJDZIE**
| Układ | Ułamek upakowania η |
|---|---|
| Kryształ fcc / hcp (najgęstszy możliwy) | **0,7405** (π/√18) |
| Losowe ścisłe upakowanie (RCP) | **≈ 0,64** |
| Krystalizacja płynu twardych kul | **0,494 → 0,545** |

- **Hipoteza Keplera** (1611): nie da się upakować kul gęściej niż w fcc
- Udowodniona przez **Thomasa Halesa** (1998), z formalną weryfikacją komputerową ukończoną w 2014 roku

**DLA CIEBIE**
- Kepler pisał o kulach armatnich. Pytanie zadał mu Thomas Harriot w imieniu Waltera Raleigha.
- Dowód Halesa wymagał tylu obliczeń komputerowych, że recenzenci nie byli w stanie go w pełni sprawdzić. Stąd projekt **Flyspeck**: formalny dowód w asystentach dowodzenia. To świetny most do AI, bo maszyna weryfikuje matematykę.
- Eksperyment na sali: słoik ziaren albo kulek. Potrząsanie zwiększa gęstość, ale nigdy do 0,74. Losowość ma swój sufit (≈ 0,64).

---

## Slajd 5 · Paradoks: entropia buduje porządek

**NA SLAJDZIE**
- Przy η ≈ 0,494 płyn twardych kul **krystalizuje**
- W modelu **nie ma przyciągania**, więc kryształ nie powstaje, bo „kule się lubią”
- Kryształ ma **większą entropię** niż zatłoczony płyn
- Kluczowe pojęcie: **objętość swobodna**. W uporządkowanej sieci każda kula ma więcej miejsca na drgania.

**DLA CIEBIE**
- To najważniejszy slajd koncepcyjnie. Intuicja studentów mówi „porządek = mniej entropii”. Tu jest odwrotnie. Gdy jest bardzo ciasno, uporządkowanie **zwalnia miejsce**, a ruch lokalny zyskuje więcej entropii, niż traci się na porządku globalnym.
- Analogia: zatłoczony parking. Auta ustawione w rzędach mają więcej swobody manewru niż auta porzucone byle jak.
- W latach 50. wielu fizyków nie wierzyło, że sama geometria wystarczy do przejścia fazowego. Rozstrzygnął to komputer, co prowadzi do następnego slajdu.

---

## Slajd 6 · Narodziny symulacji komputerowej

**NA SLAJDZIE**
- **1953, Metropolis, Rosenbluth, Rosenbluth, Teller, Teller**: pierwsza symulacja Monte Carlo cieczy na komputerze MANIAC w Los Alamos. Układem były **twarde dyski** (2D).
  → narodziny **algorytmu Metropolisa** (MCMC)
- **1957, Alder i Wainwright**: pierwsza **dynamika molekularna**, czyli twarde kule zderzające się zgodnie z prawami Newtona
  → komputerowy dowód **przejścia fazowego** płyn–kryształ

**DLA CIEBIE**
- To moment dla studentów AI: **algorytm Metropolisa powstał na twardych kulach**. Ten sam pomysł (próbkowanie z rozkładu przez łańcuch Markowa) siedzi dziś w statystyce bayesowskiej, simulated annealing i modelach generatywnych.
- Twarde kule były idealne dla ówczesnych komputerów: nie trzeba liczyć sił. Wystarczy wykryć zderzenie i odbić kule, co jest tanie obliczeniowo.
- Puenta: **najprostszy model fizyczny stał się poligonem, na którym urodziła się nauka obliczeniowa.** Model był za prosty, żeby był prawdziwy, i dlatego był wystarczająco prosty, żeby go policzyć.

---

## Slajd 7 · Twarde kule w chemii: teoria zderzeń

**NA SLAJDZIE**
- Reakcja A + B zachodzi tylko przy **zderzeniu** o wystarczającej energii
- Stała szybkości:

  $$k = P \cdot \sigma_{AB} \sqrt{\frac{8 k_B T}{\pi \mu}} \; e^{-E_a / k_B T}$$

- σ_AB to przekrój czynny twardych kul, μ to masa zredukowana
- **P** to **czynnik steryczny**: ułamek zderzeń z „dobrą” orientacją

**DLA CIEBIE**
- Pokaż, skąd bierze się postać równania **Arrheniusa**: częstość zderzeń × ułamek zderzeń z energią > Eₐ.
- Czynnik steryczny P to uczciwe przyznanie się, że cząsteczki **nie są kulami**. P bywa rzędu 10⁻⁶ dla złożonych cząsteczek. Dobry moment na wskazanie granic modelu.
- Dalsze rozwinięcie to **teoria stanu przejściowego** (Eyring), która zastępuje „zderzenie kul” powierzchnią energii potencjalnej.

---

## Slajd 8 · Czego uczy nas model, który jest „fałszywy”?

**NA SLAJDZIE**
- Twardych kul **nie ma** w przyrodzie, a mimo to model przewiduje:
  - lepkość i dyfuzję gazów
  - strukturę cieczy i krystalizację
  - realne układy, czyli **koloidy** (cząstki PMMA w cieczy zachowują się prawie jak twarde kule)
- Zasada: **dobry model to nie kopia rzeczywistości, tylko jej najmniejszy szkielet, który jeszcze działa**

> *„Wszystkie modele są błędne, ale niektóre są użyteczne.”* (G. E. P. Box)

**DLA CIEBIE**
- Koloidy domykają historię. Od lat 80. (Pusey i van Megen) krystalizację twardych kul **widać pod mikroskopem**, bo cząstki koloidalne są wystarczająco duże. Model z tablicy stał się eksperymentem.
- Most do AI (jeśli to grupa AI): sieć neuronowa też jest „fałszywym” modelem mózgu, a działa. Pytanie do sali: *jaki jest najmniejszy szkielet inteligencji, który jeszcze działa?*
- Wróć do slajdu 1: zero energii, sama geometria, a wychodzi z tego termodynamika. Zakończ zdaniem: **„Porządek nie zawsze wymaga siły. Czasem wystarczy brak miejsca.”**

---

### Pytania kontrolne dla studentów (opcjonalnie, na koniec)
1. Dlaczego przekrój czynny to πd², a nie π(d/2)²?
2. Jak zmieni się średnia droga swobodna, gdy dwukrotnie zwiększymy ciśnienie w stałej temperaturze?
3. Dlaczego kryształ twardych kul może mieć większą entropię niż płyn o tej samej gęstości?
4. Jaki związek ma algorytm Metropolisa z twardymi dyskami?
