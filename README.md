Got it — let’s make your README more engaging with a few well-placed emojis while keeping it professional.

---

# 🇦🇲 Mashtots Dataset v2 – Armenian Handwritten Letter Classification ✍️

## 📌 Overview

This project is built around the **Mashtots Dataset v2**, a Kaggle competition focused on classifying **Armenian handwritten letters**.
The dataset was developed by the Automation Systems & Modeling Laboratory at the **National Polytechnic University of Armenia** and is widely used in education and research.

🔗 [Kaggle Competition Page](https://www.kaggle.com/competitions/mashtots-dataset-v2/overview)

---

## 📂 Dataset Details

* **🎯 Task**: Classification of Armenian handwritten characters.
* **🏛 Origin**: Created by the Basic Research Laboratory of Automation Systems & Modeling, NPUA, with support from the Science and Technology Foundation of Armenia.
* **📊 Structure**:

  * **Train**: \~70,060 grayscale images (64×64 px) across **78 classes**.
  * **Test**: \~50,000 images (some with incorrect labels for fraud detection).
* **💡 Use Cases**: Benchmark for CNN-based vision models & educational purposes.

---

## 🎯 Objectives

* 🧠 Build a high-accuracy handwritten letter classifier.
* 🔬 Experiment with architectures like **ResNet**, **VGG**, and **SpinalNet**.
* 📈 Improve accuracy with **image augmentation** (rotation, noise, perspective shifts).

---

## 📁 Project Structure

```
├── data/
│   ├── Train/
│   ├── new_test/
│   └── sample_submissions.csv
├── notebooks/
│   └── TorchKeras
├── README.md
└── requirements.txt
```

---

## ⚙️ Installation

```bash
git clone (https://github.com/erantonyan24/Armenian-Letters-Classification.git)
cd Armenian-Letters-Classification
pip install -r requirements.txt
```

---

## 🚀 Usage

1. 📥 **Download the dataset** from Kaggle and place it under `data/`.
2. 🔄 **Preprocess the data**:

   ```bash
   python src/data_preprocessing.py --data-dir data/
   ```
3. 🏋️ **Train the model**:

   ```bash
   python src/train.py --architecture resnet --epochs 50
   ```
4. 📊 **Evaluate performance**:

   ```bash
   python src/train.py --evaluate --model-path models/resnet_best.pth
   ```

---

## 🔮 Future Enhancements

* 🖌️ More diverse data augmentations (brightness, warping, synthetic data).
* 🤖 Try transformer-based architectures (ViT, Swin).
* 🌐 Deploy as a real-time web app for instant letter recognition.

---

## 🙏 Acknowledgments

* 📚 **Automation Systems & Modeling Laboratory**, NPUA – for dataset creation.
* 🤝 Kaggle community – for helpful notebooks and ideas.

---

