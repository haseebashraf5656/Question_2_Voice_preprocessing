Voice Preprocessing and Feature Extraction
Overview

This project demonstrates basic speech preprocessing and feature extraction techniques used in Machine Learning and Deep Learning.
Since uploading a real dataset was not possible, synthetic speech-like audio samples were generated to simulate real voice signals.

The goal of this assignment is to understand how raw audio is prepared before being used in ML models.

Objectives

Understand audio preprocessing steps

Learn how to clean and enhance speech signals

Extract useful features from audio

Prepare speech data for ML/DL models

Audio Samples

Two synthetic speech-like audio signals were created using sine waves with different frequencies.
Silence was added to simulate pauses in real human speech.

Preprocessing Pipeline

The following preprocessing steps were applied to both audio samples:

Audio Generation
Two speech-like signals were generated using multiple sine waves.

Resampling
Audio was generated at a sampling rate of 16 kHz, which is standard for speech processing.

Normalization
The audio amplitude was scaled between -1 and 1.

Silence Trimming
Silent parts at the beginning and end of the audio were removed.

Filtering (Pre-emphasis)
A pre-emphasis filter was applied to enhance high-frequency components of speech.

Visualization

The following visualizations were generated:

Raw waveform of both audio samples

Processed waveform after preprocessing

Comparison of raw vs processed signals

These visualizations help in understanding how preprocessing affects speech signals.

Feature Extraction

For both audio samples:

MFCC (Mel Frequency Cepstral Coefficients) were extracted

MFCCs were displayed as log-scale heatmap spectrograms

MFCCs are widely used features in speech recognition and audio classification tasks.

Feature Tensor

The extracted MFCC features from both audio samples were:

Padded to equal length

Combined into a single 3D tensor

Final tensor shape:

(2, 13, Time Steps)


This tensor can be directly used as input for ML or DL models.

Bonus: Noise Experiment

Random noise was added to one audio sample to observe its effect.

Observations:

Noise distorts the waveform

Silence trimming reduces unnecessary noise

Filtering improves feature quality

Tools and Libraries Used

Python

NumPy

Librosa

Matplotlib

Learning Outcomes

Learned basic audio preprocessing techniques

Understood silence trimming and filtering

Extracted MFCC features from speech

Prepared audio data for machine learning models

Conclusion

This project demonstrates a complete speech preprocessing and feature extraction workflow.
Even without a real dataset, synthetic audio effectively shows how speech data is prepared for machine learning applications.
