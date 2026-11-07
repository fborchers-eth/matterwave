# Condensate Interference Bench

An interactive browser simulator of matter-wave interference between Bose–Einstein condensates, made for teaching.

**Open it:** https://&lt;user&gt;.github.io/matterwave/

You can cut a trapped 2D condensate with light-sheet barriers and give each part its own phase. Then you choose a temperature and density, release the cloud or merge the parts in the trap, and watch the fringes form. Guided experiments follow:

1. Andrews et al., *Science* 275, 637 (1997): two condensates that interfere
2. Javanainen & Yoo, *PRL* 76, 161 (1996), and Castin & Dalibard, *PRA* 55, 4330 (1997): random relative phase and atom detection
3. Loss of contrast with temperature
4. Phase drift between parts of unequal size during a hold
5. Scherer et al., *PRL* 98, 110402 (2007): vortices from merging three condensates

## How it works

- 2D Gross–Pitaevskii equation, split-step Fourier method, units ħ = m = ω = 1.
- Everything runs in the student's browser. The page is one static file (`index.html`) and needs no server-side code.
- The temperature model is simple: condensate fraction 1 − (T/Tc)³, a non-interfering thermal Gaussian, and a phase-noise field.

## Run locally

Open `index.html` in a browser, or run `python3 -m http.server` and go to http://localhost:8000.
