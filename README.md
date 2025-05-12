# 🧠 Handwritten Digit Recognition using CNN

This project demonstrates handwritten digit recognition using a **Convolutional Neural Network (CNN)** trained on the **MNIST dataset**. You can upload your own digit image (like "2") or even use a webcam (optional extension) to recognize digits in real-time.

---

## 📌 Project Highlights

- 🧠 Trained on the MNIST dataset (60,000 training, 10,000 testing samples)
- ⚙️ Built using TensorFlow, Keras, NumPy, and PIL
- 🖼️ Can predict digits from static images (28x28 pixels, grayscale)
- 📷 Extendable to real-time digit recognition using webcam and OpenCV

---

## 🛠️ Prerequisites

Before running the code, make sure you have Python 3 installed along with these libraries:

```bash
pip install tensorflow numpy pillow
````

> Optional for webcam version:

```bash
pip install opencv-python
```


## 🧠 About CNN (Convolutional Neural Network)

CNNs are specialized deep learning models for processing image data. Key layers:

* **Conv2D:** Extracts features from image using filters
* **MaxPooling2D:** Reduces image size to retain dominant features
* **Flatten:** Converts feature map to a 1D array
* **Dense:** Fully connected layer for classification

CNNs are widely used for image classification, facial recognition, medical imaging, and more.

---

## 🧪 Model Summary

* **Input Shape:** `(28, 28, 1)` grayscale image
* **Architecture:**

  * Conv2D (32 filters) → MaxPooling
  * Conv2D (64 filters) → MaxPooling
  * Flatten → Dense (64) → Output (10)
* **Loss Function:** `sparse_categorical_crossentropy`
* **Optimizer:** `adam`
* **Final Accuracy:** \~98% on test data

---

## 🚀 How to Use

### 1. Train the Model (if not already trained)

```bash
python train_model.py
```

This will save the model as `digit_model.keras`.

### 2. Predict Digit from Image

Make sure your image:

* Is **28x28 pixels**
* Is in **grayscale**
* Has a **white digit on black background**

Then run:

```bash
python predict_digit.py
```

Example output:

```
Predicted digit from image: 2
```

---

## 📷 Optional: Real-time Webcam Prediction

If you want to draw a digit on paper and show it to your webcam:

```bash
python webcam_predict.py
```

> Make sure:
>
> * Lighting is good
> * Digit is centered in the webcam view
> * Background is dark for better accuracy

---

## 📚 Dataset

The [MNIST dataset](http://yann.lecun.com/exdb/mnist/) is a standard benchmark for handwritten digit recognition containing 70,000 images (28x28 grayscale).

---

## 🤝 Contributing

Pull requests are welcome! Feel free to open issues for suggestions or bugs.

---

## 📃 License

This project is licensed under the MIT License. See `LICENSE` for more details.

---

## ✨ Author

**Bharath G P** – https://github.com/BharathGuddadar

---
