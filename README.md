# CIFAR-10 Image Classification using Inception_v1

This project demonstrates the training of an **Inception_v1 Convolutional Neural Network** on the **CIFAR-10 dataset**, leveraging **auxiliary classifiers** and a **custom learning rate scheduler** to enhance performance and convergence.

---

## 📊 Dataset

- **Dataset**: [CIFAR-10](https://www.cs.toronto.edu/~kriz/cifar.html)
- **Total Images**: 60,000
  - **Training**: 50,000 images
  - **Testing**: 10,000 images
- **Classes**: 10 (airplane, automobile, bird, cat, deer, dog, frog, horse, ship, truck)
- **Image Size**: 32×32 RGB (3 channels)

---

## 🧠 Model Architecture

- **Base Network**: Inception_v1 (GoogLeNet)
- **Auxiliary Classifiers**: 2
- **Final Layer Activation**: `softmax` (for multiclass classification)
- **Loss Function**: `categorical_crossentropy`
- **Optimizer**: Adam (or your choice)
- **Learning Rate Scheduling**: Custom learning rate scheduler applied per epoch

---

## 🏁 Final Training Results (Epoch 25)

| Metric                         | Value    |
|-------------------------------|----------|
| Training Accuracy             | 93.62%   |
| Training Loss                 | 0.3260   |
| Validation Accuracy           | 76.27%   |
| Validation Loss               | 1.4739   |
| Final Learning Rate           | 0.0088   |
| Aux Output 1 Accuracy         | 89.75%   |
| Aux Output 2 Accuracy         | 93.29%   |
| Val Aux Output 1 Accuracy     | 75.11%   |
| Val Aux Output 2 Accuracy     | 75.90%   |

---

## 🛠️ Technologies Used

- Python
- TensorFlow / Keras
- NumPy, Matplotlib
- Jupyter Notebook (optional)

---

## 🚀 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/inception-cifar10.git
   cd inception-cifar10
