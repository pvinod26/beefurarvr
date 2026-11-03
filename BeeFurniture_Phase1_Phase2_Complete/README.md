# Bee Furniture — Phase 1 + Phase 2 starter

## What is included
- `index.html`: the supplied Phase 1 Bee Furniture website, retained as the foundation, with a Phase 2 **Watch in My Room** AR entry point added to sofa details. There is no separate 3D product-viewing page or visible 3D viewer.
- `models/sample-sofa.glb`: a generic sample model for demonstrating the AR launch workflow only.
- `variant-data.example.json`: example structure for adding verified, product-specific colour photographs and AR model paths.

## Run locally
Because camera and AR features require a secure context, use HTTPS when testing on a phone. For local desktop preview, opening `index.html` may show the catalogue, but AR requires a deployed HTTPS origin or localhost.

## Deploy to Render (Static Site)
1. Create a GitHub repository.
2. Extract this ZIP and upload the **contents** of this folder to the repository root. `index.html` must be directly at the root, and `models/` must be beside it.
3. In Render choose **New → Static Site** and connect the repository.
4. Root Directory: leave blank.
5. Build Command: leave blank.
6. Publish Directory: `.`
7. Deploy, then open the HTTPS Render URL on a compatible phone.

## Important asset limitations
The supplied Phase 1 catalogue contains reference product images and requested colour names, not verified Bee Furniture colour-variant photos or product-specific 3D models. This package does not invent them. The Watch in My Room button currently demonstrates the AR workflow using a clearly labelled generic sample sofa. To show the exact sofa selected, add its approved GLB/glTF model and configure that product to use it. To make colour selection switch the actual photograph, supply a genuine photograph for each available colour and connect it to the product variant data.

## AR compatibility
The browser/device decides which AR mode is available. Android Scene Viewer generally requires a compatible Android device and Google Play Services for AR; iOS AR Quick Look requires a compatible iPhone/iPad and a USDZ asset. WebXR support varies by browser. The page reports when AR cannot be launched. Test on physical devices before claiming universal support.

## Existing Phase 1 notes
Catalogue prices and external product photographs in the original file are reference/demo content. Confirm ownership, product accuracy, pricing, colour availability and WhatsApp contact details before publishing commercially.
