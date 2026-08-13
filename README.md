# testhero — clawSW Industrial Temple (HERO3D experiment)

Sandbox experiment for **Sanjay Wood Tech / clawSW**.  
**Does not touch** the production Hero3D in the main clawSW repo.

## Run locally

```bash
# from repo root
python3 -m http.server 8765
```

Open:

- [http://127.0.0.1:8765/machine-hero.html](http://127.0.0.1:8765/machine-hero.html) — **primary** Industrial Temple hero  
- [http://127.0.0.1:8765/precision-cut-core.html](http://127.0.0.1:8765/precision-cut-core.html) — earlier timber-core experiment  

## Industrial Temple (`machine-hero.html`)

- Real machine mesh: `public/models/machine.glb` (meshopt-compressed Tripo export)
- Three.js + `MeshoptDecoder` (required for meshopt GLB)
- Timber stream along the **machine bed** (photo-matched feed path)
- Scroll stages: Infeed → Registration → Cut → Kerf → Outfeed → Joint → Assembly → Form
- Creative grammar: factory rhythm + temple gravity, mortise & tenon, dougong / Daibutsuyō / Zenshūyō as structural metaphors
- Custom PBR: gunmetal machine, wood stock, gold joint accent

## Assets

| Path | Notes |
|------|--------|
| `machine-hero.html` | Main experiment (self-contained CDN Three.js) |
| `precision-cut-core.html` | Prior prototype |
| `public/models/machine.glb` | ~4.2 MB meshopt GLB |

## Notes

- Geometry-only mesh (no materials in source); materials overridden in-scene.
- Parallel experiment only — not production clawSW website code.
