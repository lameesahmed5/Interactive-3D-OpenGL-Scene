# Interactive 3D Nature Scene Framework (OpenGL & GLUT)

An interactive, real-time 3D outdoor graphic environment simulated using modern C++ architectural components combined with standard OpenGL and Utility Toolkit (GLUT) libraries.

## 1. Scene Composition & Architecture
The scene aggregates a dynamic layout of over 24 independent operational objects constructed dynamically using low-level primitive topologies and geometric structures:
* **Structural Flora:** A customized tree rendered via localized polygon meshes and scaling matrices.
* **Perimeter Components:** A looped procedural wooden perimeter fence utilizing standard 3D solid cube configurations.
* **Atmospheric Assets & Textures:** Soft layered clouds and high-altitude celestial bodies rendered with multi-layered dimensional spheres.
* **Natural Terrains:** Detailed organic cluster rock matrices arranged sequentially to preserve structural orientation properties.

---

## 2. Advanced Graphics Pipeline Engineering

### Spatial Depth Integrity Validation
To prevent overlapping geometric occlusion anomalies across the viewport coordinate system, strict runtime depth evaluation blocks (`GL_DEPTH_TEST`) were enabled alongside sequential buffer clears (`GL_DEPTH_BUFFER_BIT`) to handle intersecting spatial entities cleanly.

### Illumination & Structural Color Synthesis
Standard multi-source lighting modes (`GL_LIGHTING`, `GL_LIGHT0`) were integrated to cast realistic shadow profiles. Material tracking flags (`GL_COLOR_MATERIAL`) were deployed sequentially to retain true vertex colors from being overridden by diffuse light variables.

### Real-time Kinematic Animation Loops
Continuous vertical movement mechanics were synthesized by maintaining real-time frame updating threads using callback operations (`glutIdleFunc`). Falling boundaries are checked against conditional boundary controls (`dropY > -30.0f`) to force natural landing stops at the base coordinate plane.

### Stateful Event Controls & Blending
Dynamic user events allow keyboard-driven translation matrices to shift components left/right asynchronously via localized conditional execution logic. Translucent properties were injected into ambient background quads using custom Alpha Blending equations (`GL_BLEND` and `glBlendFunc`).

---

## 3. Keyboard Controller Configurations
The runtime simulation loop interprets hardware user trigger events based on the following mapping architecture:

| Bound Key Command | Targeted Operation Handler | State Result Mapping |
| :---: | :--- | :--- |
| `A` / `a` | Increments current translation parameters (`moveX += 5`) | Structural segments translate horizontally to the left. |
| `B` / `b` | Decrements current translation parameters (`moveX -= 5`) | Structural segments translate horizontally to the right. |
| `SPACE` | Resets current global coordinate offsets to defaults | Restores camera translation, rotation angle, and resets animation states. |

---
*Developed as part of the Computer Graphics Lab Project (CS360) course at Princess Noura bint Abdulrahman University.*
