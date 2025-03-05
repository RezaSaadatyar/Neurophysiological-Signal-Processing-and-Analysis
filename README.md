# Neurophysiological Signal Processing and Analysis
This repository contains an extensive collection of tools and scripts specifically designed for the processing and analysis of neurophysiological signals. The primary focus of this software is on various critical aspects of neurophysiological data handling, including:

1. **Spike Detection**: The software offers sophisticated algorithms for identifying spikes in neural recordings. These algorithms are imperative for understanding neuronal activity as spikes are fundamental signals that indicate when a neuron fires.

2. **Feature Extraction**: Once spikes are detected, the next step is to extract relevant features that can provide insights into the characteristics of these spikes and the overall neuronal activity. This may include metrics such as spike amplitude, duration, frequency, and inter-spike intervals.

3. **Clustering**: The repository also includes tools for clustering detected spikes. Clustering is essential for grouping similar spike events, which can help distinguish between different neuronal populations or types of spikes, enhancing the analysis of brain activity.

4. **Firing Rate Analysis**: Firing rate analysis allows researchers to quantify the frequency of neuron firing over time, providing crucial insights into neuronal behavior under various conditions.

The software is intended for researchers and practitioners in the field of neuroscience who require reliable and efficient tools to analyze complex neural data. Overall, this repository is an invaluable resource for enhancing our understanding of neural dynamics and functions.

This repository contains tools and scripts for processing and analyzing neurophysiological signals, focusing on spike detection, feature extraction, clustering, and firing rate analysis. Below is an overview of the steps involved in the pipeline and the functionalities provided by the software.




**Related Article**:<br/>
[Restoring the firing activity of ventral tegmental area neurons by lateral hypothalamic deep brain stimulation following morphine administration in rats](https://www.sciencedirect.com/science/article/abs/pii/S0031938423001348).

## Demo
https://github.com/user-attachments/assets/63ad798b-1b53-4c0c-a431-453ac2859a92

## Steps in the Pipeline

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
