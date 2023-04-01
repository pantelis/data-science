# Simple Language Models

In this assignment you will build an neural network that can model language. This is essentially your first step n understanding chatGPT !

You will build the neural network using the JAX library.
JAX is an extensible system for **composable function transformations**. You can read its benefits for a wide range of scientific applications [here](https://github.com/google/jax) and in the following video:

```{eval-rst}
.. youtube:: WdTeDXsOSj4
```

Bear in mind that although JAX will feel veryu much as numpy, there is one important difference between JAX and NumPy arrays: JAX arrays are immutable, meaning that once created their contents cannot be changed. This is not a limitation but for many a desired attribute of functional programming.

## Part 1: Autodiff (30 points)

Watch this video and implement the neural network (called Multi Layered Perceptron) using the JAX autodiff instead of the micrograd library that the presenter uses.

```{eval-rst}

.. youtube:: VMj-3S1tku0
```

Please pay attention to using the `import jax.numpy as jnp` instead of `import numpy as np` and the `import jax` instead of `import micrograd.engine as engine`.

## Part 2: Bigram Language Model (50 points)

Watch these two videos and implement the language model neural network using the JAX and [Flax](https://flax.readthedocs.io/en/latest/guides/flax_basics.html).

```{eval-rst}

.. youtube:: PaCmpygFfXo

```

```{eval-rst}

.. youtube:: TCH_1BHY58I
```

You are **not** allowed to use `torch` or `TF2`. 


## Part 3: Documentation (20 points)

Write a summary of your experiment in your README.md file such as the objective clearly explaining what a simple language model is. Please note that points will be subtracted if your code is delivered uncommented.   



