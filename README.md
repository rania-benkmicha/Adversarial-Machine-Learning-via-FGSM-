
# Adversarial Examples with FGSM

This project explores the creation of adversarial examples using the Fast Gradient Sign Method (FGSM) attack. It demonstrates how imperceptible perturbations to an image can mislead a pre-trained image classification model.

## Project Goal

The main objective is to understand and implement the FGSM attack to fool a pre-trained MobileNetV2 model, causing it to misclassify images.

## Implementation

1. **Load Data:** Load a pre-trained MobileNetV2 model and an image of a tiger.
2. **Implement FGSM:** Create a function to generate adversarial perturbations using the gradients of the loss with respect to the input image.
3. **Apply Perturbations:** Add the generated perturbations to the original image with varying epsilon values (intensity of the attack).
4. **Observations:** Observe the impact of different epsilon values on the model's classification.
5. **Find Maximum Perturbation:** Empirically determine the maximum perturbation that doesn't fool the model.
6. **Plot Probability:** Visualize the probability of the correct class as the attack intensity increases.


## Results

- As the epsilon value increases, the model's confidence in the correct class decreases, eventually leading to misclassification.
- The maximum perturbation without fooling the model was found around an epsilon value of 0.006.
- The probability of the correct class decreases as the intensity of the attack increases.


## Conclusion

This project demonstrates the vulnerability of image classification models to adversarial attacks. By understanding and implementing FGSM, we can gain insights into the potential risks and develop strategies for defense.
