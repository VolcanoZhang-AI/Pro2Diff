<h1 style="text-align: center">Pro2Diff: Proposal Propagation for Multi-Object Tracking via the Diffusion</h1>

This repository is an official implementation of [Pro2Diff](https://ieeexplore.ieee.org/document/10753449).

# Abstract
Multi-object tracking (MOT) aims to estimate the bounding boxes and ID labels of objects in videos. The challenging issue in this task is to alleviate competitive learning between the detection and tracking subtasks, for which, two-stage Tracking-By-Detection (TBD) optimizes the two subtasks individually, and the single-stage Joint Detection and Tracking (JDT) adjusts the complex network architectures finely in an end-to-end pipeline. In this paper, we propose a new MOT method, i.e., Proposal Propagation via Diffusion Models, called Pro2Diff, which integrates a diffusion model into the proposal propagation in multi-object tracking, focusing on the model training process rather than complex network design. Specifically, using a generative approach, Pro2Diff generates a considerable number of noisy proposals for the tracking image sequence in the forward process, and subsequently, Pro2Diff learns the discrepancies between these noisy proposals and the actual bounding boxes of the tracked objects, gradually optimizing these noisy proposals to obtain the initial sequence of real tracked objects. By introducing the denoising diffusion process into multi-object tracking, we have made three further important findings: 1) Generative methods can effectively handle multi-object tracking tasks; 2) Without the need to modify the model structure, we propose self-conditional proposal propagation to enhance model performance effectively during inference; 3) By adjusting the numbers of proposals and iterations appropriately for different tracking sequences, the optimal performance of the model can be achieved. Extensive experimental results on MOT17 and DanceTrack datasets demonstrate that Pro2Diff outperforms current end-to-end multi-object tracking methods. We achieve 61.9 HOTA on DanceTrack and 57.6 HOTA on MOT17, reaching the competitive result of the JDT approach.

<p align="center">
  <img src="assets/overview.png" width="800">
</p>

# News

* Code will be released soon.