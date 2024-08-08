### Types of Gradient Descent:

1. **Batch Gradient Descent**:
   - Updates the model after evaluating the entire training set.
   - Pros: Stable convergence.
   - Cons: Computationally intensive for large datasets.

2. **Stochastic Gradient Descent (SGD)**:
   - Updates the model after each individual training example.
   - Pros: Faster and can escape local minima.
   - Cons: Noisy gradients may cause fluctuations in the error.

3. **Mini-Batch Gradient Descent**:
   - Updates the model after evaluating small batches of the training set.
   - Pros: Balances efficiency and speed.
   - Cons: May still experience some fluctuations but less so than SGD.
