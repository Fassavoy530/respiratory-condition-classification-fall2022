# NYUSH-Machine-Learning-Fall2022-Final-Project

This is a course project for class CSCI-SHU 360 Machine learning, completed by my teammate Lihan Feng and I and guided by Prof. Mathieu Lauriere. <br> <br>
Recently diagnoses based on AI techniques have come to the stage because the nature of inflammation caused by various diseases can lead to audible changes which can further be identified as diagnostic signals. To better understand what kind of techniques are best suit for the issue, we constructed our project topic as **Multi-Respiratory Diseases Classifications: Implementing and Comparing Different Machine Learning Techniques** where we focus on: <br>
- Classify 8 different respiratory health condition based on respiratory cycles.
- Compare the performance of different machine learning models such as tranditional ML models and deep learning models.

## Dataset
Our primary dataset is an open source dataset from kaggle called Respiratory Sound Database ([link](https://www.kaggle.com/datasets/vbookshelf/respiratory-sound-database)). <br>
The paper for orginal data collection is call "Α Respiratory Sound Database for the Development of Automated Classification" [^1].

## Data Pre-processing and Model development
We used librosa package to trim wav files, extract MFCCs and Mel-spectrograms features from the wav files. Tranditional model such as Decision Tree and SVM were implemented using scikit-learn library. We also used PyTorch framework to experiment transfer learning using pretrained CNN models such as VGG16 and Alexnet. Both models were also trained from scratch due to a potential domain shift problem brought by our task and input. Details can be found in the source code notebook, arranged by different sections.


[^1]: Rocha, B. M., Filos, D., Mendes, L., Vogiatzis, I., Perantoni, E., Kaimakamis, E., ... & Maglaveras, N. (2018). Α respiratory sound database for the development of automated classification. In Precision Medicine Powered by pHealth and Connected Health: ICBHI 2017, Thessaloniki, Greece, 18-21 November 2017 (pp. 33-37). Springer Singapore.
