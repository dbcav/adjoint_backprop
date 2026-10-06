# Adjoints and Backprop

This is a short series of notebooks about adjoint methods, backpropagation, and why they turn out to be the same algorithm. The last part treats the optimizer as a time stepper too, and uses that to introduce an idea from my own research.

| Part | Read | Run |
|---|---|---|
| 1. What is an adjoint method? | [Read](./notebooks/adjoints_part1.ipynb) | [In your browser](__SITE_URL__/lite/notebooks/index.html?path=adjoints_part1.ipynb) · [Colab](https://colab.research.google.com/github/__REPO__/blob/main/notebooks/adjoints_part1.ipynb) |
| 2. What is backpropagation? | [Read](./notebooks/adjoints_part2.ipynb) | [In your browser](__SITE_URL__/lite/notebooks/index.html?path=adjoints_part2.ipynb) · [Colab](https://colab.research.google.com/github/__REPO__/blob/main/notebooks/adjoints_part2.ipynb) |
| 3. Backpropagation is an adjoint method | [Read](./notebooks/adjoints_part3.ipynb) | [In your browser](__SITE_URL__/lite/notebooks/index.html?path=adjoints_part3.ipynb) · [Colab](https://colab.research.google.com/github/__REPO__/blob/main/notebooks/adjoints_part3.ipynb) |
| 4. Gradient descent is a time stepper | [Read](./notebooks/adjoints_part4.ipynb) | [In your browser](__SITE_URL__/lite/notebooks/index.html?path=adjoints_part4.ipynb) · [Colab](https://colab.research.google.com/github/__REPO__/blob/main/notebooks/adjoints_part4.ipynb) |

## Running the code

The pages on this site show the notebooks with their output already filled in, so you can read them without running anything. To change a parameter and rerun a cell, open a notebook "in your browser." That runs Python directly in your browser tab; the first load takes a few seconds while Python downloads. Python runs more slowly there than on a regular computer, so the timing comparisons in Parts 1, 2 and 4 will show larger absolute numbers, though the comparisons themselves still hold. If you'd rather have full speed, the Colab links open the same notebooks on Google's servers, which requires a Google account.
