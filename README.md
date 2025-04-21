# Modified Swin UNETR using MONAI

This repository contains a modified version of the `SwinUNETR` model from [MONAI](https://monai.io/), a PyTorch-based framework for deep learning in healthcare imaging. This modification was made to adapt the original Swin UNETR architecture for task-specific segmentation requirements.

---

## ✅ Overview

The Swin UNETR architecture combines the power of Swin Transformers with a U-Net-like encoder-decoder design for 3D medical image segmentation. In this repository, the official MONAI version has been partially customized to suit our task (e.g., number of classes, input shape, attention tuning, or decoding depth).

---

## 📦 Environment Setup

We recommend using a clean Python virtual environment. The following packages are required:

- Python ≥ 3.8  
- PyTorch ≥ 1.10  
- MONAI ≥ 1.2.0  
- Torchvision, nibabel, numpy, matplotlib, etc.

### Step-by-step installation:

```bash
# 1. Create and activate a virtual environment (optional but recommended)
python -m venv venv
source venv/bin/activate  # or use venv\\Scripts\\activate on Windows

# 2. Install PyTorch with CUDA support (adjust CUDA version if needed)
pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu117

# 3. Install MONAI
pip install monai

# 4. Install other dependencies
pip install nibabel numpy matplotlib scikit-learn tqdm
