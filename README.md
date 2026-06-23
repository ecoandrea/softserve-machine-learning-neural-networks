# softserve-machine-learning-neural-networks
Understanding Neural Networks,  machine learning models made of layers of neurons that learn patterns from data. They work by adjusting weights while learning, improving predictions over time, and are used for tasks like classification, regression, and generating data.


# Neural Networks - Summary

## What are Neural Networks?

* Neural networks are machine learning models inspired by the human brain.
* They learn patterns from data by adjusting internal parameters called **weights**.
* They are used for classification, regression, and data generation tasks.

---

## Structure of a Neural Network

### Input Layer

* Receives the raw data (features).
* Each neuron represents one input feature.

### Hidden Layers

* Perform most of the learning.
* Detect patterns and relationships in the data.
* Deeper layers learn more complex features.

### Output Layer

* Produces the final prediction.
* Structure depends on the task (binary, multi-class, regression).

---

## Forward Propagation

* Process where data flows from input → output.
* Each neuron computes:

```text id="fwd1"
z = (w₁x₁ + w₂x₂ + ... + wₙxₙ) + b
a = activation(z)
```

Where:

* **x** = inputs

* **w** = weights

* **b** = bias

* **a** = output

* This process generates the model’s prediction.

---

## Activation Functions

* Add **non-linearity**, allowing networks to learn complex patterns.
* Without them, the model would behave like a linear function.

Common ones:

* **ReLU**: removes negative values, widely used in hidden layers.
* **Sigmoid**: outputs values between 0 and 1 (binary classification).
* **Softmax**: converts outputs into probabilities for multiple classes.

---

## Loss Functions

* Measure how wrong the model’s predictions are.
* The goal of training is to **minimize loss**.

Examples:

* **Binary Cross-Entropy**: binary classification.
* **Categorical Cross-Entropy**: multi-class classification.
* **Mean Squared Error (MSE)**: regression tasks.

---

## Training Process

1. Forward propagation generates predictions.
2. Loss function calculates error.
3. Backpropagation computes how to adjust weights.
4. Weights are updated to improve performance.

### Key terms:

* **Epoch**: one full pass through the dataset.
* **Batch size**: number of samples processed before updating weights.

---

## Neural Network Architectures

### Feed-Forward Neural Networks (FNN)

* Basic architecture.
* Works well with structured/tabular data.
* Used for classification and regression.

### Recurrent Neural Networks (RNN)

* Designed for sequential data.
* Can retain memory of previous inputs.
* Used in text, speech, and time series.

### Convolutional Neural Networks (CNN)

* Specialized for images and spatial data.
* Detect features like edges, shapes, and textures.

### Generative Adversarial Networks (GAN)

* Two networks:

  * Generator creates fake data.
  * Discriminator detects real vs fake.
* Used for image generation and data synthesis.

---

## Overfitting and Regularization

### Overfitting

* Happens when a model memorizes training data.
* Leads to poor performance on new data.

### Regularization Techniques

* **L1 / L2**: control weight size.
* **Elastic Net**: combination of L1 and L2.
* **Dropout**: randomly disables neurons during training.
* **Early Stopping**: stops training before overfitting.
* **Batch Normalization**: stabilizes learning.
* **Data Augmentation**: increases dataset diversity.

---

## Key Idea

* Neural networks learn by adjusting weights through training.
* They improve gradually over time by minimizing error.
* Different architectures are used depending on the type of data and problem.
