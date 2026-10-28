# Sky at Brio / General Property 3D Walkthrough Generator

Fully set up stack. Input a property URL → outputs a browser-navigable walkthrough in the familiar style users know (thumbnail/point navigation + full view, similar to Matterport's click-to-move feel).

## Quick Start
```bash
pip install -r requirements.txt
python generate.py "https://www.skyatbrio-apts.com/"
# Then open walkthrough.html in any browser
```

## What it does
1. Scrapes public images from the given URL (gallery, listing photos).
2. Prepares reconstruction path (COLMAP/Gaussian/NeRF ready — expand as needed).
3. Generates `walkthrough.html`: familiar interactive viewer where you click room thumbnails to jump, full-screen view, easy navigation. No learning curve.

## Expansion for full Gaussian/NeRF
- Photos land in `photos/`
- Run COLMAP or `ns-train` on them for true 3D splat.
- HF models available via `huggingface_hub` for texture fill or upscaling.

Public, unlimited. Drop any property URL and it produces the tour.
