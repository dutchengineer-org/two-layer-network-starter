# Two-Layer Network

Starter repository for the **Calculus and Optimisation** capstone on [DutchEngineer](https://dutchengineer.org).

## What you will build

A two-layer neural network trained by hand-computed backpropagation — no autograd, no framework. Every gradient is derived and implemented manually. Before training, gradient correctness is verified numerically. Then the network is trained to solve a non-linearly-separable problem.

This is where the calculus module stops being abstract. A working backprop implementation means you understand exactly what happens inside the automatic differentiation system you will use for the rest of your career.

## Requirements

1. **Forward pass** — a two-layer network with a hidden activation and an output activation. The forward pass returns enough intermediate state to compute gradients.
2. **Loss function** — a loss appropriate for binary classification, numerically stable when predictions are near 0 or 1.
3. **Backward pass** — gradients for all parameters, derived by hand from the chain rule. No autograd at any step. The derivation must be documented in the code.
4. **Gradient verification** — all gradients checked numerically before training. Maximum relative error across all parameters must be below an accepted tolerance. The check runs on a small batch and produces a pass/fail result.
5. **Training to convergence** — the network is trained on the XOR problem. Final training loss must be below 0.05. Loss is printed periodically so convergence is visible.

## Getting started

1. **Fork this repository** — click **Fork** at the top of [this page](https://github.com/dutchengineer-org/two-layer-network-starter) to create your own copy.
2. Clone your fork:
   ```
   git clone https://github.com/<your-username>/two-layer-network-starter
   cd two-layer-network-starter
   ```
3. Install dependencies: `uv sync`
4. Build and run: `uv run python network.py`

## Submitting

When your work is ready, paste your repository URL into the submission form on your [capstone page](https://dutchengineer.org/foundations/calculus-and-optimisation/capstone-two-layer-network/).
