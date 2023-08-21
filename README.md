# Speech-Emotion-Recognition

#### Problem Statement:
Speech is the most natural way of expressing ourselves as humans. It is only natural 
then to extend this communication medium to computer applications. We define 
speech emotion recognition (SER) systems as a collection of methodologies that 
process and classify speech signals to detect the embedded emotions. Below we will 
show the needed steps to achieve the goal of the assignment. 

#### Dataset:
We will use CREMA dataset that is available at the following link: 
https://www.kaggle.com/dmitrybabko/speech-emotion-recognition-en
a. **Data Splitting:**
   -  We splited the data into 70% for training and validation, and 30% for testing.

b. **Validation Data:**
   - 5% of the training and validation data for the validation set.


#### Feature Space:

In this step, we will generate different features from the audio data including:

1. **Zero-Crossing Rate:** The rate at which the audio signal changes sign within a frame.
2. **Energy:** The sum of squared amplitudes within a frame, indicating signal intensity.
3. **Mel-Frequency Cepstral Coefficients (MFCCs):** Coefficients capturing spectral characteristics for audio analysis.
4. **Chroma:** A representation of musical notes, highlighting pitch classes in audio.
5. **Contrast:** Measures amplitude differences between peaks and valleys.
6. **Mel Spectrogram 1D:** Visualizes frequency energy distribution over time.
7. **Mel Spectrogram 2D:** Matrix-based representation of frequency energy over time.

#### CNN Models:
   For the CNN models we used varies archeticture to test the performance of each on the features we extracted.
   We used some of the famouse archetictures like AlexNet, VGG16, leNet5, and we build our own archeticture.
   For each model we used it as a 1D archeticture and as a 2-D archeticture for the 2 feature space we created as for the 1-D feature space we used zero-crossing rate, energy, MFCCS, chroma, contrast, and mel Spectrogram 1D.
   for the 2-D feature space we used mel Spectrogram 2D.
