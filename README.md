# Audio-Augmentation-MFCC

Enhancing Whale Sound Data: Audio Augmentation and MFCC Analysis

"Audio Augmentation and MFCC Analysis for Whale Sound Data"

Technical Description:

In this comprehensive audio processing pipeline, we first load a whale sound dataset using the PyDub library and perform pitch shifting to manipulate the audio's pitch by a specified number of semitones. This step facilitates the creation of variant audio samples for analysis. Subsequently, we apply advanced audio augmentation techniques using the Audiomentations library, introducing Gaussian noise with a 50% probability. This augmentation process diversifies the dataset, making it more robust for subsequent analyses.

Next, we extract the augmented audio data as NumPy arrays and convert it back to PyDub's AudioSegment format. The augmented audio is saved to a specified export directory in WAV format, enabling easy accessibility for further analysis and model training.

The pipeline's analytical aspect involves the computation of Mel-frequency cepstral coefficients (MFCCs) for both the original and augmented audio segments using the Librosa library. MFCCs are essential features for acoustic analysis, capturing critical characteristics of sound, such as spectral content and timbral information. These coefficients enable us to gain insights into the acoustic properties of whale sounds and facilitate the comparison of augmented and original audio samples.

Lastly, we visualize the MFCC spectrogram of the augmented audio using Matplotlib and Librosa. This spectrogram offers a graphical representation of the audio's frequency content over time, aiding in the identification of patterns and distinctions between augmented and unaltered audio samples. This holistic approach enhances the analysis and understanding of whale sound data, contributing to the development of more effective machine learning models and acoustic research.
