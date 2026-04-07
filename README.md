# SIMULATION-OF-AUTOCORRELATION-AND-PSD-USING-SCILAB-1-T1-C12-EVEN
AIM:

Write a program for Autocorrelation and PSD of signals in SCILAB and verify Wiener-Khinchin relation.

EQUIPMENTS Needed:

.Computer with i3 Processor

.SCI LAB

THEORY:

The Wiener-Khinchin theorem states that the power spectral density of a wide sense stationary random process is the Fourier transform of the corresponding autocorrelation function.

Algorithm:

1.Load or Define the Signal: Input your time-domain signal.

2.Compute Autocorrelation: Calculate the autocorrelation function of the signal.

3.Compute Power Spectral Density (PSD): Estimate the PSD of the signal, either directly using a method like Welch’s periodogram or by using the Fourier transform of the autocorrelation.

4.Plot Results: Visualize the autocorrelation function and PSD.

PROCEDURE:

Refer Algorithms and write code for the experiment.

Open SCILAB in System

Type your code in New Editor

Save the file

Execute the code

If any Error, correct it in code and execute again

Verify the generated waveform using Tabulation and Model Waveform

PROGRAM:
```
clc;
clear;

t = 0:0.01:2*%pi;
x = Sin (2*t);

Subplot (3,2,1);
plot (t,x);
title("original Signal");

au = x Corr (x,x);
Subplot (3,2,2);
plot (a,u);
title ("FFT of autocorrelation");

fw = fft (x);
Subplot (3,2,4);
plot (abs (fw));
title ("FFT of Signal");

fw2 = (abs (fw)).*2
Subplot (3,2,5);
plot (fw2);
title("Power spectrum");
```

OUTPUT:
<img width="2874" height="1465" alt="EXP6" src="https://github.com/user-attachments/assets/d394ae07-dd85-4f46-a121-91462eef6c72" />





RESULT:
<img width="1600" height="921" alt="image" src="https://github.com/user-attachments/assets/692beeea-83e0-4792-9b45-880c0cd046b3" />



