# 🌌 Black Hole JSS Simulations

An interactive web-based simulation of a black hole built using **HTML, CSS, and JavaScript**.  
It uses the Canvas API to render a real-time visualization of particles influenced by a simplified gravitational field.

🔗 Live Demo:  
https://alcatord.github.io/Black-Hole-JSS-Simulations/

🔗 GitHub Repository:  
https://github.com/Alcatord/Black-Hole-JSS-Simulations

---

## 📁 Project Structure


Black-Hole-JSS-Simulations/
│
├── index.html # Main HTML file (canvas container)
├── style.css # Styling (layout, background, visuals)
├── script.js # Simulation logic (physics + animation)
└── assets/ # Optional resources (images, effects)


---

## 📖 Overview

This project is a visual and interactive simulation inspired by black holes and gravitational physics.  
It is designed for educational and demonstration purposes, helping users understand how objects behave under strong central forces.

Instead of using complex astrophysical equations, the simulation relies on **simplified physics models** to produce smooth, visually appealing motion that is easy to understand and computationally efficient in the browser.

---

## ✨ Key Features

- 🌠 Real-time particle simulation
- 🕳️ Central black hole attraction effect
- 🔄 Smooth orbital and spiral motion
- ⚡ Lightweight physics-based animation
- 🎨 Canvas-based rendering for performance
- 🧠 Simplified gravitational model for visual clarity

---

## ⚙️ How It Works

### 🖥️ 1. Canvas Rendering System

The simulation runs entirely inside an HTML `<canvas>` element.  
JavaScript continuously redraws the scene using `requestAnimationFrame()` to create smooth animations.

Each frame follows this cycle:

1. Clear the canvas
2. Update particle positions
3. Apply gravitational forces
4. Redraw all elements
5. Repeat

This creates a fluid and continuous motion effect.

---

### 🌠 2. Particle System

The simulation is based on multiple independent particles.

Each particle contains:

- Position (`x`, `y`)
- Velocity (`dx`, `dy`)
- Direction toward the black hole
- Speed affected by distance

Particles move freely but are continuously influenced by the black hole’s gravitational pull.

---

### 🕳️ 3. Black Hole Behavior

The black hole is positioned at the center of the canvas and acts as the main force generator.

It:

- Attracts all particles inward
- Serves as the simulation’s central point
- Creates orbital instability near its center

As particles approach the black hole:

- Their velocity increases
- Their trajectory becomes spiral-like
- Some may disappear visually when reaching the center

---

### 🌌 4. Gravity Model (Simplified Physics)

Instead of using real astrophysical equations, the project uses a simplified inverse-distance model:

- Distance between particle and black hole is calculated
- A force is applied inversely proportional to this distance
- Closer particles experience stronger attraction

This results in visually realistic effects such as:

- Orbital motion
- Spiral trajectories
- Accelerated collapse near the center

---

### 🔁 5. Animation Loop

The entire simulation is driven by a continuous animation loop:

```js
function animate() {
    updateParticles();   // Update physics
    drawBlackHole();     // Render black hole
    drawParticles();     // Render particles
    requestAnimationFrame(animate);
}

This loop ensures smooth 60fps animation in most modern browsers.

🎯 Purpose of the Project

This simulation is intended for:

Educational demonstrations of gravity-like behavior
Visualizing particle motion under central force
Experimenting with Canvas-based animations
Learning basic physics simulation concepts in JavaScript
🚀 Technologies Used
HTML5 (Canvas)
CSS3 (Styling and layout)
JavaScript (Physics and animation logic)
📌 Notes
This is not a scientifically accurate astrophysics simulation
It is optimized for visual clarity and performance
Physics behavior is intentionally simplified for educational purposes
📜 License

This project is open-source and free to use for educational and personal projects.

👨‍💻 Author

Developed by Alcatord
GitHub: https://github.com/Alcatord
