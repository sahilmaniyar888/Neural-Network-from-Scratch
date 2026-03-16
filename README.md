# Neural Network from Scratch

A notebook-first PyTorch learning repo that moves from tensor basics and manual training loops to data pipelines, computer vision, transfer learning, and SFT batching concepts.

## Project goals

- learn core PyTorch operations from first principles,
- understand how `nn.Module`, loss functions, and optimizers fit together,
- practice real data loading workflows,
- build at least one end-to-end vision model,
- and connect the basics to more advanced topics such as transfer learning and supervised fine-tuning.

## Repository structure

```text
.
|-- notebooks/
|   |-- README.md
|   |-- 01_fundamentals/
|   |   |-- README.md
|   |   |-- 01_pytorch_basics_and_training_loop.ipynb
|   |   `-- 02_sft_batch_preparation.ipynb
|   |-- 02_data_loading/
|   |   |-- README.md
|   |   |-- 01_dataset_preparation_and_loading.ipynb
|   |   `-- 02_pytorch_dataloader_workflow.ipynb
|   `-- 03_computer_vision/
|       |-- README.md
|       |-- 01_mnist_cnn_end_to_end.ipynb
|       `-- 02_transfer_learning_with_alexnet.ipynb
|-- src/
|   `-- neural_network_from_scratch/
|       |-- __init__.py
|       `-- cli.py
|-- pyproject.toml
`-- README.md
```

## Learning path

1. `notebooks/01_fundamentals/01_pytorch_basics_and_training_loop.ipynb`
2. `notebooks/01_fundamentals/02_sft_batch_preparation.ipynb`
3. `notebooks/02_data_loading/01_dataset_preparation_and_loading.ipynb`
4. `notebooks/02_data_loading/02_pytorch_dataloader_workflow.ipynb`
5. `notebooks/03_computer_vision/01_mnist_cnn_end_to_end.ipynb`
6. `notebooks/03_computer_vision/02_transfer_learning_with_alexnet.ipynb`

## Setup

Recommended local setup on Windows with Python 3.12:

```powershell
uv venv .venv312 --python 3.12
.\.venv312\Scripts\activate
uv pip install -e ".[dev]"
python -m ipykernel install --user --name nn-scratch-312 --display-name "Neural Network Scratch (3.12)"
```

Then open the notebooks and select the `Neural Network Scratch (3.12)` kernel.

## Notes

- The project is designed to run well on CPU for most notebooks.
- `notebooks/02_data_loading/02_pytorch_dataloader_workflow.ipynb` downloads `helper_functions.py` on demand if it is missing.
- `notebooks/03_computer_vision/01_mnist_cnn_end_to_end.ipynb` is the best computer-vision starting point if you want a fast local run.
- `notebooks/03_computer_vision/02_transfer_learning_with_alexnet.ipynb` is more resource-heavy and is a good Colab candidate.

## Quick start

If you want the fastest route through the project, start with:

1. `notebooks/01_fundamentals/01_pytorch_basics_and_training_loop.ipynb`
2. `notebooks/03_computer_vision/01_mnist_cnn_end_to_end.ipynb`
3. `notebooks/03_computer_vision/02_transfer_learning_with_alexnet.ipynb`
