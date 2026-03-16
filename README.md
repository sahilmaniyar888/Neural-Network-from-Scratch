# Neural Network from Scratch

Notebook-first PyTorch exercises for learning how tensors, data loaders, training loops, and transfer learning fit together from first principles.

The repo is organized as a guided learning path, so the folder order matches the order you should study the material.

## Repo layout

- `notebooks/01_fundamentals/`: first-principles tensor and training-loop work.
- `notebooks/02_data_loading/`: dataset, image loading, and dataloader practice.
- `notebooks/03_computer_vision/`: transfer learning and higher-level PyTorch workflows.
- `src/neural_network_from_scratch/`: lightweight package and CLI entry point.

## Learning order

1. `notebooks/01_fundamentals/nn_end_to_end.ipynb`
2. `notebooks/02_data_loading/data_loaders.ipynb`
3. `notebooks/02_data_loading/dataloader_pytorch.ipynb`
4. `notebooks/03_computer_vision/transfer_learning.ipynb`

## Recommended setup

This repo is best used with Python 3.12 on a local CPU environment.

Why:

- `nn_end_to_end.ipynb` is small and runs comfortably on CPU.
- CPU keeps the setup simple while you are learning the training loop.
- Colab is still a good fallback for heavier image notebooks or if local installs get annoying.

## Local install

Windows PowerShell with `uv`:

```powershell
uv venv .venv312 --python 3.12
.\.venv312\Scripts\activate
uv pip install -e ".[dev]"
python -m ipykernel install --user --name neural-network-from-scratch --display-name "Neural Network from Scratch (3.12)"
```

Then open the notebooks in VS Code or Jupyter and select the `Neural Network from Scratch (3.12)` kernel.

## If you prefer Google Colab

Use Colab when:

- you want a zero-setup environment,
- you want an easy GPU option later,
- or you are working on `notebooks/03_computer_vision/transfer_learning.ipynb`.

Minimal Colab install cell:

```python
!pip install torch torchvision matplotlib numpy pillow requests tqdm
```

For `notebooks/01_fundamentals/nn_end_to_end.ipynb`, local CPU is still the cleaner choice.

## Notes

- The repo is still notebook-first, but the top-level layout is now cleaner and more standard.
- `notebooks/02_data_loading/dataloader_pytorch.ipynb` downloads `helper_functions.py` on demand if it is missing.
- If you want CUDA/GPU support locally, install PyTorch using the official selector first, then install the rest of the repo dependencies.

## Project structure

```text
.
|-- notebooks/
|   |-- README.md
|   |-- 01_fundamentals/
|   |   `-- nn_end_to_end.ipynb
|   |-- 02_data_loading/
|   |   |-- data_loaders.ipynb
|   |   `-- dataloader_pytorch.ipynb
|   `-- 03_computer_vision/
|       |-- README.md
|       `-- transfer_learning.ipynb
|-- src/
|   `-- neural_network_from_scratch/
|       |-- __init__.py
|       `-- cli.py
|-- pyproject.toml
`-- README.md
```

## Quick start

1. Start with `notebooks/01_fundamentals/nn_end_to_end.ipynb`.
2. Move to `notebooks/02_data_loading/` once the tensor and training-loop pieces feel comfortable.
3. Use `notebooks/03_computer_vision/transfer_learning.ipynb` when you want a more practical computer-vision example.
