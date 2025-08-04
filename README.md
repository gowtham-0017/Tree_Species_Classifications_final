# 🌳 Tree Species Classification using EfficientNetB0

This project uses a deep learning model to classify images of different tree species using the **EfficientNetB0** architecture. The model is trained on a dataset containing images of various tree categories like neem, mango, banyan, coconut, etc.

## 📁 Dataset

The dataset contains images for 30+ tree species, structured in folders — one for each class.

Example structure:

Tree_Species_Dataset/ ├── mango/ ├── neem/ ├── banyan/ ├── coconut/ └── ...

## 🧠 Model Architecture

- **Base Model**: EfficientNetB0 (pre-trained on ImageNet, without top layer)
- **Additional Layers**:
  - GlobalAveragePooling2D
  - Dense (128 units, ReLU)
  - Dropout (0.3)
  - Dense (number of classes, Softmax)

## 🏋️ Training Details

- **Epochs**: 10
- **Optimizer**: Adam (learning rate = 0.001)
- **Loss Function**: Categorical Crossentropy
- **Batch Size**: 32
- **Input Image Size**: 224x224

### 📊 Model Performance (on validation data)

- ✅ **Validation Accuracy**: 91.3%
- 📉 **Validation Loss**: 0.28

## 📦 Files Included

- `Tree_Species_Classification.ipynb` – Colab notebook for training and evaluation
- `model.h5` – Saved trained model
- `README.md` – Project documentation

## 🚀 How to Use

1. Clone this repo:
    ```bash
    git clone https://github.com/gowtham-0017/Tree_Species_Classifications_final.git
    ```

2. Open the notebook in Google Colab.

3. Upload your dataset and follow the steps to train or test the model.

## 👨‍💻 Author

- Gowtham (AICTE Internship Project)

## 📜 License

This project is for educational and academic purposes only.
