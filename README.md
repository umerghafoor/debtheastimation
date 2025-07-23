# Depth Estimation and 3D Visualization with MiDaS and Open3D

This repository contains Python notebooks for estimating depth from a single RGB image using the MiDaS model (DPT_Large) and visualizing the results in 3D using Open3D and Matplotlib.

## Features

- **Depth Estimation**: Uses Intel ISL's MiDaS model (DPT_Large) to predict depth from a single RGB image
- **3D Point Cloud Generation**: Converts depth maps into 3D point clouds with color mapping
- **Multiple Visualization Methods**:
  - 2D depth maps
  - 3D point clouds
  - 3D grid visualizations
  - 2D projections (top-down, front, and side views)

## Requirements

- Python 3.7+
- PyTorch
- torchvision
- OpenCV
- Open3D
- Matplotlib
- NumPy

## Installation

```bash
pip install torch torchvision opencv-python open3d matplotlib numpy
```

## Usage

1. **Depth Estimation** (`main.ipynb`):
   - Load an RGB image
   - Estimate depth using MiDaS
   - Save and visualize the depth map

2. **3D Point Cloud Generation** (`depthmap.ipynb`):
   - Convert depth map to 3D point cloud
   - Visualize point cloud in 3D and 2D projections

3. **3D Grid Visualization** (`depthmap_isometric.ipynb`):
   - Create a 3D grid from depth map
   - Visualize from different angles

## Notes

- The MiDaS model requires an internet connection for the first run to download pretrained weights
- Camera intrinsics in the point cloud generation are approximate - for real applications, use calibrated values
- The 3D visualizations are best viewed interactively in Jupyter Notebook

## Acknowledgments

- Intel ISL for the MiDaS model
- Open3D development team
- PyTorch community
