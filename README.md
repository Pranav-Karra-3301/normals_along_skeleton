# normals_along_skeleton

[![NumPy](https://img.shields.io/badge/-NumPy-blue?logo=numpy)](https://numpy.org/)
[![scikit-image](https://img.shields.io/badge/-scikit--image-orange)](https://scikit-image.org/)
[![Plotly](https://img.shields.io/badge/-Plotly-orange?logo=plotly)](https://plotly.com/)

Extract the medial skeleton of a 3D volume and compute surface normals along that skeleton. The notebook loads a NIFTI volume, skeletonizes the binary structure, estimates a normal direction at each skeleton point from the local gradient field, and renders the skeleton with its normal vectors as an interactive 3D plot.

**Live demo:** [normals-along-skeleton.vercel.app](https://normals-along-skeleton.vercel.app)

## What is here

- **extractNormals.ipynb** — loads the volume, runs `skeletonize`, smooths with a Gaussian filter, computes normals along the skeleton, and visualizes the result with Plotly.
- **index.html** — the exported interactive Plotly figure (deployed at the link above).

## Getting started

1. Clone the repository:
   ```bash
   git clone https://github.com/Pranav-Karra-3301/normals_along_skeleton.git
   cd normals_along_skeleton
   ```
2. Install the dependencies:
   ```bash
   pip install numpy scipy nibabel scikit-image plotly
   ```
3. Open `extractNormals.ipynb` in Jupyter and run the cells.

---

Built by [Pranav Karra](https://pranavkarra.me).
