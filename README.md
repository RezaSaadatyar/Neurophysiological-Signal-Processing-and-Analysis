# Neurophysiological Signal Processing and Analysis
This repository contains an extensive collection of tools and scripts for processing and analyzing neurophysiological signals. The primary focus is on various critical aspects of neurophysiological data handling, including spike detection, feature extraction, clustering, and firing rate analysis. The software is intended for researchers and practitioners in the field of neuroscience who require reliable and efficient tools to analyze complex neural data.

**Related Article**:<br/>
[Restoring the firing activity of ventral tegmental area neurons by lateral hypothalamic deep brain stimulation following morphine administration in rats](https://www.sciencedirect.com/science/article/abs/pii/S0031938423001348).

## What do you Learn
- Spike Detection: Identifying action potentials (spikes) in neural signals using techniques like amplitude threshold discrimination.
- Feature Extraction: Extracting relevant features from signals for further analysis.
- Clustering: Grouping similar neural signals or patterns, potentially using methods like k-means or fuzzy c-means clustering.
- Firing Rate Analysis: Analyzing the frequency of neural spikes to understand neural activity.
- Interspike Interval (ISI) Analysis: Measures the time intervals between consecutive spikes in a neuron’s firing sequence. ISI is critical for analyzing firing patterns, such as bursting or regular spiking, and can reveal insights into neuronal excitability and network dynamics.

## Demo
https://github.com/user-attachments/assets/63ad798b-1b53-4c0c-a431-453ac2859a92

## Software Outline

1. **Data Import and Preprocessing**
   - Import data from various formats (e.g., `.mat`, `.txt`, `.xlsx`).
   - Perform artifact removal and filtering using methods like Moving Average, Butterworth, Chebyshev, and Elliptic filters.
   - Apply band-pass filtering to the waveform.
   - Fs = 30000 Hz;                 % Sampling frequency  
   - F_low = 300 Hz;                % low pass filter for detection  
   - F_high =3000 Hz;               % high pass filter for spike detection  

2. **Spike Detection**
   - Use amplitude threshold discrimination to detect spikes.
   - Record spike times and align events.

3. **Feature Extraction**
   - Extract feature coefficients using Principal Component Analysis (PCA) and Wavelet Transform.
   - Select relevant feature coefficients for further analysis.

4. **Spike Clustering**
   - Cluster spikes using unsupervised algorithms such as Fuzzy C-Means (FCM), and K-Means.

5. **Firing Rate and ISI Analysis**
   - Analyze the distribution of firing rates.
   - Compute Interspike Interval (ISI) histograms and autocorrelograms for each class.

6. **Visualization and Results**
   - Generate and display firing rate figures, ISI histograms, and autocorrelograms.
   - Save results for further analysis.

## Usage

1. Clone the repository:
   ```bash
   git clone https://github.com/RezaSaadatyar/Neurophysiological-Signal-Processing-and-Analysis
   ```
2. Open MATLAB and navigate to the cloned directory.
3. Run the `main.m` file to launch the graphical user interface.

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request with your changes.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contact

For any questions or support, please contact Reza.Saadatyar@outlook.com
