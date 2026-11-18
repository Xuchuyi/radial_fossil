Figure scripts and data for the paper "The Connection between Halo Assembly History and the Stellar Distribution II: A Radially Stratified Fossil Record of Past Halo Mass" by Shuo Xu, Song Huang, Conghao Zhou, Alexie Leauthaud, Benedikt Diemer.
arxiv: https://arxiv.org/abs/2611.12470

## Contents

- `FigureNotebooks/`: Jupyter notebooks that produce each figure in the paper. Each notebook is named after the figure it generates:
- `Fig1new.ipynb`: Figure 1
- `Fig2.ipynb` to `Fig4.ipynb`: Figures 2 to 4
- `FigA.ipynb`, `FigA2.ipynb`: Appendix figures

Each notebook can be run top to bottom to reproduce the corresponding figure. Paths in the notebooks are relative to the `FigureNotebooks/` directory.

- `Data/`: data products used by the notebooks. These are derived from the IllustrisTNG-300 hydrodynamical simulation: a halo-mass-complete sample of the top 3388 massive central galaxies at z = 0.4 (snapshot 72), including merger-tree histories (mass accretion histories, progenitor halo masses, stellar mass histories), stellar masses in annular apertures over a range of galactocentric radii, halo positions, richness and satellite mass measurements, and a redshift-snapshot-age mapping of the simulation.
- Also included are precomputed catalogs of the top 3500 most massive halos at every snapshot from 25 to 71 (z = 3 to z = 0.4), with halo IDs and masses, which are used to compute the rank retention fraction, as well as a table of fossil-correlation peak redshifts.
- `Fig3.ipynb` reads a file that are not included in this repository: an ex-situ mass decomposition table provided by collaborators. Interested readers can contact the authors for access. The notebook expects these files in a sibling `external_data/` directory.

## Requirements:

Python 3 with the following packages: numpy, matplotlib, scipy, astropy, pandas, palettable. One notebook has an additional dependency: `Fig2.ipynb` requires pingouin.
## License

The code in this repository is released under the MIT License (see `LICENSE`). The data products are derived from IllustrisTNG and remain subject to its data policy.
