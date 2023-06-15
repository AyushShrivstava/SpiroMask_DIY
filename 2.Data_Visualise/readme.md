## Data Visualization

This folder provides valuable code for visualizing data in the SpiroMask project. These visualization scripts offer insights into the characteristics of the audio files associated with the SpiroMask. Here's an overview of the contents within this folder:

### 1. **Visualise_Waveforms.ipynb**: 
This notebook generates visual representations of the raw waveforms of audio files. By plotting the waveforms in the time domain, users can observe the temporal variations in the audio signals. The notebook iterates through the SpiroMask_Audio_Samples folder, producing waveform visualizations for each audio file.

### 2. **Visualise_Bandpass.ipynb**: 
Focusing on bandpass filtered waveforms, this notebook helps users examine the effects of filtering on the audio signals. By visualizing the waveforms after applying the bandpass filter, users can observe the specific frequency range emphasized by the filter. It performs this visualization for all audio files in the SpiroMask_Audio_Samples folder.

### 3. **Visualise_Envelope.ipynb**: 
This notebook visualizes the envelope of the audio signals after applying the bandpass filter. The envelope represents the amplitude envelope of the filtered signals, providing insights into the overall amplitude variations. Similar to the previous notebooks, it generates envelope visualizations for all audio files in the SpiroMask_Audio_Samples folder.

### 4. **Visualise_Autoclipping.ipynb**: 
This notebook focuses identifying the start and end points of each breath within the audio signals. By visualizing the autoclipping effects, users can accurately detect and demarcate breath cycles. Autoclipping helps in distinguishing breath-related components from other background noises, facilitating a more precise analysis of respiratory patterns. The notebook applies autoclipping visualization to all audio files in the SpiroMask_Audio_Samples folder, enabling users to gain insights into breath segmentation and enhance their understanding of respiratory dynamics.

### 5. **Visualise_Spectrogram.ipynb**: 
This notebook generates spectrograms, which provide a comprehensive frequency-domain representation of the audio signals. It showcases the spectral content over time, both before and after applying the bandpass filter. All the previous visualizations are also applied on the filtered audio signal making this file the one_stop visualize all notebook. Additionally, the notebook creates a PDF file containing spectrograms for all audio files in the SpiroMask_Audio_Samples folder, facilitating a holistic view of the audio data.

---

By utilizing these data visualization resources, users can gain deeper insights into the audio characteristics of the SpiroMask project. These visualizations contribute to a better understanding of the signal processing techniques applied and can aid in identifying any anomalies or patterns within the audio data.