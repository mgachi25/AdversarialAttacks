# Gradient-based perturbation attacks
This notebook investigates a method for finding adversarial examples on image classification tasks. In particular, we use gradient based perturbation attacks, which climb the loss gradient with respect to input images to find adversarial perturbations.

To implement these attacks, we train a CNN which achieves near-perfect accuracy on the original MNIST digit classification dataset, but quickly gets arbitrarily bad accuracy when faced with adversarial perturbations. By introducing gradient-based attacks during the training process, we train a new model which achieves the same accuracy on MNIST while being far more robust to perturbations.

The attack used is based on the Fast Gradient Sign Method (FGSM), which was introduced in ["Explaining and Harnessing Adversarial Examples"](https://arxiv.org/pdf/1412.6572) (Goodfellow et. al., 2015)
