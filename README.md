[README.md](https://github.com/user-attachments/files/32063341/README.md)
# Fossil Fractals

A generative art program that renders fossil-inspired fractal artwork in Python — chambered ammonite spirals, recursively branching fern fronds, and a fractal stone-texture backdrop, all composed into a single warm, sepia-toned piece.

## Description

**Fossil Fractals** combines several classic fractal-generation techniques to imitate the natural geometry found in real fossils:

- Ammonite shells are drawn as **logarithmic spirals**, the same growth curve seen in nautilus shells and galaxy arms, complete with ribbed "suture" chamber lines.
- Smaller ammonites are scattered around the focal shell using the **golden angle** (phyllotaxis), so the same shell shape repeats self-similarly at shrinking scales — much like a real fossil bed.
- Fern fronds are generated with a **recursive binary fractal tree**, where each branch is a smaller copy of the whole, echoing the self-similarity of real fern leaves.
- The rock backdrop is generated procedurally using the **diamond-square algorithm**, a classic fractal terrain technique that builds natural-looking texture by repeatedly averaging and perturbing midpoints at finer and finer scales.

## Fractal Types Implemented

| Fractal | Technique |
|---|---|
| Ammonite shell spirals | Logarithmic spiral (`r = a·e^(bθ)`) |
| Fossil fern fronds | Recursive self-similar branching (fractal tree) |
| Rock / stone texture | Diamond-square fractal terrain generation |
| Ammonite field layout | Golden-angle (phyllotaxis) self-similar scattering |

## Tools, Languages, and Libraries Used

- **Language:** Python 3
- **Libraries:**
  - [NumPy](https://numpy.org/) — vectorized math for spiral coordinates and the diamond-square height map
  - [Matplotlib](https://matplotlib.org/) — rendering, color gradients, and image export

## Setup and Run Instructions

1. **Install Python 3** (3.8 or later recommended).
2. **Install the required libraries:**
   ```bash
   pip install numpy matplotlib
   ```
3. **Run the script:**
   ```bash
   python fossil_fractal.py
   ```
4. The program will display the artwork in a window and save a rendered copy as `fossil_fractal.png` in the same folder.

To generate a different composition, change the `seed` value in the last line of the script:
```python
make_fossil_fractal_art(save_path="fossil_fractal.png", seed=7)
```

## Screenshot

![Fossil Fractals output](fossil_fractal_preview.png)

## Author

**Name:** Qazi Muhammad Anas Alam
**Registration Number:** 553047
