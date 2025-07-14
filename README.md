# MiniRT
**MiniRT** is a small ray tracing engine. The program renders 3D scenes using ray tracing techniques, supporting basic geometric primitives, lighting, and camera controls.

<img height="500" alt="Screenshot 2025-07-12 at 19 43 31" src="https://github.com/user-attachments/assets/ce1c665e-c92e-4a14-b799-bfb0dc1fe4c1" />

<img width="1169" height="845" alt="Screenshot 2025-07-12 at 19 45 01" src="https://github.com/user-attachments/assets/9728a0a8-00f3-42e4-9b3c-92e847459d17" />

---

## Features

- Ray tracing engine with support for:
  - Point light sources
  - Ambient lighting
  - Perspective camera
  - Simple scene description file format

---

## Build

To compile the project, run:

```bash
make
./miniRT [scene.rt]
```


## Scene File Format

Scenes are described in plain text using one element per line. Parameters are space-separated.
<img width="674" height="227" alt="Screenshot 2025-07-14 at 10 04 06" src="https://github.com/user-attachments/assets/cce3fe11-25c2-420c-bbff-eb0d5c95e7b6" />

## Supported objects

Each object is defined with its parameters on a single line. Common properties like color and material coefficients (ambient, diffuse, specular) are included. Specular exponent controls the shininess of the surface. Supported objects: Plane, Disc, Sphere, Triangle, Cone

---

### Object format example – Plane

```txt
pl  <position>  <normal_vector>  <color>  <amb,diff,spec>  <spec_exp>  [optional label]
```
Position: A point on the plane (x,y,z)

Normal Vector: The plane’s orientation (x,y,z)

Color: RGB values (0–255)

Material: Ambient, Diffuse, Specular coefficients (0.0–1.0)

Specular Exponent: Controls highlight sharpness (higher = shinier)

---

