---
title: "Deep-Learning Segmentation Uncertainty in Coronary FFR-CT Digital Twins"
weight: 5
summary: "Deep-learning CTA segmentation with uncertainty quantification to sharpen patient-specific FFR-CT prediction for coronary artery disease. (AHA postdoctoral fellowship proposal)"
pub: 'N. Arefin, C. Georgiadis, M. Usman, A. Narayan, L. Timmins. Quantifying Deep Learning Segmentation-Driven Geometric Uncertainty in Coronary FFR-CT Predictions. Annals of Biomedical Engineering <em>(in preparation)</em>.'
pub: 'M. Usman, N. Arefin, A. Narayan, L. Timmins. Geometric Uncertainty Quantification in Vascular Biomechanics. Journal of Biomechanics <em>(in preparation)</em>.'
---

Non-invasive FFR-CT lets clinicians judge whether a narrowing in a coronary artery actually restricts blood flow, directly from a CT angiogram, without an invasive catheter procedure. But the accuracy of that prediction depends heavily on how precisely the artery is reconstructed from the images, and that reconstruction step is a major, under-quantified source of error. This project, part of my American Heart Association (AHA)-funded postdoctoral work, builds an image-based digital-twin pipeline that makes this uncertainty explicit.

Deep-learning models are trained to segment the coronary arteries from CT angiography, producing patient-specific 3D lumen geometries. Rather than trusting a single segmentation as ground truth, the framework characterizes the geometric variability across plausible segmentations and propagates it through computational blood-flow models to quantify how much the resulting FFR-CT value can shift. Coupled 3D–0D reduced-order models with Windkessel (RCR) boundary conditions keep the simulations efficient enough for patient-specific use.

The work brings together deep-learning image segmentation, patient-specific CFD, reduced-order modeling, and uncertainty quantification, in direct collaboration with clinicians and using high-resolution photon-counting CT data. The goal is a digital-twin workflow that not only predicts FFR-CT but also reports how confident that prediction is — information that is essential before such tools can responsibly guide treatment decisions for coronary artery disease.
