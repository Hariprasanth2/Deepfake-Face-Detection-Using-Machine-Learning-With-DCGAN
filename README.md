# Deepfake Face Detection Using Machine Learning with DCGAN
The project Deepfake Face Detection Using Machine Learning with DCGAN focuses on building an intelligent system to identify manipulated videos and images generated through deepfake technology. It leverages Convolutional Neural Networks (CNNs) to extract spatial features and Long Short-Term Memory (LSTM) networks to capture temporal inconsistencies across video frames. To strengthen the training process, a Deep Convolutional Generative Adversarial Network (DCGAN) is used to generate synthetic samples, improving model’s ability to generalize and detect unseen deepfake manipulations. The system was trained on benchmark datasets like FaceForensics++, Celeb-DF, and DFDC, achieving an accuracy of 94.3%, outperforming traditional CNN-LSTM methods. This research demonstrates improved robustness in combating misinformation and fake media, while also highlighting future enhancements such as integrating transformer-based models, multimodal detection IMAGE, and developing real-time browser or mobile applications for wider accessibility.


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

## What Are GAN'S?
Generative Adversarial Networks also known as GANs are a set of deep-learning based adversarial models. That means they are able to generate new content from the given content. Generative modelling is a type of unsupervised learning algorithm in machine learning that learns and discovers patterns or irregularities in the input data in such a way that the model generates an output of new data instances that look almost like the input data. Long cut short a GAN takes in input data identifies its patter and underlying probability distribution and generates or mimics it to create fake versions of the original data and then classifies if the generated data is fake or real. For example a GAN can create images that look like photographs of human faces even though the face doesn't belong to any real person. A GAN model architecture involves two sub-models namely : a Generator model that creates the new instances(data) and a Discriminator model that classifies if the generator created data is real or fake. The generator tries to fool the discriminator, and the discriminator tries to keep from being fooled.

Generator - The generator plays the part of a falsifier and attempts to make music/image/speech from random noise. It figures out how to plan from an inert space to a specific data distribution of interest. It for the most part actualizes a Deconvolutional Network to do as such.

Discriminator-The Discriminator then again plays the function of the evaluator and attempts to recognize the fake data (made by the Generator) from the genuine one. It is generally executed as a Convolutional Network.
<img width="1536" height="1024" alt="Generative Adversarial Network Diagram" src="https://github.com/user-attachments/assets/548f7ca2-8eda-4510-8fea-aeec17f8d320" />


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

