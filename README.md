# 🔵 Volume Tire Calculator

A Python command-line tool that calculates the volume of a tire using its standard three-number size code (e.g. 205/55R16), applying geometric formulas to derive the inner and outer torus dimensions.

---

## Features

- ✅ Accepts standard tire size notation as input (width, aspect ratio, rim diameter)
- ✅ Computes tire volume using torus geometry
- ✅ Displays results in cubic inches and liters
- ✅ Input validation for realistic tire dimensions

---

## Demo

```
=== Tire Volume Calculator ===

Enter tire width (mm):        205
Enter aspect ratio (%):        55
Enter rim diameter (inches):   16

--- Results ---
Tire Size:        205/55R16
Sidewall Height:  112.75 mm  (4.44 inches)
Outer Diameter:   632.5 mm   (24.90 inches)

Volume:           33.51 liters
                  2,045.8 cubic inches
```

---

## How to Run

**Requirements:** Python 3.x

```bash
# Clone the repository
git clone https://github.com/f-anselm88/volume-tire.git

# Navigate into the project
cd volume-tire

# Run the program
python volume_tire.py
```

---

## The Formula

A tire's cross-section forms a torus (donut shape). Volume is calculated as:

```
Sidewall Height = Width × (Aspect Ratio / 100)
Outer Radius    = (Rim Diameter / 2) + Sidewall Height
Inner Radius    = Rim Diameter / 2

Volume = (π² / 4) × (Outer Radius + Inner Radius) × (Outer Radius - Inner Radius)²
```

---

## What I Learned

- Translating real-world engineering specifications into computational formulas
- Working with Python's `math` module (`math.pi`)
- Unit conversion between metric and imperial measurements

---

## Author

**Anselm Munango**
[f-anselm88.github.io](https://f-anselm88.github.io) · [GitHub](https://github.com/f-anselm88) · [LinkedIn](https://linkedin.com/in/anselm-munango-bs) · [anselm.mu@gmail.com](mailto:anselm.mu@gmail.com)

