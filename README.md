# 高速公路应急车道更换备胎

Interactive Three.js scene of a spare-tire change on a highway emergency shoulder: cinematic golden-hour lighting, a vendored PBR car, and a step-by-step Chinese walkthrough.

License plate text (front and rear): **www.3Dfans.site**

## Run

The page loads Three.js as an ES module, so serve the repository root over HTTP. Opening `index.html` as a `file://` URL will not work.

```bash
python3 -m http.server
```

Then open [http://127.0.0.1:8000/](http://127.0.0.1:8000/).

Drag to orbit and scroll to zoom. Use **上一步 / 下一步**, or the left and right arrow keys (or Space), to move through the procedure. Add `?step=4&snap=1` to jump to a step.

`shots/` holds reference screenshots of the scene.

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
