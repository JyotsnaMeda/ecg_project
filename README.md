# ECG_SENSOR_DESIGN
This project involves the various processing steps used to extract an ECG signal from the patient and further calculate the BPM of the patient by looking at the output waveform

Initially the project was planned to be implemented on hardware, but due to COVID-19, it was pushed to simulation mode.

We modelled an input waveform, which comprised noises at different frequencies similar to what we would get in an actual raw ECG signal. But in no means is this equivalent to the actual signal.

Multiple stages are used in the processing of the ECG sensor circuit as shown in the "full-circuit.pdf" which was simulated on LT-Spice.

The filtered signal is fed into a thresholding circuit which extracts only the highest peak in the wave , which is indicated by the red colored wave in "final_output.jpg". This output peak is used for the determination of Beats-Per-Minute of the patient.
