# Audio Exploration Dashboard

This real-time audio explorer was created in response to a coursework assignment for this Simulation and Visualisation module, which required students to pick and partially solve a Mini Challenge from the 2018 VAST Challenge (http://www.vacommunity.org/VAST+Challenge+2018).

I chose to tackle the following objective from Mini Challenge 1 (http://vacommunity.org/VAST+Challenge+2018+MC1):

*Determine whether the bird call exemplars provided by Kasios back up their claim that the Pipits are thriving in the reserve*

## Audio Clip Classification 

Birdcall_classifier.ipynb reads in audio files, extracts MFCC features and trains a 4-layer stacked LSTM using Keras, as devised by Dr. Jason Collins in his Deep Listening experiments (https://github.com/jaron/deep-listening/blob/master/7-us8k-rnn-extract-train.ipynb).

This trained model is then used to predict classifications for each of the test clips provided by Kasios.

This notebook was not marked and is uploaded here as a working file, i.e. not cleaned and commented.

## Dashboard Visualisation

The test clips' waveforms were then dynamically displayed alongside species exemplars, such that the user can interactively select test clips and species clips and compare them so as to visually confirm the model classification. To increase visual diagnostic ability, there is also the option to carry out a Fourier transform on the clips so as to plot the spectrograms.

This was made dynamic and interactive using ipywidgets and the Dashboard extension for Jupyter (https://jupyter-dashboards-layout.readthedocs.io/en/latest/index.html).


**Github occasionally struggles to render large .ipynb files; if they are not displaying, please paste the whole URL into nb viewer (https://nbviewer.jupyter.org/).**
