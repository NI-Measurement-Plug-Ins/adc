# ADC Measurements
This measurement plugin makes the measurements for the ADC's. This measurement plugin was developed in 2021 SP1 LabView. This test generates an Analog signal and then acquires the digital waveform and measures it.   
![AC](https://github.com/NI-MeasurementLink-Plug-Ins/adc/blob/main/docs/images/AC.PNG)

## Key Features
- Measurements
    - AC Measurement
    - Linearity Measurement
    - Gain And Offset Measurement
    - Full-Scale Error Measurement
    - Channel To Channel Isolation Measurement

## Hardware setup:
- NI 446x
- NI 657x
- NI 4139
- AD7606B evaluation board
- SMU or power supply (note: the software does not use the SMU/power supply but need something to power the DUT)

  ![image](https://github.com/NI-MeasurementLink-Plug-Ins/adc/blob/main/docs/images/AC%20Measurement%20Setup.PNG)

## Software dependencies:
- LabVIEW 64-bit 2021.0 SP1
- Sound and Vibration Toolkit support for LabVIEW (21.5 or higher)
- LabVIEW FPGA development support (22.3 or higher)
- MeasurementLink 2024 Q1
- MeasurementLink Dependencies (https://github.com/ni/measurementlink-labview/releases/tag/v2.0.0.1)
- NI Digital driver (22.8 or higher)
- NI DAQmx driver (22.8 or higher)
- NI DMM driver (22.8 or higher)



[comment]: # (add link to documnetation at community level)

## Getting Started
When you are ready to start using the software, check out [this](docs/help.md).

## Contributing
Use the instructions in [software development](docs/sw-dev.md) for setting up a development environment and overview of the code.
