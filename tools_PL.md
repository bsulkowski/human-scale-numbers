# Narzędzia HSN — Specyfikacja

Ten dokument opisuje specyfikację projektową miarek HSN przeznaczonych do użytku w kuchni. Narzędzia zostały zaprojektowane z myślą o druku 3D, ale mogą być wykonane dowolną metodą. Wszystkie projekty są objęte licencją CC0 — każdy może je implementować, modyfikować i udostępniać.

---

## 1. Zestaw miarek łyżkowych

Zestaw sześciu miarek łyżkowych do odmierzania małych ilości składników sypkich i płynnych.

### Wartości

| Miarka | Objętość | Odniesienie |
|--------|----------|-------------|
| 1 | 5 ml | 1 łyżeczka |
| 2 | 6,4 ml | ~1,25 łyżeczki |
| 3 | 8 ml | 1,6 łyżeczki |
| 4 | 16 ml | 1 łyżka (HSN) |
| 5 | 20 ml | 1,25 łyżki |
| 6 | 25 ml | ~1,6 łyżki |

Uwagi:
- Łyżka HSN (16 ml) jest zdefiniowana niezależnie od tradycyjnej łyżki (15 ml). Różnica 1 ml mieści się w marginesie błędu typowego pomiaru kuchennego.
- Wartości powyżej 25 ml łatwo uzyskać wielokrotnym użyciem miarki (np. 2 × 16 ml = 32 ml, 4 × 16 ml = 64 ml).
- Wartości poniżej 5 ml (np. 1,25 ml ≈ 0,25 łyżeczki) można dodać jako opcjonalne rozszerzenie zestawu.

### Wytyczne projektowe

- Miarki mogą być wykonane jako osobne elementy lub połączone w zestaw.
- Każda miarka powinna być czytelnie oznaczona objętością w ml.
- Kształt czerpaka nie jest narzucony — okrągły, owalny lub inny są dopuszczalne.
- Długość rączki powinna umożliwiać wygodne trzymanie oraz zawieszenie na haku lub kółku.

---

## 2. Miarka

Rozszerzające się naczynie do odmierzania płynnych i sypkich składników w większych ilościach.

### Geometria

| Parametr | Wartość |
|----------|---------|
| Średnica przy podstawie | 64 mm |
| Średnica na górze (przy kresce 500 ml) | 100 mm |
| Wysokość robocza (od podstawy do kreski 500 ml) | ~95 mm |
| Wysokość całkowita (z marginesem na dziubek) | ~110 mm |

Naczynie rozszerza się liniowo od podstawy ku górze. Oznacza to, że skala jest gęstsza na dole (gdzie precyzja jest ważniejsza) i rzadsza na górze — naturalne dopasowanie do geometrycznej natury wartości HSN.

### Podziałki

Obliczone dla liniowo rozszerzającego się stożka ściętego o podanych wymiarach:

| Objętość | Wysokość od podstawy | Średnica wewnętrzna | Odstęp od poprzedniej kreski |
|----------|---------------------|--------------------|-----------------------------|
| 100 ml | 26,8 mm | 74 mm | — |
| 125 ml | 32,5 mm | 76 mm | 5,7 mm |
| 160 ml | 40,0 mm | 78 mm | 7,5 mm |
| 200 ml | 48,0 mm | 81 mm | 8,0 mm |
| 250 ml | 57,3 mm | 85 mm | 9,2 mm |
| 320 ml | 69,1 mm | 89 mm | 11,8 mm |
| 400 ml | 81,4 mm | 93 mm | 12,3 mm |
| 500 ml | 95,3 mm | 98 mm | 13,9 mm |

Uwaga: odstępy między kreskami wynoszą od ~6 mm do ~14 mm — czytelne i spójne. To bezpośrednia konsekwencja ciągu geometrycznego: każda wartość jest o ~26% większa od poprzedniej, a rozszerzający się kształt naczynia równomiernie rozkłada kreski w przestrzeni fizycznej.

### Wytyczne projektowe

- Zalecany dziubek do przelewania.
- Podziałki powinny być wytłoczone lub wgłębione, nie tylko nadrukowane na powierzchni — dla trwałości.
- Każda kreska powinna być opisana objętością w ml.
- Grubość ścianki: minimum 1,5 mm przy druku FDM.
- Średnica podstawy (64 mm) jest sama w sobie wartością HSN — celowy wybór.
- Geometria powyżej jest geometrią referencyjną. Warianty kształtu (np. walec, inne rozszerzenie, uszko) są mile widziane, pod warunkiem przeliczenia wysokości podziałek.

---

## Udział w projekcie

Jeśli stworzysz model na podstawie tej specyfikacji, rozważ jego udostępnienie na Printables, Thingiverse lub MakerWorld z linkiem do tego repozytorium.
