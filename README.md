# Workshop Setup Instructions

Welcome to the Intro to ML Workshop! Please follow the instructions below to get your environment ready.

## 1. Clone the Repository

First, clone the workshop repository to your working directory:

```bash
git clone https://github.com/abhi-mal/intro_ml_workshop.git 
cd intro_ml_workshop
```

## 2. Environment Setup

Choose **one** of the following options to set up your Python environment:

### Option A: Standard Installation (Recommended)

Build the environment from the provided configuration file. This ensures package integrity and allows you to customize the environment later if needed.

```bash
conda env create -f environment.yml -n intro_ml
```

**Don't have Conda installed?**
If you are on Linux, you can quickly install Miniconda by running:

```bash
wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
bash Miniconda3-latest-Linux-x86_64.sh -b -p $HOME/miniconda3
~/miniconda3/bin/conda init bash
```
*Note: After running the above commands, please quit your terminal and open a new one before continuing.*

### Option B: Fast Track (Shared Environment)

If you want to skip the installation and jump straight to the exercises, you can directly activate a pre-built shared environment:

```bash
source /data/mallampalli/miniconda3/bin/activate /data/mallampalli/miniconda3/envs/intro_ml
```

> **Note:** In general, it is always safer to build environments from a `yaml` file yourself to verify package integrity. For this hackathon, feel free to use this shared build to save time!

## 3. Activate and Configure Jupyter

Once your environment is set up (via either Option A or B), ensure it is activated and install the Jupyter kernel so you can run the workshop notebooks:

```bash
# Activate the environment (Required if you used Option A)
conda activate intro_ml

# Install the Jupyter kernel
python -m ipykernel install --user --name intro_ml --display-name "Python (intro_ml)"
```

You are now ready to launch your Jupyter server and begin the exercises!
