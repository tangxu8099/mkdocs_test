# Installation Guide

Welcome to the installation guide for `compas_torch_fofin`. To ensure a smooth installation process, please follow the steps below.

---

## Prerequisites

`compas_torch_fofin` requires the following dependencies:

- **PyTorch**
- **DGL (Deep Graph Library)**

!!! warning Important Note on Dependencies
    Both PyTorch and DGL require specific configurations depending on your system (e.g., CUDA version if you have a GPU). As a result, these cannot be automatically installed as part of the package dependencies and must be installed manually.

---

## Installation Steps

### 1. (Optional, Recommended) Create a Virtual Environment
To avoid conflicts with other Python packages and to maintain a clean working environment, we highly recommend creating a new Python virtual environment.

For instance, with Conda:
```bash
conda create -n compas_torch_fofin_env python=3.9
conda activate compas_torch_fofin_env
conda install pip
```

### 2. Install PyTorch

Visit the [PyTorch Installation Guide](https://pytorch.org/get-started/previous-versions/#v230) to find the correct command for your system. We recommend **PyTorch 2.3.0** (newer versions will require installing DGL from source).

For example, if using CUDA 11.8:

```bash
pip install torch==2.3.0+cu118 torchvision==0.15.0+cu118 torchaudio==2.3.0+cu118 -f https://download.pytorch.org/whl/torch_stable.html
```

### 3. Install DGL

Install the **latest pip-installable version** of DGL (**2.2.1**) using the following command:

```bash
pip install dgl==2.2.1
```

!!! info "Alternative: Install from Source"
    Optionally, to use newer versions of DGL (or PyTorch), you must build it from source. Follow the instructions in the [DGL Installation Guide](https://docs.dgl.ai/install/index.html#install-from-source) for detailed steps.

### 4. Install `compas_torch_fofin`

Install the `compas_torch_fofin` package via pip:

```bash
pip install compas_torch_fofin
```

### 5. Verify the Installation

To verify the installation, open Python and run the following:

```python
import compas_torch_fofin
```

If no errors occur you have succesfully installed `compas_torch_fofin`.
