# # RepYOLOv5-SF3D

A cascaded framework for fine-grained student behavior recognition in complex classroom scenes.

## Overview

Student behavior recognition in classroom environments is important for teaching-quality assessment and intelligent education. However, it remains challenging due to dense student distributions, frequent occlusion, substantial scale variation, and the subtle nature of common classroom actions.

To address these issues, this project proposes **RepYOLOv5-SF3D**, a cascaded framework for fine-grained student behavior recognition in complex classroom scenes. The framework integrates a lightweight **RepYOLOv5m** detector with a dual-stream **SlowFast-3D** recognition branch, enabling automated inference from raw video input to behavior label output.

## Method

The proposed framework is designed to improve robustness and efficiency in dense and occluded classroom scenarios.

### Key Components

- **RepYOLOv5m detector**  
  Used as a lightweight front-end detector for student localization.

- **Dual-stream SlowFast-3D recognition branch**  
  Captures spatiotemporal behavior features from classroom video clips.

- **Decoupled training strategy**  
  Reduces the impact of localization instability on back-end spatiotemporal learning.

- **SDS3D (Spatiotemporal Depthwise-Separable 3D module)**  
  Alleviates the redundancy of conventional 3D convolutions and enhances fine-grained spatiotemporal representation.

- **NTAM (Normalization-Based Temporal Attention Mechanism)**  
  Reuses normalization scale factors to emphasize informative temporal segments without introducing additional learnable parameters.

## Features

- Fine-grained student behavior recognition in dense classroom scenes
- Improved robustness under occlusion and scale variation
- Lightweight design for efficient inference
- Reduced model size and inference latency
- Potential deployment on edge computing devices in practical classroom environments

## Experimental Results

Experimental results on real classroom datasets demonstrate that the proposed method achieves a favorable balance between **recognition accuracy** and **inference efficiency** under dense occlusion.

Compared with mainstream spatiotemporal networks, the proposed framework also shows advantages in:

- **Model size**
- **Inference latency**
- **Practical deployment efficiency**

These results indicate its potential for routine deployment on edge computing devices in real-world classroom scenarios.

## Data Availability

In accordance with the journal’s requirements, part of the dataset has been uploaded. The remaining datasets are stored on our cloud drive and are available upon request by email to **sun_ching@163.com**.

## Contact

For questions regarding the dataset or this work, please contact:

**sun_ching@163.com**
