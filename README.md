This project focuses on developing a classifier for urban sounds using deep learning techniques. The dataset used is "UrbanSound8K," which contains 8,732 sound clips categorized into 10 distinct classes, including air conditioners, car horns, and dog barks.

Objective
The main goal is to implement two deep learning models:

Multilayer Perceptron (MLP)
Convolutional Neural Network (CNN)
These models are designed to classify the sounds after performing necessary data preprocessing, including resampling audio to a uniform frequency and normalizing audio lengths.

Preprocessing
Audio Standardization: Resampled all audio clips to 44,100 Hz and normalized their duration to 4 seconds using zero padding.
Feature Extraction: Extracted Mel Frequency Cepstral Coefficients (MFCCs) as features, which were then used as inputs for the models.
Models
MLP: Utilized a simple architecture with one input layer and one output layer, using ReLU activation and softmax for classification. The model was trained for 15 epochs with Adam optimizer.
CNN: Employed a two-dimensional convolutional neural network with ReLU activation, batch normalization, and max-pooling layers, followed by dense layers for final classification.
Advanced Techniques
Time Manipulation: Techniques like sound repetition and interpolation were applied to enhance the dataset, particularly improving the performance over zero-padding alone.
Model Refinement: Adjusted model parameters, including dropout, L2 regularization, and learning rate, to improve performance while preventing overfitting.
Results
MLP: Achieved an average accuracy of 66% using cross-validation, indicating a moderate generalization capability.
CNN: Showed an average accuracy of 43%, with noticeable oscillations in loss, suggesting challenges in model stability and representativity of the validation data.
Conclusion
Both models provided moderate results, with MLP slightly outperforming CNN in generalization. However, neither model achieved exceptional performance, highlighting areas for future improvement, such as exploring more advanced architectures or fine-tuning hyperparameters.

This project demonstrates the complexities involved in urban sound classification and sets the stage for further research and refinement in this domain.

versão do python usada: Python 3.9.13

lista com versões das bibliotecas usadas:


librosa                   0.9.2
matplotlib                3.5.2           
numpy                     1.25.2
pandas                    1.4.4
scikit-learn              1.2.2
seaborn                   0.11.2
scipy                     1.9.1
soundata                  0.1.2
soundfile                 0.12.1
tensorflow                2.15.0

Para compilar o codigo basta executar todas as celulas presentes no notebook.
