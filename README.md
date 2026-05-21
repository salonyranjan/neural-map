# 🧠 Neural Map | 3D Knowledge Graph Portfolio

**Live Demo:** [salonyranjan.github.io/neural-map/](https://salonyranjan.github.io/neural-map/)

An interactive, force-directed 3D visualization of my software engineering projects, research, and technical repositories. Built to break away from traditional grid-based portfolios, this project represents my work as a living, breathing neural network.

### 🚀 Technical Overview
This project is split into an automated data pipeline and a high-performance 3D rendering engine:

* **The Data Engine (Python):** A custom GitHub fetcher script that analyzes my repositories. It calculates a distinct `complexity_score` based on commit history, code volume, and deployment status, exporting the sanitized data to a JSON pipeline.
* **The Physics Engine (D3.js):** Uses `d3-force-3d` to calculate real-time spatial repulsion, collision detection, and category-based attraction, allowing the graph to organically expand and settle.
* **The Rendering Engine (React Three Fiber):** A custom WebGL environment featuring a dynamic "Plexus" synapse background, emissive bloom post-processing, and raycasted hitboxes for precision interactions within a constantly drifting 3D space.

### 🛠️ Tech Stack
* **Frontend:** React, Next.js (Static Export), TypeScript
* **3D & Graphics:** Three.js, `@react-three/fiber`, `@react-three/drei`, `@react-three/postprocessing`
* **Physics:** `d3-force-3d`
* **Data Pipeline:** Python, PyGithub

### ✨ Features
* **Auto-Categorization:** Projects are automatically sorted into categories (Research, Tool, Design, Writing) based on repository naming conventions and complexity scores.
* **Dynamic Node Sizing:** Node radius and glow intensity scale proportionally with the project's calculated complexity.
* **Immersive Controls:** Full 3D camera orbit, pan, and zoom capabilities.
* **Interactive Tooltips:** Real-time data overlay on hover, with seamless click-through routing to live deployments or source code.
