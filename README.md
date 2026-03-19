# Reality Simulator 

A browser-based particle physics playground. Spawn particles, bend the laws of physics, and watch your own little universe unfold — all in vanilla HTML, CSS, and JavaScript. No dependencies. No build step. Just open and run.

---

## Demo

Click anywhere on the canvas to spawn particles. Hit **Big Bang** to explode them all outward from the center. Tweak gravity, bounce, and friction in real time.

---

## Features

- **5 physics modes** — Gravity, Repulsion, Attraction, Chaos, Orbit
- **Real-time controls** — Adjust gravity, bounce elasticity, and friction on the fly
- **Particle trails** — Motion blur-style trails for each particle
- **Click to spawn** — Click anywhere on the canvas to add new particles
- **Big Bang** — Explodes all particles outward from the center
- **Kinetic energy tracker** — Live stats for particle count and total energy
- **Responsive canvas** — Scales to fit any screen size
- **Zero dependencies** — Pure vanilla JS, no libraries or frameworks

---

## Getting Started

No installation needed.

```bash
git clone https://github.com/your-username/reality-simulator.git
cd reality-simulator
open reality_simulator.html
```

Or just download `reality_simulator.html` and open it in your browser.

---

## Physics Modes

| Mode | Description |
|------|-------------|
| **Gravity** | Particles fall downward and bounce off walls |
| **Repulsion** | Particles flee from your cursor |
| **Attraction** | Particles are pulled toward your cursor |
| **Chaos** | Random forces act on every particle every frame |
| **Orbit** | Particles orbit around the center of the canvas |

---

## Controls

| Control | Effect |
|---------|--------|
| **Gravity** slider | Strength of downward pull |
| **Bounce** slider | Energy retained on wall collision (0 = absorb, 1 = perfect bounce) |
| **Friction** slider | Velocity damping per frame |
| **Particles** dropdown | Number of particles in the simulation |
| **Physics** dropdown | Active physics mode |
| **Reset** | Respawn all particles randomly |
| **Big Bang** | Explode all particles from the center |
| **Click canvas** | Spawn 8 new particles at cursor position |

---

## File Structure

```
reality-simulator/
└── reality_simulator.html   # The whole thing — self-contained
```

---

## How It Works

Each particle has a position, velocity, mass (proportional to radius²), color, and a short trail history. Every frame:

1. Forces are applied based on the active physics mode
2. Velocity is scaled by friction and capped at a max speed
3. Position is updated and trail history is appended
4. Wall collisions are resolved with configurable energy retention
5. Canvas is redrawn with a semi-transparent overlay to produce the trail fade effect

---

## License

MIT — do whatever you want with it.

---
