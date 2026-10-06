# Adjoints and Backprop

**Read it here: https://dbcav.github.io/adjoint_backprop/**

A four-part series of interactive notebooks on adjoint methods, backpropagation, and why
they turn out to be the same algorithm. Everything is implemented from scratch in NumPy
(no autodiff libraries), and each notebook can be run in the browser or on Colab.

| Part | Topic |
|---|---|
| 1. What is an adjoint method? | Computing gradients through a simulation, using a projectile as the example |
| 2. What is backpropagation? | Training a small network with hand-written backprop |
| 3. Backpropagation is an adjoint method | Deriving backprop from the Lagrangian; ResNets and neural ODEs |
| 4. Gradient descent is a time stepper | Nonlinear splitting of the gradient (Levenberg–Marquardt) and of the constraint (an implicit layer trained with one solver iteration per step) |

My research is on gradient-based adjoint optimization for physics problems, and multi-agent systems. Part 4
demonstrates ideas from [Nonlinear splitting for gradient-based unconstrained and adjoint
optimization](https://doi.org/10.48550/arXiv.2508.20280)  (which applied them to neutron
transport) on small neural networks.

## Repository layout

| Path | What it is |
|---|---|
| `notebooks/` | The notebooks. The site shows whatever outputs are saved in them. |
| `index.md` | The landing page. |
| `myst.yml` | Site configuration: title, author, and page order. |
| `.github/workflows/deploy.yml` | Builds the site and deploys it to GitHub Pages on every push to `main`. |
| `requirements.txt` | The Python packages the notebooks use, for running them locally. |

