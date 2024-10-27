# Neural-ODEs-for-MNIST

This repository contains my solutions and notes for the Neural Ordinary Differential Equations (ODEs) homework. The tasks involve using neural ODEs for image classification, exploring the architecture, and performing various experiments on the provided source code.

🔗 Resources

- Main Neural ODE Library: [torchdiffeq GitHub repository](https://github.com/rtqichen/torchdiffeq)

- MNIST Classification Example Code: [odenet_mnist.py](https://github.com/rtqichen/torchdiffeq/blob/master/examples/odenet_mnist.py)

- Reference Paper: [Neural Ordinary Differential Equations by Chen et al](https://arxiv.org/abs/1806.07366)

- Reference Paper: [Complete 72-Parametric Classification of New and Old Kinds of Surface Plasmon Waves by Maxim Durach](https://arxiv.org/abs/1806.00736)

- Neural ODE features: [Pytorch training repository](https://github.com/fabiocarrara/neural-ode-features)

📋 Tasks

- Task 1: Set Up Code in Google Colab

Goal: Load and run the provided MNIST classification example code (odenet_mnist.py) in Google Colab.

Instructions: Clone the torchdiffeq repository, install dependencies, and make any necessary modifications to ensure the code runs smoothly in the Colab environment.

- Task 2: Structure and Role of ODEfunc Class
  
Description: Explain the structure and role of the ODEfunc class in several sentences.

Objective: Describe how ODEfunc defines the dynamics of the ODE system for neural ODEs.

- Task 3: Structure and Role of ODEblock Class

Description: Explain the structure and role of the ODEblock class in several sentences.

Objective: Describe how ODEblock handles the integration process for computing the forward pass through the neural ODE.

- Task 4: Layer Roles in the Architecture

Layers: The architecture consists of the following layers:

Downsampling Layer: Reduces input dimensionality for efficient processing.

Neural ODE Layer: Applies continuous transformations for feature extraction.

Classifier Layer: Maps the transformed features to output classes.

Objective: Describe the role of each layer in several sentences.

- Task 5: Training with adjoint=True

Description: Train the model with adjoint=True and observe the output values for each epoch, paying special attention to the NFE values.

Objective: Describe the meaning of each metric value shown during training, with a focus on NFE (Number of Function Evaluations).

- Task 6: Comparison of adjoint=False and adjoint=True

Objective: Train the model with both adjoint=False and adjoint=True.
For adjoint=True, test different solvers (Euler, RK4, DOPRI).
Create a chart comparing training/testing accuracy across all cases.
Report the average training time per epoch for each configuration.

Output: Paragraph explaining the impact of using the adjoint method on speed and accuracy, along with the chart and average wall-clock time.

- Task 7: Testing on Other Datasets

Objective: Test the neural ODE model on a new dataset of choice, such as CIFAR-10, SVHN, or Tiny ImageNet (subsample if necessary).

Additional Requirements:
Experiment with model architecture modifications.
Tune the model with techniques like batch normalization, optimizers, ODE solvers, dropout, and learning rate scheduling.

- Task 8: Deriving the Backward Pass and Gradient of Neural ODEs

Objective: Derive the backward pass and gradient for neural ODEs. Reference the Neural ODEs paper or other online resources for guidance.

Explanation: Provide a proof or derivation. There are multiple approaches, ranging from complex to simpler methods.

📊 Results Summary

- Task 6 Results: Include a chart showing training/testing accuracy vs. epochs for different adjoint settings and solvers.

- Task 7 Results: Report results for the new dataset, including tuning choices and their impact on accuracy.
