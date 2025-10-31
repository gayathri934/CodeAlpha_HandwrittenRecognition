This project demonstrates Handwritten Character/Digit Recognition using Deep Learning (CNN). It can identify handwritten digits from the MNIST dataset, and can be extended to characters (EMNIST) or full-word recognition using CRNN.

Objective

Identify handwritten digits or characters from images.

Extendable to full-word recognition with CRNN.

Approach

Dataset: MNIST (digits) or EMNIST (letters)

Preprocessing: Normalization, resizing, and reshaping images for CNN input

CNN Architecture:

Convolution → ReLU → Max Pool → Dropout → Fully Connected

Trained using CrossEntropyLoss for classification

Evaluation:

Accuracy, Confusion Matrix, Sample predictions

Optional CRNN:

CNN extracts features, RNN models sequences for full-word recognition

Uses LSTM + FC layer (CTC loss recommended for training)

