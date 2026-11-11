# UPC_HF_study
# Heavy-flavour jets in ultra-peripheral Pb+Pb collisions 

Nihal Gozlukluoglu, California State University, Northridge (November 2026)

## What the project does
In ultra-peripheral collisions (UPCs), electromagnetic interactions dominate, and hadronic interactions are strongly suppressed. This makes UPCs a clean environment for processes such as nuclear photoproduction. In this study,y we focus on photon–nucleus (γ+A) interactions, which can be used to study nuclear parton distribution functions (nPDFs).

One nucleus emits a photon, and the photon hits a gluon in the other nucleus: γ g → c c̄ or b b̄. The two heavy-flavour jets give the gluon momentum fraction xA. Comparing a nuclear PDF (EPS09) with free protons and neutrons shows the nuclear effect on the gluon.


The chain:

1. **Step 1**: Pythia 8 makes photon + Pb events, and we check them against ATLAS (PRD 111, 052006).
2. **Step 2**: Every jet gets a label (b, c, or light) and an origin (how the heavy quark was made).
3. **Step 3**: selects the γ g → Q Q̄ signal (two heavy-flavour jets, xγ > 0.70).
4. **Step 4**: adds nucleus survival, tagging and luminosity, then estimates the expected precision.
5. **Step 5**: does the same at detector level with Delphes, plus a track-based tagger for ATLAS-like and EIC trackers.



## What is needed

Pythia 8.310, FastJet 3, ROOT 6, and Delphes 3 (only for Step 5). `pythia8-config`,
`fastjet-config` and `root-config` must be in your PATH.

## Compile

```
make
