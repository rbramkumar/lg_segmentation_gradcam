# LG Segmentation Grad-CAM

This repository provides Grad-CAM visualizations for a U-Net model trained to segment the lacrimal gland on MRI images. Grad-CAM (Gradient-weighted Class Activation Mapping) helps visualize which regions of an MRI image most influence the U-Net's segmentation, offering insights into model interpretability for medical imaging applications.

## Features

- **U-Net Model**: Performs lacrimal gland segmentation on MRI images.
- **Grad-CAM Visualization**: Generates heatmaps highlighting image regions important to segmentation decisions.
- **Medical Imaging Focus**: Tailored for lacrimal gland segmentation in orbital MRI datasets.
- **Modular & Extendable**: Easily adapt to your own models and MRI datasets.

## Table of Contents

- [Usage](#usage)
- [Examples](#examples)
- [Project Structure](#project-structure)
- [Contributing](#contributing)
- [License](#license)
- [References](#references)

## Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/rbramkumar/lg_segmentation_gradcam.git
   cd lg_segmentation_gradcam
   ```


## Usage

1. **Prepare your model and data**
   - Place your trained U-Net model weights in the `models/` directory.
   - Add MRI images for testing in the `data/` folder.

2. **Run Grad-CAM visualization**
   - Run the code cells in the jupyter notebook with the input images and models replaced
     
3. **View results**
   - Visualizations are saved in the main directory.

## Examples

Example output of Grad-CAM on an orbital MRI:

| MRI Slice | Segmentation Mask | Grad-CAM Overlay |
|-----------|------------------|------------------|
| ![input](examples/input.png) | ![mask](examples/mask.png) | ![gradcam](examples/gradcam.png) |

## Project Structure

```
lg_segmentation_gradcam/
│
├── 03_lg_segmentation_grad_cam.ipynb # Main script for visualization
├── Grad CAM Visualization.png                 # Utility functions
├── layers.txt
└── README.md
```

## Contributing

Contributions are welcome! Please open issues or pull requests.

## License

This project is licensed under the MIT License.

## References

- Selvaraju, R.R., et al. "Grad-CAM: Visual Explanations from Deep Networks via Gradient-based Localization." ICCV, 2017.
- Ronneberger, O., et al. "U-Net: Convolutional Networks for Biomedical Image Segmentation." MICCAI, 2015.
- Jacob Gil, pytorch-grad-cam (https://github.com/jacobgil/pytorch-grad-cam)

---

**Contact:**  
For questions or support, please open an issue or reach out to [rbramkumar](https://github.com/rbramkumar).
