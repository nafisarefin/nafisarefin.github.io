---
title: "Aerodynamic Coefficient Prediction for the Cirrus SR22 via Open-Source CFD"
weight: 60
thumb: "/projects/aircraft/project6c.png"
summary: "Open-source CFD with advanced transition turbulence modeling to predict lift/drag for the Cirrus SR22."
figures:
  - src: "/projects/aircraft/project6a.png"
    style: "width: 225%; max-width: 375px;"
  - src: "/projects/aircraft/project6b.png"
    style: "width: 200%; max-width: 400px;"
  - src: "/projects/aircraft/project6c.png"
    style: "width: 200%; max-width: 400px;"
  - src: "/projects/aircraft/project6d.png"
    style: "width: 200%; max-width: 400px;"
---

This study investigates the aerodynamic behavior of the Cirrus SR22 light aircraft through CFD simulations using open-source tools. The primary aim was to estimate the coefficient of lift and drag under cruise conditions while validating the results against existing experimental and computational data.

A full watertight geometry of the aircraft was developed in OpenVSP using authentic design dimensions. This model was meshed using cfMesh and simulated in OpenFOAM employing the k-kL-ω SST turbulence model, a laminar-kinetic-energy-based transition model capable of capturing boundary-layer effects with high accuracy.

This project demonstrates strong proficiency in CAD geometry creation, open-source mesh generation, turbulence model selection, boundary condition specification, solver control setup, and post-processing using ParaView and Gnuplot. Mesh refinement studies and convergence analysis were carried out to ensure simulation robustness.

Results showed that the computed coefficient of drag (0.01876) and lift (1.97102) closely matched published benchmarks (Hardie, 2006; Harloff & Gary, 2014), with an error margin within 8.5%. Advanced flow visualizations including q-criterion, vorticity, and streamlines were also generated to understand complex wake behavior and flow separation zones.
