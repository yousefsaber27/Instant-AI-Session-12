### Types of Gradient Descent

1. **Batch Gradient Descent**

   - **Description**: Computes the gradient of the loss function with respect to the parameters for the entire training dataset and performs an update after processing all training examples. This process is repeated for each training epoch.
   - **Advantages**: 
     - Provides stable error gradients and convergence.
     - Often results in smooth convergence to a minimum.
   - **Disadvantages**:
     - Can be computationally expensive and slow for large datasets as it requires loading the entire dataset into memory.
     - Might converge to local minima rather than the global minimum.

2. **Stochastic Gradient Descent (SGD)**

   - **Description**: Computes the gradient of the loss function with respect to the parameters for a single training example and updates the model parameters immediately after processing each example.
   - **Advantages**:
     - Requires less memory as it processes one example at a time.
     - Can potentially escape local minima due to noisy gradients, increasing the chance of finding a global minimum.
   - **Disadvantages**:
     - The frequent updates can lead to noisy gradients and less stable convergence.
     - May be less computationally efficient due to the constant updates.

3. **Mini-batch Gradient Descent**

   - **Description**: Splits the training dataset into small batches and performs gradient updates for each batch. The model parameters are updated after processing each mini-batch.
   - **Advantages**:
     - Balances between computational efficiency and the speed of convergence.
     - Reduces the variance of the parameter updates, which can lead to more stable convergence than SGD.
   - **Disadvantages**:
     - Requires tuning of the mini-batch size, which can affect performance.
     - While more efficient than batch gradient descent, it still involves managing multiple batches.
