# Calculus I MAT-140 - Bounce Physics Simulation & Calculus Derivatives

An interactive, responsive single-page web application that simulates a bouncing ball undergoing physics-based height decay across exactly 5 bounces. The simulator graphs the mechanical motion alongside its first derivative (Velocity) and second derivative (Acceleration) in real time.

<img width="421" alt="image" src="https://github.com/user-attachments/assets/f0c3481b-5b5e-4e71-9aa9-1fbad74dbbe2" />

Link to Live app: https://realityexpander.github.io/Calculus-I-Bounce-Simulation/

Link to conversation: https://share.google/aimode/6tB65UM5rrTYGHmWQ

## 🚀 Features

- **Real-Time Physics Engine:** Accurately models kinetic energy loss using a customizable Coefficient of Restitution ($e$).
- **Calculus Derivative Graphs:** Live canvas rendering of Position ($y$), Velocity ($rac{dy}{dt}$), and Acceleration ($rac{d^2y}{dt^2}$).
- **Interactive Controls:** Dynamic sliders to adjust Gravity ($g$), Bounce Efficiency ($e$), and Initial Drop Height ($H_0$).
- **Synchronized Tracking Crosshairs:** Cross-plot visual markers that lock onto precise timeline states during playback.
- **High-DPI Support:** Crisp, anti-aliased canvas rendering optimized for Retina and high-resolution screens.
- 
## 📐 Mathematical Model

The simulator tracks continuous cinematic equations segmented by boundary impacts:

1. **Position ($y$):** $y_{new} = y_{old} + v \cdot \Delta t$
2. **First Derivative - Velocity ($v$):** $v_{new} = v_{old} - g \cdot \Delta t$
3. **Second Derivative - Acceleration ($a$):** Constant pulling gravity ($-g$) interspersed with instantaneous impulse spikes ($+180$) upon ground impact ($y \le 0$).

Each consecutive peak height decays according to the restitution fraction:
$$H_n = H_0 \cdot e^{2n}$$

## 🛠️ Setup & Usage

1. Clone or download the repository.
2. Open `bounce_simulation.html` directly in any modern web browser.
3. Use the control sliders to dynamically alter physical behaviors during or before runtime loops.
