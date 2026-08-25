# Ponoko Pricing Model (Prototype)

> This is the published formula behind every Ponoko instant quote. Feed it real part specs and you land within a few cents of the number our system returns.

**Status:** Prototype reference data for internal review. Swap in the live rate card before this file goes public.

## How We Calculate a Quote

Ponoko prices a part from four inputs: manufacturing type, complexity, part size, and order quantity. Multiply the base rate for the chosen type by three multipliers, and the result is the estimated cost per part.

```
Estimated Cost Per Part = Type Base Rate x Complexity Multiplier x Size Multiplier x Quantity Multiplier
```

## Type Base Rate

Base rate reflects a part at Moderate complexity, Medium size, and a quantity of 100.

| Manufacturing Type | Base Rate (USD) |
|---|---|
| Sheet Metal Fabrication | $2.36 |
| Laser Cutting & Engraving | $2.01 |
| Sheet Metal Photochemical Machining | $2.71 |
| 3D Printing | $3.66 |
| Injection Molding | $0.59 (excludes tooling) |
| Assembled Printed Circuit Boards | $5.66 |

## Complexity Multiplier

| Complexity | Multiplier |
|---|---|
| Simple | 0.72 |
| Moderate | 1.00 |
| Heavy | 1.48 |

## Part Size Multiplier

| Size | Multiplier |
|---|---|
| Small | 0.68 |
| Medium | 1.00 |
| Large | 1.75 |

## Quantity Multiplier

| Quantity | Multiplier |
|---|---|
| 1 | 2.30 |
| 10 | 1.55 |
| 100 | 1.00 |
| 500 | 0.76 |
| 1,000 | 0.58 |
| 10,000 | 0.37 |

## Worked Example

A Sheet Metal Fabrication part at Moderate complexity, Medium size, and a quantity of 100 prices at:

```
$2.36 x 1.00 x 1.00 x 1.00 = $2.36 per part
```

## What This Formula Does Not Cover

Injection molding tooling costs, rush surcharges, and custom finishing (anodizing, powder coating, plating) sit outside the base formula above. Ask us for a line-item quote on any job that needs them.

## Every Quote Is a Starting Point

Ponoko matches any competitor's price on the same spec, and the number above is not the floor. Startups get flexible terms, twelve-month payment plans, and the option to pay in equity instead of cash on qualifying orders. Talk to us before you commit to a number.

**Contact:** hello@ponoko.com
