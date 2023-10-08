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


reverb, delay, equalization
The FPGA-based audio equalizer will process an audio input signal and enable users to modify the gain or attenuation of specific frequency bands, thereby enhancing or customizing the audio output to their preferences.

Multiple Equalization Bands: Instead of just basic bass, midrange, and treble adjustments, you can implement a multi-band equalizer with more frequency bands for precise control.
Presets: Include preset equalization settings that users can quickly select for different audio scenarios (e.g., music, movies, gaming).
Real-Time Spectrum Analyzer: Implement a graphical display that shows users the frequency spectrum of the audio signal in real-time. This can be a visual representation of how the equalization is affecting the audio.
User Profiles: Allow users to save and load their custom equalization profiles, so they can switch between their preferred settings easily.
Signal Effects: Extend the project to include other DSP audio effects like reverb, chorus, or dynamic range compression, giving users a broader range of audio processing capabilities.
Advanced User Interface: If your FPGA board has a touchscreen or graphical display, create an intuitive and visually appealing interface for controlling the audio processing and effects.
Integration with External Devices: Explore ways to connect the FPGA project with external devices, such as smartphones or computers, to enable remote control or streaming audio from external sources


Select DSP Algorithms: Choose the DSP (Digital Signal Processing) algorithms that will form the core of your audio equalization system. Common algorithms for equalization include Finite Impulse Response (FIR) and Infinite Impulse Response (IIR) filters. These filters allow you to adjust the amplitude of specific frequency components.
Frequency Bands: Decide on the number of frequency bands for your equalizer. The more bands you have, the finer the control over the audio response. Common choices include 3-band (bass, midrange, treble), 5-band, or 10-band equalizers.
Implement Filters: Write VHDL or Verilog code to implement the selected filters for each frequency band. Ensure that your FPGA's resources are used efficiently. You'll need to design and connect multiple filter stages for multi-band equalization.
User Interface: Create a user interface (UI) for controlling the equalization settings. This can include buttons, switches, or a graphical interface (if supported by your FPGA board). Users should be able to adjust the gain (boost or attenuation) for each frequency band.
Audio Input and Output: Implement audio input and output modules that interface with the ADC and DAC on your FPGA board. Ensure that audio data is sampled at an appropriate rate and that the digital audio data is processed in real-time.
Real-Time Processing: Optimize your FPGA design to achieve real-time audio processing with minimal latency. Pay attention to clock domains and synchronization to prevent audio glitches.
Testing and Debugging: Test your equalizer's functionality and performance thoroughly. Use test signals and actual audio sources to validate that the equalization is working as expected.
User Documentation: Document your project, including a user manual that explains how to operate the equalizer and adjust settings. Include information about the equalization bands, their frequency ranges, and suggested use cases.
Project Presentation: Prepare a demonstration or presentation to showcase your FPGA-based audio equalizer. Highlight its features and how it can enhance audio quality.
Optional Enhancements: If you have the time and interest, consider adding optional features like presets, real-time spectrum analysis, or user profiles.
Finalization: Once you are satisfied with the functionality and performance of your audio equalizer, finalize the project by organizing your code, documentation, and any additional materials.


Filter Bands
Bass : below 300 Hz , 
Mid Range : 300Hz - 4kHz
Treble : 4kHz - 20KHz+ 

Filter Type for each frequency range
Bass - Low passa filter
Mid Range - Band Pass
Treble - High pass filter




