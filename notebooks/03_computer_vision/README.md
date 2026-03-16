# Computer Vision Notebooks

This folder contains higher-level PyTorch notebooks that build on the fundamentals and data-loading sections.

## Included notebook

- `simple_vision_end_to_end.ipynb`: a compact CNN example that loads MNIST, trains on a small subset, and inspects predictions.
- `transfer_learning.ipynb`: fine-tuning a pretrained torchvision model on your own dataset.

## When to use this folder

Come here after you are comfortable with:

- tensors,
- autograd,
- the training loop,
- and basic dataset/data-loader patterns.

## Practical tip

`transfer_learning.ipynb` is more resource-heavy than `nn_end_to_end.ipynb`, so Colab can be a good fit if your local machine feels slow.

If you want a faster CPU-friendly starting point, begin with `simple_vision_end_to_end.ipynb` first.
