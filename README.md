This project demonstrates Handwritten Character/Digit Recognition using Deep Learning (CNN). It can identify handwritten digits from the MNIST dataset, and can be extended to characters (EMNIST) or full-word recognition using CRNN.

Objective

Identify handwritten digits or characters from images.

Extendable to full-word recognition with CRNN.

Approach

Dataset & Preprocessing (20–30 sec)

Used the MNIST dataset, which contains 28x28 grayscale images of digits 0–9.

For letters, EMNIST can be used.

Images are normalized and reshaped for input into a Convolutional Neural Network, which helps the model learn effectively.

CNN Architecture:

Convolution → ReLU → Max Pool → Dropout → Fully Connected

Trained using CrossEntropyLoss for classification

Evaluation:

Accuracy, Confusion Matrix, Sample predictions

Optional CRNN:

CNN extracts features, RNN models sequences for full-word recognition

Uses LSTM + FC layer (CTC loss recommended for training)

