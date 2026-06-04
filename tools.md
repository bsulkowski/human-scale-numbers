# HSN Physical Tools — Specification

This document describes the design specification for HSN measuring tools intended for kitchen use. The tools are designed to be 3D-printed, but can be manufactured by any method. All designs are CC0 — anyone is free to implement, modify, and share them.

---

## 1. Spoon set

A set of six measuring spoons covering small quantities of dry and liquid ingredients.

### Values

| Spoon | Volume | Reference |
|-------|--------|-----------|
| 1 | 5 ml | 1 teaspoon |
| 2 | 6.4 ml | 1¼ teaspoon |
| 3 | 8 ml | 1⅗ teaspoon |
| 4 | 16 ml | 1 tablespoon (HSN) |
| 5 | 20 ml | 1¼ tablespoon |
| 6 | 25 ml | 1⅗ tablespoon |

Notes:
- The HSN tablespoon (16 ml) is defined independently of the traditional tablespoon (15 ml). The 1 ml difference is within the margin of error of typical kitchen measurement.
- Values above 25 ml are easily obtained by using a spoon multiple times (e.g. 2 × 16 ml = 32 ml, 4 × 16 ml = 64 ml).
- Values below 5 ml (e.g. 1.25 ml ≈ ¼ teaspoon) may be added as an optional extension.

### Design guidelines

- Spoons may be produced as individual pieces or connected in a set.
- Each spoon should be clearly labeled with its volume in ml.
- The bowl shape is not constrained — round, oval, or other forms are acceptable.
- Handle length should be sufficient for comfortable use and for hanging on a hook or ring.

---

## 2. Measuring cup

A tapered cup for measuring liquid and dry ingredients in larger quantities.

### Geometry

| Parameter | Value |
|-----------|-------|
| Diameter at base | 64 mm |
| Diameter at top (at 500 ml mark) | 100 mm |
| Working height (base to 500 ml mark) | ~95 mm |
| Total height (including spout margin) | ~110 mm |

The cup tapers linearly from base to top. This means the scale is denser at the bottom (where precision matters more) and more spread out at the top — a natural fit for the geometric nature of HSN values.

### Graduation marks

Calculated for a linearly tapered truncated cone with the dimensions above:

| Volume | Height from base | Inner diameter at mark | Gap from previous mark |
|--------|-----------------|----------------------|----------------------|
| 100 ml | 26.8 mm | 74 mm | — |
| 125 ml | 32.5 mm | 76 mm | 5.7 mm |
| 160 ml | 40.0 mm | 78 mm | 7.5 mm |
| 200 ml | 48.0 mm | 81 mm | 8.0 mm |
| 250 ml | 57.3 mm | 85 mm | 9.2 mm |
| 320 ml | 69.1 mm | 89 mm | 11.8 mm |
| 400 ml | 81.4 mm | 93 mm | 12.3 mm |
| 500 ml | 95.3 mm | 98 mm | 13.9 mm |

Note: gaps between marks range from ~6 mm to ~14 mm — readable and consistent. This is a direct consequence of the geometric sequence: each value is ~26% larger than the previous one, and the tapered shape distributes the marks evenly in physical space.

### Design guidelines

- A pouring spout is recommended.
- Graduation marks should be embossed or engraved, not just printed on the surface, for durability.
- Each mark should be labeled with its volume in ml.
- Wall thickness: minimum 1.5 mm for FDM printing.
- The base diameter (64 mm) is itself an HSN value — intentional.
- The design above is a reference geometry. Variations in shape (e.g. cylindrical, different taper, handle) are encouraged as long as the graduation mark heights are recalculated accordingly.

---

## Contributing

If you create a model based on this specification, consider sharing it on Printables, Thingiverse, or MakerWorld with a link back to this repository.
