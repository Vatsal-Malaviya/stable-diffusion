# Installation

## Requirements

- Python 3.8+
- CUDA capable GPU
- 40GB+ GPU memory for full model

## Quick Setup

```bash
# Clone repository
git clone https://github.com/Vatsal-Malaviya/stable-diffusion.git
cd stable-diffusion

# Install dependencies
pip install -r requirements/base.txt

# Optional: Install development dependencies
pip install -r requirements/dev.txt
```

## Docker Setup

```bash
# Build image
docker build -t diffusion-models .

# Run container
docker run --gpus all -it diffusion-models
```

## Verify Installation

```bash
# Run tests
pytest tests/

# Train mini model
python scripts/train.py --config configs/mini.yaml
```
