# testhero — clawSW Industrial Temple (HERO3D experiment)

Sandbox experiment for **Sanjay Wood Tech / clawSW**.  
**Does not touch** the production Hero3D in the main clawSW repo.

## Quick start

```bash
git clone https://github.com/sanjaymaverick-cmd/testhero.git
cd testhero
python3 -m http.server 8765
```

Open [http://127.0.0.1:8765/machine-hero.html](http://127.0.0.1:8765/machine-hero.html)

## Files

| File | Role |
|------|------|
| `machine-hero.html` | Industrial Temple hero (Three.js + meshopt machine) |
| `machine-hero-app.js` | Scene logic (loaded by the HTML) |
| `precision-cut-core.html` | Earlier timber-core prototype |
| `public/models/machine.glb` | Meshopt-compressed Tripo machine mesh (~4.2 MB) |

## Full assets

Complete experiment sources also live in the Grok artifacts sandbox:

`clawsw-hero3d-experiment/machine-hero.html` + `public/models/machine.glb`

To push the full binary GLB and latest HTML from a local copy of that folder:

```bash
cp machine-hero.html precision-cut-core.html /path/to/testhero/
mkdir -p /path/to/testhero/public/models
cp public/models/machine.glb /path/to/testhero/public/models/
cd /path/to/testhero
git add -A && git commit -m "Sync full Industrial Temple experiment" && git push
```

## Creative brief (summary)

- Stream of timber along the machine bed (photo-matched feed)
- Scroll stages: Infeed → Cut → Kerf → Outfeed → Mortise/tenon → Chair form
- Grammar: factory rhythm + temple gravity; joinery as kept promises
