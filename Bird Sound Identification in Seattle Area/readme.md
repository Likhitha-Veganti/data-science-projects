# Bird Species Classification Using Neural Networks

## Abstract
This project explores the application of neural networks in classifying bird species based on their sounds. Utilizing a dataset from Xeno-Canto with 10 audio clips for each of the 12 selected bird species, the study focuses on binary classification (amecro vs. norfli) and multi-class classification for all 12 species. Various neural network architectures, including convolutional neural networks (CNNs) and transfer learning with VGG16, are employed and evaluated. The report discusses encountered limitations, compares model performances, and emphasizes the potential of neural networks for bird species identification.

## Introduction
Identification of bird species traditionally requires expertise. This project leverages machine learning, specifically neural networks, to classify species based on unique sound patterns. Binary and multi-class classification tasks are undertaken, addressing challenges of distinguishing between specific species and handling diverse characteristics. The dataset consists of 10 sound clips per species sourced from Xeno-Canto, recorded in the Seattle area.

### Dataset Description
The dataset includes original sound clips from Xeno-Canto, with 10 clips for each of the 12 bird species. Spectrograms generated from these clips serve as input for training the neural network.

### Problem Types
Binary classification focuses on distinguishing amecro and norfli, while multi-class classification involves all 12 species. This dual approach provides insights into different aspects of bird species classification, evaluating the performance of various neural network structures.

## Theoretical Background
### Neural Networks
Neural networks, inspired by the human brain, consist of interconnected nodes organized into layers. Various types, such as Feedforward Neural Networks (FNNs), Convolutional Neural Networks (CNNs), Recurrent Neural Networks (RNNs), and Long Short-Term Memory (LSTM) Networks, are employed based on the characteristics of the data.

### Compilation Techniques
Compilation involves configuring and optimizing the model before training. Choices like loss function, optimizer, and evaluation metrics significantly impact performance. Hyperparameters such as learning rate, batch size, and regularization techniques are carefully tuned for optimal results.

### Activation Function
Activation functions, like sigmoid and SoftMax, introduce non-linearity, enhancing the network's ability to learn complex patterns.

### Transfer Learning
Transfer learning leverages pre-trained models for new tasks, reducing data and computation requirements. This project employs VGG16 for audio classification.

### Spectrograms
Spectrograms visually represent frequency content over time, crucial for analyzing audio signals. They serve as input features for sound classification models.

## Methodology
### Data Preprocessing
Audio files undergo resampling, windowing, and spectrogram computation. Labels are one-hot encoded, and data is split into training and testing sets.

### Binary Classification
Two models, one with and one without dropout, are employed for distinguishing amecro and norfli.

### Multi-Class Classification
Sequential CNN models with and without dropout address the challenge of classifying all 12 bird species.

### Transfer Learning
Pre-trained VGG16 is adapted for audio classification, and model performance is evaluated.

## Computational Results
### Binary Classification
| Model                | Train Accuracy | Test Accuracy | Training Loss | Testing Loss |
|----------------------|----------------|---------------|---------------|--------------|
| Model 1              | 99.57%         | 99.16%        | 1.76%         | 1.78%        |
| Model 2 (with dropout)| 99.36%         | 99.16%        | 1.65%         | 1.75%        |

### Multi-Class Classification
| Model                | Train Accuracy | Test Accuracy | Training Loss | Testing Loss |
|----------------------|----------------|---------------|---------------|--------------|
| Model 1              | 90.95%         | 88.23%        | 31.15%        | 48.59%       |
| Model 2 (with dropout)| 92.22%         | 89.22%        | 26.28%        | 35.89%       |

### Transfer Learning
| Model                | Train Accuracy | Test Accuracy | Training Loss | Testing Loss |
|----------------------|----------------|---------------|---------------|--------------|
| VGG16                | 94.27%         | 92.94%        | 26.96%        | 32.54%       |

## Discussion
### Binary Classification
Both models performed well, with Model 2 showing potential benefits from dropout regularization. Overfitting concerns were mitigated, and generalization improved.

### Multi-Class Classification
Model 2, with dropout, outperformed Model 1, demonstrating improved generalization. The confusion matrix indicated challenges in distinguishing specific classes, potentially due to similar spectrogram patterns.

### Transfer Learning
VGG16 transfer learning achieved the highest accuracy, highlighting its effectiveness in audio classification tasks.

## Conclusion
The study showcased the effectiveness of neural networks in bird species classification based on sounds. Binary and multi-class classification tasks, along with transfer learning, provided valuable insights. Model performances were analyzed, and transfer learning demonstrated superior accuracy. The study lays the foundation for further exploration in the field of bird species identification using deep learning techniques.
