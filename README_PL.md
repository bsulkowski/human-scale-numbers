# HSN — Human Scale Numbers

*Also available in English: [README](README.md)*

Mały zestaw okrągłych liczb, który pokrywa cały zakres codziennych pomiarów — i pasuje do siebie tak, że możesz skalować cokolwiek bez przeliczania.

Zamiast "trochę więcej" bierzesz następną wartość z ciągu. Zamiast mnożyć przez 1,6 — przesuwasz każdą wartość o tę samą liczbę kroków. Liczby są dobrane tak, żeby je łatwo zapamiętać, a kroki — żeby różnice między nimi miały znaczenie.

HSN działa wszędzie tam, gdzie mierzysz, eksperymentujesz lub skalujesz: gotowanie, trening, finanse, czas, modelowanie 3D, projektowanie gier i nie tylko.

## Ciąg

| Krok | Wartość |
|------|---------|
| 0 | 1 |
| 1 | 1,25 |
| 2 | 1,6 |
| 3 | 2 |
| 4 | 2,5 |
| 5 | 3,2 |
| 6 | 4 |
| 7 | 5 |
| 8 | 6,4 |
| 9 | 8 |
| 10 | 10 |

Dalej: 12,5 — 16 — 20 — 25 — 32 — 40 — 50 — 64 — 80 — 100 …

## Skalowanie bez przeliczania

Ponieważ ciąg jest geometryczny, typowe mnożenia stają się prostymi przesunięciami o kroki:

| Operacja | Kroki |
|----------|-------|
| ×2 (lub ÷2) | +3 (lub −3) |
| ×3 (lub ÷3) | +5 (lub −5) — w przybliżeniu |
| ×10 (lub ÷10) | +10 (lub −10) |

Żeby podwoić dowolną wartość, przesuń ją o 3 kroki w górę. Żeby zmniejszyć trzykrotnie — przesuń o 5 kroków w dół. Ta sama logika działa w różnych dziedzinach:

- **Gotowanie** — przeskaluj przepis dla jednej osoby lub całej rodziny
- **Trening** — zwiększaj dystans biegu: 3,2 → 4 → 5 km
- **Finanse** — ustalaj kieszonkowe, które rośnie sensownie wraz z wiekiem
- **Czas** — dobieraj czasy gotowania lub parzenia z wariantu czasowego
- **Modelowanie 3D** — wybieraj wymiary, które wzajemnie do siebie pasują
- **Projektowanie gier** — buduj skale liczbowe dla mechanik (np. wskaźnik siły)

## Wariant czasowy

Dla czasu ciąg jest dostosowany do godzin i minut:

| Krok | Wartość |
|------|---------|
| 0 | 1:00 |
| 1 | 1:15 |
| 2 | 1:36 |
| 3 | 2:00 |
| 4 | 2:30 |
| 5 | 3:12 |
| 6 | 4:00 |
| 7 | 5:00 |
| 8 | 6:24 |
| 9 | 8:00 |
| 10 | 10:00 |
| 11 | 12:30 |
| 12 | 16:00 |
| 13 | 20:00 |
| 14 | 25:00 |
| 15 | 32:00 |
| 16 | 40:00 |
| 17 | 50:00 |
| 18 | 1:00:00 |

Dalej tak samo w godzinach, przy czym zamiast „25 h" pojawia się 1 doba.

## Przykład: przepis na gofry

Przepis powstał przez iteracyjne eksperymentowanie z wartościami HSN, a następnie został przeskalowany o 2 kroki w górę (≈ ×1,6), żeby starczyło dla całej rodziny — bez przeliczania żadnych proporcji:

| Składnik | Ilość |
|----------|-------|
| Jajka | 3 |
| Mleko | 500 ml |
| Mąka pszenna | 400 g |
| Proszek do pieczenia | 1,6 łyżeczki |
| Olej rzepakowy | 100 ml |

Mleko (500 ml) i mąka (400 g) leżą dokładnie na wartościach HSN. Jajka są niepodzielne — zaokrąglone do najbliższej liczby całkowitej. Proszek do pieczenia 1,6 łyżeczki to wartość HSN; w praktyce 1,5 łyżeczki sprawdza się równie dobrze — przypomnienie, że HSN to punkt odniesienia, a nie sztywne ograniczenie.

Zobacz też: [Specyfikacja miarek kuchennych](tools_PL.md)

## Dla zainteresowanych

HSN jest zorientowaną na człowieka adaptacją serii R10 Renarda (ISO 3, 1952) i jest strukturalnie zbliżony do serii E12 stosowanej w elektronice. Tamte systemy były projektowane pod kątem tolerancji produkcyjnych i standaryzacji asortymentu. HSN jest zoptymalizowany pod codzienne ludzkie użycie: wartości są zaokrąglone tak, żeby były łatwe do zapamiętania, a nie matematycznie dokładne; wariant czasowy nie ma odpowiednika w seriach Renarda ani E.

Bazowy krok to 2^(1/3) ≈ 10^(1/10) — czyli około 26% między sąsiednimi wartościami. Sekwencja prędkości filmów ISO w krokach 1/3 EV (…25 — 32 — 40 — 50 — 64 — 80 — 100…) używa tego samego kroku i jest dobrze znanym, dziedzinowym przykładem tej samej idei.

## Licencja

CC0 — domena publiczna. Atrybucja niewymagana, choć mile widziana.
