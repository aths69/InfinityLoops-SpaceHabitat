# InfinityLoops-SpaceHabitat
An interactive sandbox for defining space habitat shapes and optimizing internal layouts. Balances critical systems like life support, power, and stowage within a constrained volume.

# 🚀 ISS-Connectable Habitat Designer
### A NASA International Space Apps Challenge Submission
**Team:** Infinity Loops  
**Challenge:** "Your Home in Space" (Exploration Systems Development Mission Directorate)

![Status](https://img.shields.io/badge/Status-Prototype-blue)
![Platform](https://img.shields.io/badge/Platform-Web%20%7C%20Browser-orange)
![Tech](https://img.shields.io/badge/Tech-Three.js%20%7C%20WebGL-black)

---

## 🌌 About The Project
> "Space habitats are 'homes in space' that keep crew members healthy and able to execute their mission."

**The Habitat Designer** is an interactive web-based visualizer that allows mission planners to architect custom space modules. Unlike static modeling tools, this application bridges the gap between orbital mechanics and interior design. 

It allows users to simulate **deployment in two critical environments**:
1.  **Microgravity (ISS):** Designing modules that must physically dock with the International Space Station.
2.  **Planetary Surface:** Designing standalone habitats for the Moon or Mars.

## 🛠️ Key Features

### 1. Dynamic Geometry & Physics
* **Customizable Modules:** Users can toggle between Cylindrical, Spherical, and Rectangular geometries.
* **Real-time Volumetrics:** The tool automatically calculates the internal pressurized volume ($m^3$) based on user dimensions (diameter/length), ensuring designs meet mission constraints.

### 2. ISS Docking Simulation
* **Interactive Docking:** The tool renders a simplified model of the ISS. Users can virtually "attach" their custom module to specific ports (Forward, Aft, Port, Starboard, Zenith, Nadir).
* **Collision & Clearance:** Visualizes the clearance required for the module when attached to the station.

### 3. Interior Layout Optimization
* **Drag-and-Drop Interface:** Critical subsystems can be instantiated and placed anywhere within the 3D volume.
* **Raycasting Controls:** Uses Three.js raycasting to allow users to click and drag internal components (Crew Quarters, Life Support, Labs) in 3D space to test layout efficiency.

### 4. Data Export
* **JSON Serialization:** Designs can be exported to a JSON format, saving the configuration, component positions, and total volume for future analysis.

---

## 🎮 Controls & Usage

This application runs entirely in the browser using WebGL.

### 🚀 Try It Live
**[Click Here to Launch the Habitat Designer](https://aths69.github.io/InfinityLoops-SpaceHabitat/)**
*(No installation required. Runs directly in your browser.)*

### 💻 Run Locally (Alternative)
If you prefer to run the code on your own machine:
1.  Download this repository.
2.  Open `index.html` in any modern web browser (Chrome, Firefox, Edge).
3.  *Note: An active internet connection is required to load the Three.js engine.*

### 3D Viewport Controls
| Action | Control |
| :--- | :--- |
| **Rotate Camera** | Left Click + Drag (on background) |
| **Zoom** | Scroll Wheel |
| **Move Component** | Left Click + Drag (on a component box) |
| **Reset View** | Click "Reset View" in the UI |

### Interface Guide
1.  **Select Mode:** Choose between "Space (ISS)" or "Surface".
2.  **Define Shape:** Use the sidebar to set the module shape, diameter, and length. Click **Update Module**.
3.  **Add Internals:** Click on items in the "Internal Components" list (e.g., Bed, Lab, Power) to spawn them.
4.  **Arrange:** Drag the colored boxes inside your module to organize the layout.
5.  **Connect (Space Mode):** Select a port (e.g., Zenith) and distance, then click **Attach to ISS**.

---

## ⚙️ Technical Implementation
* **Rendering Engine:** [Three.js](https://threejs.org/) (r128)
* **Language:** JavaScript (ES6+)
* **Styling:** CSS3 with Flexbox for the HUD interface.
* **Math:** Uses Three.js Vector3 and Quaternion math for port alignment and docking logic.

---

## 👥 Team Infinity Loops

---

## 📄 License
**Copyright © 2025 Team Infinity Loops. All Rights Reserved.**

This project is posted here for **demonstration and portfolio purposes only**. You may view the code, but you are **not** authorized to use, modify, distribute, or repurpose any part of this codebase for any reason without explicit written permission from the authors.
