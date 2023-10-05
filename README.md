# Audio-Equalizer

Project Description - The goal of this project is to implement a real-time audio proccesing device on a FPGA that can perform audio equilization. 

Hardware Components
MAX 10 FPGA - 50K logics Elements
Audio Source
Audio Amplifier - Speaker
Additional Features
Should include a user interface
Other audio processing algorithms


Software 
Quartus Prime

Algorithm Used for Adui DEwqulization
Finite Impulse Response Filter

Audio Processing Flow
1) Audio(Analog) is converted to Digital with an ADC(on the FPGA board)
2) Audio is proccesed using FIR filter
3) The filter is applied to the audio
4) Audio is converted to analog by the DAC on the FPGA board and played with a speaker



