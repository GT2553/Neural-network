
**TensorFlow Model Training & Analysis**

**Overview**

This project covers essential TensorFlow operations, including tensor
manipulations, loss function comparisons, optimizer performance
analysis, and TensorBoard logging. The tasks were implemented step by
step with explanations, providing hands-on experience in deep learning
techniques.

**Student Information**

**Name:** Tadikonda Gnandeep 

**ID:** 700759736 

**University:**University of Central Missouri

**Email:**gxt97360@ucmo.edu.com

**Project Tasks**

**Tensor Manipulations & Reshaping**

-   Created a random tensor of shape (4, 6).

    > Found its rank and shape before and after reshaping.

    > Reshaped it to (2, 3, 4) and transposed it to (3, 2, 4).

    > Applied broadcasting to add a smaller tensor (1, 4) to the larger
    > tensor.

**Broadcasting Explanation:** Broadcasting allows smaller tensors to be
automatically expanded to match the shape of larger tensors without
explicit copying. This simplifies element-wise operations by avoiding
redundant data storage and improving computational efficiency.

**Loss Functions & Hyperparameter Tuning**

-   Defined true values (y_true) and predicted values (y_pred).

    > Computed Mean Squared Error (MSE) and Categorical Cross-Entropy
    > (CCE).

    > Modified predictions slightly and observed loss variations.

    > Plotted a bar chart comparing MSE and CCE loss values.

**Key Insight:**

-   MSE is sensitive to small prediction variations, making it effective
    > for regression tasks.

    > CCE penalizes incorrect predictions more aggressively, making it
    > ideal for classification.

    > Loss values change significantly when predictions are modified,
    > highlighting the importance of well-tuned models.

**Train a Model with Different Optimizers**

-   Loaded the MNIST dataset (handwritten digits).

    > Trained two models using different optimizers:

    -   **Adam Optimizer:** Adaptive learning rates ensure faster
        > convergence.

    -   **SGD Optimizer:** Simpler approach but requires more epochs to
        > reach optimal accuracy.

    > Compared training & validation accuracy trends.

**Comparison:**

-   Adam optimizer converges faster and achieves better early-stage
    > performance.

    > SGD, while slower, can generalize better in some cases, especially
    > with larger datasets.

**Train a Neural Network and Log to TensorBoard**

-   Loaded and preprocessed the MNIST dataset.

    > Built a simple neural network for classification.

    > Enabled TensorBoard logging to track training progress.

    > Launched TensorBoard to analyze key performance metrics:

    -   **Training vs. Validation Loss**

    -   **Training vs. Validation Accuracy**

**Stored logs in:** logs/fit/

**Questions & Answers**

**1. Patterns in Training & Validation Accuracy:** Overfitting occurs
when validation accuracy stops improving while training accuracy
continues to increase. This indicates that the model is memorizing
training data rather than generalizing well.

**2. Using TensorBoard to Detect Overfitting:** Monitor validation loss
trends. If validation loss starts increasing while training loss
decreases, the model is likely overfitting.

**3. Effect of Increasing Epochs:**

-   More epochs allow the model to learn better representations, but too
    > many can lead to overfitting.

    > Implementing early stopping can prevent unnecessary training and
    > improve generalization.
