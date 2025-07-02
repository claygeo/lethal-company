Ultra Immersive (Three.js Fan Demake)

> **Play in your browser • No installs • 100 % JavaScript & WebGL**

## Table of Contents

* [About](#about)
* [Features](#features)
* [Play Now](#play-now)
* [Controls](#controls)
* [Getting Started (Dev)](#getting-started-dev)

## About

“**Lethal Company – Ultra Immersive**” is a **browser‑based fan demake** of Zeekerss’ co‑op survival horror hit *Lethal Company*.
Built from scratch with **[Three.js](https://threejs.org)** and vanilla JavaScript, the project is my playground for procedural level generation, enemy AI, and WebGL performance tricks.

> **Disclaimer :** This is an unofficial, fan‑made project. I am **not affiliated with or endorsed by Zeekerss**. Made purely for learning & fun.

---

## Features

|   Feature                                                                                                           |
| --------------------------------------------------------------------------------------------------------------------|
|  First‑person exploration with pointer‑lock camera & smooth WASD movement                                           |
|  Three enemy archetypes with distinct hunt behaviours (Stalker, Charger, Dodger) powered by a lightweight FSM       |
|  Real‑time shadows, volumetric fog & bloom post‑processing for atmosphere                                           |
|  Positional audio cues & dynamic reverb zones                                                                       |
|  Procedural scrap spawning + basic quota/HUD tracking                                                               |
|  Modular ES‑module architecture – no bundler required                                                               |

## Play Now

1. **Clone / Download** the repo.
2. Open **`index.html`** in any modern desktop browser (Chrome ≥ 117, Edge, Firefox).
   That’s it – everything is loaded from CDNs.

*(Optional)* Serve locally for correct audio‑origin policies:

```bash
python -m http.server 8080
# or
npx serve .
```

Browse to **[http://localhost:8080](http://localhost:8080)**.

---

## Controls

|  Action            |  Key        |
| ------------------ | ----------- |
| Move               | **W A S D** |
| Sprint             | **Shift**   |
| Jump               | **Space**   |
| Crouch             | **Ctrl**    |
| Interact / Pick Up | **E**       |
| Toggle Flashlight  | **F**       |
| Exit Pointer‑Lock  | **Esc**     |

---

## Getting Started (Dev)

```bash
# 1 – Clone
 git clone https://github.com/claygeo/lethal-company-threejs.git
 cd lethal-company-threejs

# 2 – Serve (recommended)
 npx serve .
# or
 python -m http.server 8080

```

Dependencies are pulled via CDN (Three.js r128, dat.GUI, howler.js).
For a bundled version with tree‑shaking, see the **/build** branch (Vite).
