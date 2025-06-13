# Apple Tree Animation – Perlin Noise Edition

This is my individual contribution to the group project for animating the apple tree image. My version uses Perlin noise to create smooth, organic animations for the visual elements of the tree.
---

## Interaction Instructions

- Open the project in your browser (or use a live server).
- The animation starts automatically.
- Watch how the branches breathe and shift in color over time.
- There is no mouse or audio interaction in this version – it's a passive animation driven by code.

---

## Individual Animation Approach

I chose Perlin noise to animate various properties of the apple tree circles (branches and trunk).

### Properties I Animated:
1. The size of each circle changes using a pulse animation
2. There is a color shift on the top and bottom of each circle (especially visible on branches).
3. Stroke weight is added and animated to slightly beat with the animation.

These effects symbolise a breathing, living tree that reacts to natural forces.

---

## How It’s Different From My Group

- Other members used different methods such as randomness or interaction.
- My version focuses on:
  - Smooth, continuous movement
  - No user input
  - Gradual and organic animation using Perlin noise
- I added subtle stroke animation, which others didn’t.

---

## Inspirations

I was inspired by:
- Nature-based animations like wind-blown trees
- Generative art using noise:  
  - https://openprocessing.org/sketch/792689

These references showed how Perlin noise can make graphics feel “alive”.

---

## Technical Summary

- Code written in p5.js
- Main file modified: `branches.js`
- Added `this.noiseOffset = random(1000)` in the `Circles` constructor to randomize animation seeds.
- Used `noise(this.noiseOffset + frameCount * 0.01)` to animate:
  - ball diameter (scaled with `map()`)
  - stroke weight
  - color brightness and tones

### Key functions used:
- `noise()` – for smooth time-based animation
- `map()` – to convert noise to meaningful values
- `lerpColor()` – to smoothly transition colors

---

## Commit History

| Commit Message | Description |
|----------------|-------------|
| `Initial project setup with group code` | Imported base tree structure and mosaic background |
| `Add Perlin noise animation to diameter (individual work)` | Animated the size of each circle using noise |
| `Add color animation and noiseOffset for each circle` | Added color shifting based on noise |
| `Add animated strokeWeight using Perlin noise` | Final touch: stroke weight now pulses smoothly |

---

## How to Run

1. Clone the repository: git clone https://github.com/janasbat/apple-tree-perlin-animation.git
2. Open `index.html` in a browser.
3. Make sure you have the `/Assets` folder with the original artwork image.


2025 – Group 5 Final Project
Individual submission by Jana Sbat


