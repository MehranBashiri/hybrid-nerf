# Neural Radiance Field (NeRF) for 3D Scene Reconstruction

## Overview
**Neural Radiance Field (NeRF)** is a framework for synthesizing novel views of 3D scenes by representing them as continuous volumetric functions. This project implements a streamlined version of NeRF using PyTorch3D to simplify computational requirements while maintaining high-quality rendering capabilities. The models and experiments are provided in a Jupyter Notebook and can be run online or locally.

## Running the Code

The project is implemented in a Jupyter Notebook (`notebook.ipynb`), which can be executed in:

### Google Colab
1. Upload the `notebook.ipynb` to [Google Colab](https://colab.research.google.com/).
2. Follow the prompts in the notebook to install required dependencies.
3. Execute the cells sequentially to train and evaluate the models.

### Local Setup
1. Clone the repository:
    ```bash
    git clone https://github.com/your-username/repository-name.git
    ```
2. Navigate to the project directory:
    ```bash
    cd repository-name
    ```
3. Open the Jupyter Notebook locally:
    ```bash
    jupyter notebook notebook.ipynb
    ```
4. Install required dependencies as specified in the notebook's initial cells.

## Dataset

### Clean Cow Dataset
The clean cow dataset includes rendered views of a 3D cow model with simple, uncluttered backgrounds and binary silhouettes. It provides an idealized baseline for testing Neural Radiance Fields (NeRF) models.

### Complex Noisy Cow Dataset
To evaluate the robustness of the models, the complex noisy cow dataset introduces challenges such as:
- Gaussian noise and salt-and-pepper noise.
- Visual complexities like motion blur, background changes, and color jittering.

These datasets are automatically downloaded and prepared during notebook execution.

## Results
The performance of various models is evaluated using the following metrics:
- **PSNR (Peak Signal-to-Noise Ratio):** Measures pixel-level fidelity.
- **SSIM (Structural Similarity Index):** Evaluates structural and perceptual similarity.
- **LPIPS (Learned Perceptual Image Patch Similarity):** Assesses perceptual similarity based on learned features.

Comprehensive results are documented in the notebook, including visualizations of reconstructed scenes and quantitative comparisons.

