# Wyniki uruchomionych rozwiązań

## 01_sprzedaz
Wiersze: 724 unikalne pozycje: 720
duplikat_pozycji    4
bledna_data         1
bledna_ilosc        0
bledna_cena         1
bledny_rabat        1
niespojna_kwota     3
niespojny_koszt     0
Wiersze z co najmniej jednym problemem: 8
Analiza: 716 kwarantanna: 8
line_id    order_date  discount  unit_price   net
  L0010 data_nieznana      0.35         400 520.0
  L0020    2025-11-08      1.50         600 780.0
  L0030    2025-05-13      0.20          -1 768.0
  L0040    2025-10-28      0.00         600 617.0
  L0001    2025-10-18      0.20         600 960.0
  L0002    2025-10-06      0.20         240 768.0
  L0003    2025-08-03      0.10         150 675.0
  L0004    2025-12-17      0.05         240 912.0
        net_recalc       margin
count   716.000000   716.000000
mean   1128.063547   505.088687
std     995.629014   928.412039
min      65.000000 -1520.000000
25%     384.000000   -30.000000
50%     780.000000   294.000000
75%    1569.000000   900.000000
max    4800.000000  4320.000000
         positions       net   margin
product                              
A              147  172627.5  85877.5
D              150  172251.5  80441.5
E              154  171329.5  74389.5
C              145  169012.5  73672.5
B              120  122472.5  47262.5
            net_recalc   margin
order_date                     
2025-01        58670.0  18130.0
2025-02        56206.5  26286.5
2025-03        77149.0  31909.0
2025-04        67346.5  34186.5
2025-05        63288.5  29398.5
2025-06        53388.0  24788.0
2025-07        64078.0  29748.0
2025-08        70963.0  39403.0
2025-09        58949.0  24069.0
2025-10        67020.0  26500.0
2025-11        93892.0  46692.0
2025-12        76743.0  30533.0
Do wyjaśnienia, dystans <=0: record_id vehicle_id  distance_km  fuel_liters
     F004        V04            0        37.28
Średnia tras: 8.195984878866648 L/100 km; wskaźnik łączny: 8.191704820899544 L/100 km
Zero paliwa: record_id vehicle_id  distance_km  fuel_liters  l_per_100km
     F076        V04          631          0.0          0.0
Wysokie odczyty, do wyjaśnienia: Empty DataFrame
Columns: [record_id, vehicle_id, distance_km, fuel_liters, l_per_100km]
Index: []

## 02_csv
 id                   nazwa  ilość sztuk  cena netto    kolor   miasto  województwo              kategoria  wartość netto
  1      Klawiatura biurowa           16       33.86   czarny Warszawa  mazowieckie  Peryferia komputerowe         541.76
  2 Karta graficzna premium            8    11255.19  zielony  Wrocław dolnośląskie Podzespoły komputerowe       90041.52
  3        Zmywarka premium            6     3814.99 czerwony   Krosno podkarpackie               Duże AGD       22889.94
  4        Smartfon flagowy           12     5694.06     inne   Zamość    lubelskie     Urządzenia mobilne       68328.72
  5        Soundbar premium            4     4525.89    żółty    Brzeg     opolskie            Audio i RTV       18103.56
id                 int64
nazwa             object
ilość sztuk        int64
cena netto       float64
kolor             object
miasto            object
województwo       object
kategoria         object
wartość netto    float64
dtype: object
Średnia ceny w PRÓBCE: 3124.328022
{'rows': 100000, 'units': 1804250, 'net_cents': 558013808069, 'price_cents_sum': 30950504596, 'mean_unit_price_pln': 3095.0504596, 'quantity_weighted_price_pln': 3092.774327665235}
                              n   units     net_cents
Akcesoria elektroniczne    9338  168054    1684524485
Audio i RTV               12767  229698  113539620664
Duże AGD                  16698  299916  121884821579
Komputery i monitory      10914  197772  167768942662
Małe AGD                  22299  405496   61387314987
Peryferia komputerowe      7372  133255    4399866753
Podzespoły elektroniczne   1948   34868      15970446
Podzespoły komputerowe     3699   66618   29123484557
Sieci komputerowe          3732   67670    8404436481
Urządzenia mobilne        11233  200903   49804825455
Rozmiary partii: [17003, 17003, 17003, 17003, 17003, 14985]
Średnia średnich: 3095.0794048814446 poprawna średnia pozycji: 3095.0504596
Cena ważona sztukami: 3092.774327665235
Kontrola sum pełnego odczytu i partii: OK

## 03_przygotowanie
(3000, 9) {'age': 120, 'income': 150, 'amount': 0, 'past_chargebacks': 0, 'device_type': 0}
Train: 2400 test: 600
Próg z train: 1953.4289000000313 macierze: (2400, 7) (600, 7)
Transform nie uczy parametrów z testu. Nieznana kategoria obsłużona: (600, 7)
