# ADC Measurements
Data Converter Validation Module application is developed in LabVIEW 2021 SP1. In this version we are shipping our measurements as measurement services using MeasurementLink.This plug-in makes measurements for 16bit SAR ADC currently added support for the AD7606B ADC. The output of the AD7606B is a digital waveform.
![image](https://github.com/NI-MeasurementLink-Plug-Ins/data-converter-validation-module/assets/158176813/aff8e19b-9b8e-42eb-bbe3-4552a86206b2)

## Key Features
- Measurements
    - AC Measurement
    - Linearity Measurement
    - Gain And Offset Measurement
    - Full-Scale Error Measurement
    - Channel To Channel Isolation Measurement

## Hardware Setup
![Hardware setup](docs/images/hw-setup.png)
Instrumentation:
- NI Dynamic Signal Acquisition device (NI 446x)
- NI 7820/21 
- SMU or power supply (note: the software does not use the SMU/power supply but need something to power the DUT)

Tested hardware setup:
- NI 4468
- NI 657x
- NI 4139
- AD7606B evaluation board

## Software dependencies:
- LabVIEW 64-bit 2021.0 SP1
- Sound and Vibration Toolkit support for LabVIEW (21.5 or higher)
- LabVIEW FPGA development support (22.3 or higher)
- MeasurementLink 2023 Q4
- MeasurementLink Support for LabView v1.1.0.3 (https://github.com/ni/measurementlink-labview/releases/tag/v1.1.0.3)
- LabView gRPC support for LabView v1.0.0.1 (https://github.com/ni/grpc-labview/releases/tag/v1.0.0.1)
- NI Digital driver (22.8 or higher)
- NI DAQmx driver (22.8 or higher)
- NI DMM driver (22.8 or higher)

Download the latest NI package from the releases section of this repo or add the feed to NI Package Manager to get updates from this repo and other in this community 

[comment]: # (add link to documnetation at community level)

## Getting Started
When you are ready to start using the software, check out [this](docs/help.md).

## Contributing
Use the instructions in [software development](docs/sw-dev.md) for setting up a development environment and overview of the code.
