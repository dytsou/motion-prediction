---
marp: true
theme: default
paginate: true
backgroundColor: white
---

# Attention-Based Traffic Scene Understanding for Autonomous Vehicles

**Group E2**

---

### Objective:

Develop a comprehensive framework for traffic scene understanding using camera data only

### Workflow:
```
┌───────────────┐    ┌─────────────────┐    ┌─────────────────┐    ┌────────────────┐
│ Feature       │    │ Attention-Based │    │ Scene Layout &  │    │ Scene          │
│ Extraction    │ -> │ Segmentation    │ -> │ Object Detection│ -> │ Understanding  │
└───────────────┘    └─────────────────┘    └─────────────────┘    └────────────────┘
```

### Key Components:
- Camera-based semantic scene understanding
- Road and lane detection with precise boundaries
- Traffic participant detection and tracking
- Overall scene topology interpretation

---

### Technical Approach

- **Convolutional Attention Module**: Spatial awareness similar to [ABSSNet](https://ieeexplore.ieee.org/document/8709818)
- **Spatial CNN**: Enhanced spatial relationship modeling through SCNN architecture
- **Multi-cue Visual Integration**: Combining vanishing points, semantic labels, and tracklets
- **Patch-wise Classification**: Two-stage architecture for efficient segmentation

### Datasets:

- [L5Kit Dataset by Woven Planet](https://woven-planet.github.io/l5kit/)

---


### Evaluation Metrics:

- Segmentation accuracy (IoU, F1-score)
- Object detection performance (mAP)
- Feature importance through ablation studies

### Expected Outcomes

- Interactive system showing real-time scene understanding:
  - Road / lane detection
  - Object tracking
  - Scene topology visualization
- Comparison across diverse traffic scenarios
