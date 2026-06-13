# Evaluations

Architecture-review site for the registration/measurement pipeline: what failed during the
June 5 pilot, what we changed, and the batch-evaluation evidence behind each change.

## Viewing

Open `index.html` directly in a browser — no server needed.

The hero 3D viewer loads real scan-derived point cloud data from `assets/clouds.js` /
`assets/clouds.json`. Those files are **not committed** (scan data stays off GitHub) and are
shared separately — drop both into `assets/` and the viewer works. Without them the rest of
the page (summary, failure-mode sections, evaluation renders) still displays.

## Contents

- `index.html` — the site
- `assets/eval_*.png` — batch-evaluator renders backing the claims on the page
  (flipped-pose incident, wrong-STEP block, known-good pass, recovered pass)
- `assets/three.min.js` — Three.js, vendored for offline use
- `assets/clouds.js` / `assets/clouds.json` — gitignored point cloud data (see above)
