# Deepfake Face Detection Using Machine Learning with DCGAN
The project Deepfake Face Detection Using Machine Learning with DCGAN focuses on building an intelligent system to identify manipulated videos and images generated through deepfake technology. It leverages Convolutional Neural Networks (CNNs) to extract spatial features and Long Short-Term Memory (LSTM) networks to capture temporal inconsistencies across video frames. To strengthen the training process, a Deep Convolutional Generative Adversarial Network (DCGAN) is used to generate synthetic samples, improving model’s ability to generalize and detect unseen deepfake manipulations. The system was trained on benchmark datasets like FaceForensics++, Celeb-DF, and DFDC, achieving an accuracy of 94.3%, outperforming traditional CNN-LSTM methods. This research demonstrates improved robustness in combating misinformation and fake media, while also highlighting future enhancements such as integrating transformer-based models, multimodal detection IMAGE, and developing real-time browser or mobile applications for wider accessibility.


## 📄 Abstract
Deepfake technology, powered by Generative Adversarial Networks (GANs), has gained attention due to its ability to produce highly realistic but synthetic media. While such advancements have applications in entertainment, education, and digital creativity, they also raise serious concerns regarding privacy, security, and misinformation. Traditional deepfake detection models, primarily based on Convolutional Neural Networks (CNNs), often fail to generalize across different deepfake types because of the rapid evolution of generative models. To address these challenges, we propose a hybrid detection framework that integrates CNNs for spatial feature extraction with Long Short-Term Memory (LSTM) networks for capturing temporal inconsistencies across image frames.  

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
<img width="1536" height="1024" alt="ChatGPT Image Aug 22, 2025, 09_27_08 AM" src="https://github.com/user-attachments/assets/bab3d19f-8c9f-4414-9811-80babdbeb390" />



---
## 📂Literature review
Deepfake detection has emerged as a vital research domain owing to the rapid progress of generative models. A variety of techniques have been proposed, including Convolutional Neural Networks (CNNs), Recurrent Neural Networks (RNNs), and hybrid methods that integrate multiple approaches. Traditional CNN-based models, such as XceptionNet, ResNet, and VGG16, have proven effective in detecting deepfakes by extracting spatial features from individual frames. However, these models often fall short in identifying temporal inconsistencies across video frames, which reduces their accuracy in video-based detection tasks. To overcome these limitations, hybrid models that combine CNNs with recurrent networks like Long Short-Term Memory (LSTM) and Gated Recurrent Units (GRU) have been investigated. Such models leverage sequential frame analysis, enabling them to detect deepfake-specific anomalies, including mismatched lip-sync, unnatural facial expressions, and subtle pixel-level artifacts. Research indicates that adding temporal analysis substantially enhances detection performance compared to static frame-based models.


## 🧠 Methodology
1. **Preprocessing**: Extract video frames, resize, normalize, and apply augmentation.  
2. **DCGAN**: Generate synthetic deepfake samples to improve dataset diversity.  
3. **CNN (ResNeXt)**: Extracts spatial features from frames.  
4. **LSTM**: Performs temporal sequence analysis for inconsistencies.  
5. **Classification Layer**: Sigmoid-based classifier to predict real vs fake.  

---

## 📈 Results And Discussions
Performance Evaluation
The proposed deepfake detection system achieved notable improvements by integrating DCGAN for data augmentation, CNN for spatial feature extraction, and LSTM for temporal sequence analysis. The model was tested on benchmark datasets including FaceForensics++, Celeb-DF, and DFDC, and delivered strong results:
Accuracy: 94.3%
Precision: 93.8%
Recall: 94.5%
F1-Score: 94.1%
Compared to conventional CNN-LSTM approaches, the inclusion of DCGAN improved detection accuracy by 4–6%, confirming the effectiveness of synthetic data in strengthening model robustness.
Performance Metrics
Performance was measured using standard classification metrics—accuracy, precision, recall, and F1-score—on widely used deepfake datasets (FaceForensics++, Celeb-DF, DFDC). The results validate that DCGAN-enhanced training significantly boosts detection capabilities, making the model highly reliable in identifying manipulated content.

OUTPUT
![WhatsApp Image 2025-08-22 at 9 48 29 AM](https://github.com/user-attachments/assets/29705c2f-7252-4f59-9d46-0d1ea4c617be)

---

## 🚀 Future Work
- Incorporating **transformer-based architectures** for better sequence modeling.  
- Developing a **real-time browser extension or mobile app** for deepfake detection.  
- Exploring **multimodal analysis** (audio + video).  
- Expanding dataset with diverse, high-quality deepfake samples.  

---

## 📂 Conclusion
This paper introduces an enhanced deepfake detection framework that integrates DCGAN, CNN, and LSTM to overcome the limitations of traditional detection models. The DCGAN is employed to generate synthetic training data, thereby enriching the dataset and improving the model’s ability to generalize to unseen deepfake manipulations. CNNs are leveraged for spatial feature extraction, capturing fine-grained pixel-level details such as lighting inconsistencies and facial artifacts, while LSTMs focus on temporal sequence analysis, identifying irregularities across consecutive frames such as unnatural motion or lip synchronization issues. Together, these components form a hybrid architecture that enhances the accuracy, robustness, and adaptability of the system. Experimental evaluations on benchmark datasets such as FaceForensics++, Celeb-DF, and DFDC confirm the model’s effectiveness, achieving an impressive 94.3% accuracy along with balanced precision, recall, and F1-score values. The proposed approach not only reduces false positives but also demonstrates strong generalization across diverse deepfake datasets, outperforming conventional CNN-LSTM methods.

Future Enhancements

While the current system delivers high detection accuracy, several opportunities exist for further improvement. Incorporating transformer-based architectures could significantly enhance feature extraction and long-sequence modeling, making the system more adaptable to emerging deepfake techniques. Expanding the detection framework to include multimodal analysis—combining both visual and audio features—would strengthen robustness against sophisticated manipulations involving synchronized voices and facial expressions. In addition, the development of a real-time browser extension or mobile application could make deepfake detection more accessible to the public, enabling instant verification of online media. Finally, increasing the diversity and quality of the training dataset by integrating larger and more realistic deepfake samples would ensure better performance against evolving threats. These future directions highlight the potential for building scalable, user-friendly, and highly accurate deepfake detection solutions for real-world applications.


