# 高速公路应急车道更换备胎

Guided Three.js walkthrough of a spare-tire change on a highway emergency shoulder: golden-hour lighting, a vendored PBR car, and a Chinese slideshow. The camera moves itself — a first-time viewer only presses **下一步**.

License plate text (front and rear): **www.3Dfans.site**

## Run

The page loads Three.js as an ES module, so serve the repository root over HTTP. Opening `index.html` as a `file://` URL will not work.

```bash
python3 -m http.server
```

Then open [http://127.0.0.1:8000/](http://127.0.0.1:8000/).

## How to watch

The page is a guided slideshow, not a free-orbit sandbox.

- **下一步 / 上一步** (or ← → and Space) plays that step’s short demo: hazards, chock, tools, lug nuts, jack, and wheel.
- The camera eases (about 1.3s) onto the thing you are doing — usually the curb-side rear wheel, the jack pad, or the tools — and stays there. Loading opens on step 1 already framed, not on a distant highway shot.
- The numbered bar jumps to a step and replays it. It is secondary to the big Next button.
- **自由看一眼** turns on drag-orbit and scroll-zoom. The next step change turns it off and returns to the guided camera.

`?step=4&snap=1` jumps to a step’s finished pose (steps are 0–9). `shots/` holds reference screenshots.

## Attribution

### CarConcept — CC BY 4.0

`vendor/car/CarConcept.glb` is the Khronos [CarConcept](https://github.com/KhronosGroup/glTF-Sample-Assets/tree/main/Models/CarConcept) glTF sample (concept / grand-touring coupe, in-app paint **Torched Graphite**).

- License: [Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/)
- © 2024 Darmstadt Graphics Group GmbH — model and textures by Eric Chadwick
- Based on “FREE Concept Car 004” by Unity Fan (Sketchfab), CC0
- © 2015 Khronos Group — Khronos logo (trademark)
- © 2017 Khronos Group — 3D Commerce logo (trademark)

Full notice: `vendor/car/LICENSE.txt`.

`vendor/car/sedan-original.glb` is an unused fallback from the Innerscene 3D Parts Library (sedan), [CC0 1.0](https://creativecommons.org/publicdomain/zero/1.0/).

### HDRI — Poly Haven

`vendor/hdri/kiara_1_dawn_1k.hdr` is [Kiara 1 Dawn](https://polyhaven.com/a/kiara_1_dawn) by Poly Haven, [CC0 1.0 Universal](https://creativecommons.org/publicdomain/zero/1.0/). See `vendor/hdri/LICENSE.txt`.

### Three.js

`vendor/three/` is [Three.js](https://threejs.org/) r160 (MIT), including OrbitControls, GLTFLoader, and RGBELoader.
