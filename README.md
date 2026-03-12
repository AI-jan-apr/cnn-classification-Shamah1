# CNN Classification

Binary image classification using CNN to classify images as cats or dogs.

---

## Dataset
[Microsoft Cats vs Dogs — Kaggle](https://www.kaggle.com/datasets/shaunthesheep/microsoft-catsvsdogs-dataset)
- 24,996 valid images after filtering corrupted files
- Labels: 0 = Cat, 1 = Dog

---

## Model Architecture
- 4 × Conv2D (32→64→128→256) + ReLU + MaxPooling
- Flatten → Dense (512) → Dropout (0.5) → Sigmoid
- Loss: Binary Cross-Entropy | Optimizer: Adam

---

## Results

| Metric | Score |
|---|---|
| Accuracy | 0.8917 |
| Precision | 0.8951 |
| Recall | 0.8875 |
| F1-Score | 0.8913 |

---

## Observations
- Balanced performance on both classes
- The model misclassifies some images, particularly black cats and long-haired dogs which share visual features
