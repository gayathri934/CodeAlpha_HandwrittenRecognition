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

Project Structure
CodeAlpha_HandwrittenRecognition/
├─ data/               # MNIST/EMNIST datasets (downloaded automatically)
├─ handwritten_recognition.py  # Full CNN model training & evaluation
├─ crnn_template.py    # CRNN structure for word recognition (optional)
├─ demo.ipynb          # Jupyter Notebook for running and testing predictions
└─ README.md           # Project description

Getting Started
1. Clone the Repository
git clone https://github.com/<your-username>/CodeAlpha_HandwrittenRecognition.git
cd CodeAlpha_HandwrittenRecognition

2. Install Dependencies
pip install torch torchvision matplotlib scikit-learn seaborn

3. Run the Notebook (Recommended in Colab)

Open demo.ipynb in Google Colab

Select Runtime → Change runtime type → GPU (optional)

Run all cells to:

Download MNIST dataset

Train CNN model

Evaluate accuracy and confusion matrix

Test predictions on sample images

4. Run the Python Script (Optional)
python handwritten_recognition.py

Results

High test accuracy on MNIST digits (>98% typical)

Confusion matrix visualization

Demo predictions on sample images

Optional CRNN Extension

CRNN template provided (crnn_template.py) for full-word recognition

Uses CNN feature extractor + LSTM sequence modeling

Can be trained on word-level datasets for sequence recognition
