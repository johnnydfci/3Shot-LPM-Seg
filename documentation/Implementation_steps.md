# **SAM2 Model for Lumbar Paraspinal Muscle Segmentation**

This repository implements **SAM2** for **lumbar paraspinal muscle segmentation** using **Linux (Ubuntu 18.04)** with an **RTX 3060 GPU (12GB VRAM)**. The implementation is based on [Facebook Research's SAM2 repository](https://github.com/facebookresearch/sam2).

---

## **Environment Setup**

Before using SAM2, ensure that Python and PyTorch are installed. The model requires:

- **Python**: `>=3.10`
- **PyTorch**: `>=2.5.1`
- **Torchvision**: `>=0.20.1`

### **Installation Steps**
```bash
# Step 1: Create and activate the conda environment
conda create -n sam2 python=3.10
conda activate sam2

# Step 2: Install Jupyter Notebook
conda install notebook>=5.3 jupyter_server

# Step 3: Install PyTorch and dependencies
conda install pytorch==2.3.1 torchvision==0.18.1 torchaudio==2.3.1 pytorch-cuda=11.8 -c pytorch -c nvidia

# Step 4: Clone the SAM2 repository
git clone https://github.com/facebookresearch/sam2.git && cd sam2

# Step 5: Install required packages
pip3 install -r requirements.txt
```

To **remove** the environment if needed:
```bash
conda remove -n sam2 --all
```

---

## **Data Download**
Download the dataset and place the files in the following directories:

```
notebook/videos/MRI515_T1
notebook/videos/MRI515_T2
```

---
