# Agent Experiments

## Developer notes

### Setting up a conda environment to run experiments

To install a base conda environment with pytorch (gpu supported):
```bash
conda create -n agent-experiments python=3 ipykernel
conda activate agent-experiments
conda install numpy pytorch pytorch-cuda=12.4 -c pytorch -c nvidia
```

Dependencies required to set up inference and fine tuning for phi models:
```bash
pip install transformers datasets ipywidgets peft trl huggingface_hub flash_attn bitsandbytes accelerate
```