BEE FURNITURE — STANDALONE 3D / AR PROTOTYPE

WHAT THIS IS
- A separate prototype. It does not modify or depend on the existing Bee Furniture website or Flask backend.
- Interactive GLB viewer with orbit/zoom controls.
- Colour preview tint controls.
- AR launch button using model-viewer's Scene Viewer (Android), WebXR and Quick Look (iOS) modes.

RUN LOCALLY
1. Extract the ZIP.
2. Open the folder in VS Code.
3. In the terminal, run: python -m http.server 8000
4. On the same computer, open: http://localhost:8000

IMPORTANT AR TESTING
- For actual phone AR, deploy this folder to an HTTPS host (Render Static Site, GitHub Pages, or another HTTPS host).
- Open the HTTPS URL on the phone. Camera/AR support depends on device, browser and installed AR services.
- Android generally uses Google Scene Viewer. iPhone generally uses AR Quick Look.
- A normal desktop browser can inspect the 3D model but cannot provide room AR.

MODEL
The demo uses the Lowline - Low Three-Seat Sofa GLB hosted by Innerscene. The model page describes it as CC0 and approximately 260 x 95 x 84 cm, with embedded PBR materials. The model is loaded from its hosted URL; internet access is required. If the host changes its URL or blocks cross-origin loading, download the GLB from the source page and place it in models/low-profile-three-seat-sofa.glb, then change the model-viewer src in index.html to that local path.
Source/model page:
https://www.innerscene.com/tools/library/3d-parts/lowline-low-three-seat-sofa-4bb27e8c

LIMITATIONS OF THIS FIRST TRIAL
- Colour controls apply a uniform material tint to all model materials. This is a technical preview, not separate manufacturer colour variants.
- Sofa dimensions are those stated on the source model page; verify scale in a real room before treating it as a product measurement.
- This prototype is not yet merged into Bee Furniture.
