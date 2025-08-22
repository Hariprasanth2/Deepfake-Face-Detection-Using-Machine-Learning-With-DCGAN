# Deepfake Face Detection Using Machine Learning with DCGAN
The project Deepfake Face Detection Using Machine Learning with DCGAN focuses on building an intelligent system to identify manipulated videos and images generated through deepfake technology. It leverages Convolutional Neural Networks (CNNs) to extract spatial features and Long Short-Term Memory (LSTM) networks to capture temporal inconsistencies across video frames. To strengthen the training process, a Deep Convolutional Generative Adversarial Network (DCGAN) is used to generate synthetic samples, improving the model’s ability to generalize and detect unseen deepfake manipulations. The system was trained on benchmark datasets like FaceForensics++, Celeb-DF, and DFDC, achieving an accuracy of 94.3%, outperforming traditional CNN-LSTM methods. This research demonstrates improved robustness in combating misinformation and fake media, while also highlighting future enhancements such as integrating transformer-based models, multimodal detection (audio + video), and developing real-time browser or mobile applications for wider accessibility.


## 📄 Abstract
Deepfake technology, driven by Generative Adversarial Networks (GANs), has raised significant concerns due to its potential misuse in creating hyper-realistic synthetic media. Traditional detection models struggle to generalize across various deepfake types.  
This project proposes a **deepfake face detection framework** utilizing a hybrid **Convolutional Neural Network (CNN)** and **Long Short-Term Memory (LSTM)** model, enhanced with a **Deep Convolutional Generative Adversarial Network (DCGAN)** for synthetic training data generation.  
The proposed model improves robustness, generalization, and detection rates compared to traditional approaches.

---

## ⚙️ Technologies
- Python  
- TensorFlow  
- PyTorch  
- OpenCV  

---

## 📊 Datasets Used
- **FaceForensics++**  
- **Celeb-DF**  
- **DFDC (Deepfake Detection Challenge)**  

---

## 🧠 Methodology
1. **Preprocessing**: Extract video frames, resize, normalize, and apply augmentation.  
2. **DCGAN**: Generate synthetic deepfake samples to improve dataset diversity.  
3. **CNN (ResNeXt)**: Extracts spatial features from frames.  
4. **LSTM**: Performs temporal sequence analysis for inconsistencies.  
5. **Classification Layer**: Sigmoid-based classifier to predict real vs fake.  

---

## 📈 Results
- **Accuracy**: 94.3%  
- **Precision**: 93.8%  
- **Recall**: 94.5%  
- **F1-Score**: 94.1%  
- Outperformed conventional CNN-LSTM approaches by **4–6%**.

---

## 🚀 Future Work
- Incorporating **transformer-based architectures** for better sequence modeling.  
- Developing a **real-time browser extension or mobile app** for deepfake detection.  
- Exploring **multimodal analysis** (audio + video).  
- Expanding dataset with diverse, high-quality deepfake samples.  

---

## 📂 Repository Structure
```
Deepfake-Detection-DCGAN/
│── README.md                → Project details
│── finalConferencepaper.pdf → Research paper
│── requirements.txt         → Python libraries
│── src/                     → Source code folder
│   ├── model.py
│   ├── train.py
│   ├── detect.py
│── data/                    → (Optional) sample dataset links/instructions
```
---

⚠️ **Disclaimer**: This project is developed strictly for **educational and research purposes** to combat misinformation and enhance cybersecurity.

