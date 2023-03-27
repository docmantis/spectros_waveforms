Bird Call Visualization
This Python script is designed to visualize bird call recordings by plotting both the waveform and spectrogram of each audio file in a specified directory. The graph uses a dark theme with pop-out colors, making it easy to analyze the data.

Requirements
Python 3.6 or higher
NumPy
Matplotlib
SciPy
To install the required packages, you can use the following command:

  pip install numpy matplotlib scipy
 
Usage

Download the script and place it in a folder.
Update the directory variable in the script with the path to the directory containing your bird call audio files in WAV format.
Run the script:

  python bird_call_visualization.py
  
For each audio file in the directory, the script will generate a combined plot showing the waveform and spectrogram of the bird call. The waveform is plotted in green, and the spectrogram is displayed using a colormap with a high color contrast. The displayed filename is cleaned up by removing underscores and the ".wav" extension for better readability.



Notes

This script is designed for use with mono or stereo WAV files. If the input file is stereo, the script will automatically convert it to mono by averaging the two channels.

The spectrogram's time-frequency resolution may vary depending on the length of the input audio file. Shorter files will have a better time resolution.

If you encounter a WavFileWarning related to non-data chunks in the WAV file, the script will suppress the warning and continue processing the file. The warning does not affect the script's functionality.


  
