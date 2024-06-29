# Brief Description of Codes

This folder contains the programming bases used during the experimental analysis of this thesis. They are organized into two subfolders:

## Folder: Comparison of Depth-Width Impact & SeBlock

This folder includes the `.IPYNB` files `experiments-cifar-fs` and `experiments-fc-100`. These are the base codes used in the first two comparisons (Comparison of Depth Impact & Comparison of Width Impact and SE-block inclusion in the network). Essentially, it is the same programming base separated into two different Notebooks (one for each dataset) for ease of implementation.

## Folder: Comparison of Self-Supervision Impact (VAE)

This folder contains the two `.IPYNB` files `vae-resnet18-softmax-rotation` and `vae-resnet18-selfsupervision`. These are the base codes used in the third comparison, which examines the impact of auxiliary self-supervised processes using VAE. In this case, for ease of implementation, the separation was made into two Notebooks:

- `vae-resnet18-softmax-rotation`: for experiments that either do not include any auxiliary process or include the auxiliary self-supervised rotation process (Generation-0 Algorithm).
- `vae-resnet18-selfsupervision`: which served as the programming base for the study and exact implementation when the auxiliary self-supervised learning process using VAE was utilized.

Descriptions with the exact characteristics of the experiments can be found in the main text of this thesis (`Thesis.pdf`), from which appropriate modifications can be derived to verify the experimental results presented.
