# Sky at Brio 3D Walkthroughs

Generate full 3D walkthroughs of Sky at Brio apartments (all floorplans) from public still photos only.

## Goals
- Collect public images from skyatbrio-apts.com, Yelp, Apartments.com, etc.
- Process via photogrammetry (COLMAP) or Gaussian splatting (NeRF models)
- Output navigable 3D models per unit type: Crimson (1BR 715sqft), Turquoise (2BR 1025sqft), Saffron (~978sqft), plus amenities.

## Setup
```bash
git clone https://github.com/Sharplifee/sky-at-brio-3d-walkthrough.git
cd sky-at-brio-3d-walkthrough
pip install -r requirements.txt
```

## Tools
- COLMAP for photogrammetry
- Nerfstudio / Gaussian Splatting for neural reconstruction
- Hugging Face models for gap-filling and texture synthesis
- Polycam/Luma AI integration notes

## Floorplans
- Crimson: 1 BD / 1 BA / 715 sqft
- Turquoise: 2 BD / 2 BA / 1025 sqft
- Saffron: 2 BD / 2 BA / ~978 sqft

Public stills only. No on-site capture.