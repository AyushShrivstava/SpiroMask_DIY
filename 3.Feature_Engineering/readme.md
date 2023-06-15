# Feature Extraction for SpiroMask Audio Analysis

The Jupyter Notebook `Feature_Extractor` provides the feature extraction pipeline specifically tailored for analyzing audio data captured for the SpiroMask. The notebook facilitates the extraction of various features from the SpiroMask audio signals, enabling in-depth analysis of respiratory patterns and lung health estimation.

## Features Included

The feature extraction pipeline encompasses the following features, which are particularly relevant for SpiroMask analysis:

1. **Spectrogram (STFT):** Computes the spectrogram of the SpiroMask audio signals using the librosa library. The spectrogram provides a visual representation of the audio signals in the frequency domain, allowing the examination of respiratory patterns and related characteristics.

2. **MFC (Mel-frequency cepstral coefficients):** Calculates the MFC features of the SpiroMask audio signals using the librosa library. MFCs capture the spectral properties of the audio signals and are commonly used for speech and respiratory analysis.

3. **Mel Spectrogram:** Generates the mel spectrogram of the SpiroMask audio signals using the librosa library. The mel spectrogram emphasizes the perceptual frequency bands, providing valuable insights into the distribution of energy in the respiratory audio signals.

4. **MFE (Multiscale Fractal Energy):** Extracts the MFE features from the SpiroMask audio signals using the speechpy library. MFE captures the fractal-like properties of the audio signals and can offer additional information about the complexity and irregularity of the respiratory patterns.

5. **MFCC (Mel-frequency cepstral coefficients):** Computes the MFCC features of the SpiroMask audio signals using the speechpy library. MFCCs are widely used in speech and respiratory analysis and provide a compact representation of the spectral characteristics of the audio signals.

6. **MFCC CMVN (Mean-variance normalization of MFCC):** Applies mean-variance normalization to the MFCC features extracted from the SpiroMask audio signals using the speechpy library. Normalizing the MFCCs helps to remove any bias in the feature distribution and improves comparability across different audio samples.

7. **Spectral Features:** Extracts various spectral features from the SpiroMask audio signals using the tsfel library. These features provide detailed information about the frequency content of the audio signals and can be useful for characterizing respiratory patterns.

8. **Temporal Features:** Calculates a range of temporal features from the SpiroMask audio signals using the tsfel library. These features capture temporal aspects such as the duration, variability, and other statistical properties of the respiratory patterns.

## Usage

To utilize the feature extraction pipeline for SpiroMask audio analysis, follow these steps:

1. Specify the directory containing the SpiroMask audio files.
2. Select the desired features to be extracted by setting the corresponding flags.
3. Optionally, configure additional parameters such as applying a bandpass filter, audio clipping, or waveform normalization to preprocess the audio signals.
4. Run the notebook to initiate the feature extraction process.
5. The extracted features will be computed and stored for further analysis and lung health estimation.

#

The feature extraction pipeline in this notebook provides a powerful tool for analyzing SpiroMask audio data, facilitating the exploration of respiratory patterns and supporting accurate lung health estimation. By leveraging these extracted features, researchers, healthcare professionals, and developers can gain valuable insights into respiratory dynamics and the effectiveness of the SpiroMask.

#