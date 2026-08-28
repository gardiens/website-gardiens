---
date: 20-11-2025

title: EOGS++ Earth Observation Gaussian Splatting for Satellite 3D Reconstruction

tags: ["3D Reconstruction", "Satellite Imagery", "Gaussian Splatting", "Remote Sensing"]

stags: ["3D Reconstruction", "Gaussian Splatting", "Earth Observation"]

links: ["https://github.com/gardiens/EOGS2", "https://gardiens.github.io/EOGS2/"]

linksDescription: ["Github repo", "Project webpage"]

image: "eogs2.png"

---

## Abstract

We present EOGS++, an extension of Earth Observation Gaussian Splatting for accurate and efficient 3D reconstruction from satellite imagery.

Recent advances in 3D Gaussian Splatting have enabled fast novel view synthesis and 3D reconstruction, but their application to satellite imagery remains challenging due to inaccurate camera parameters and the complexity of remote sensing data. EOGS++ addresses these limitations by directly operating on raw high-resolution panchromatic satellite images, removing the need for external preprocessing such as pansharpening.

The proposed framework integrates internal camera refinement based on optical flow, enabling bundle adjustment directly during training without relying on external optimization tools. Additional improvements, including opacity reset, early stopping, and TSDF-based post-processing, improve reconstruction sharpness and geometric consistency.

Experiments on the IARPA 2016 and DFC2019 satellite datasets demonstrate improved reconstruction quality and efficiency compared to previous Gaussian Splatting and NeRF-based approaches. The method achieves a reduction of the building reconstruction MAE from 1.33 m to 1.19 m compared to the original EOGS framework.

This work was published at **ISPRS 2026**.

## Method