# Getting Started

## Adding a measurement panel to InstrumentStudio
Setting up the InstrumentStudio Panels
Open InstrumentStudio

![image](https://github.com/NI-MeasurementLink-Plug-Ins/data-converter-validation-module/assets/158176813/94b1d922-3597-4316-8f48-67d88df32163)


Click Manual Layout, and select AC measurement service in the large panel. Click OK.




AC measurement UI will get displayed on a large panel as below screenshot.

image.png

Open a new tab, Under PXIChassis 1 -> SMU/Power supply PXIe-4145 -> large panel -> SMU/Power supply PXIe-4139 -> SMU/Power Supply 1

image.png

All panels are set.

Powering ON
Set 3.3 V and 5 V Supplies according to the actual board connections:

image.png

In the example we are using two different supplies for AC and DC portions of the ADC:
SMU 4145 -> Channel 0 -> 3.3V
SMU 4139 -> Channel 0 -> 5V
Turn on the Output for each SMU.

AC Measurement Software Workflow
Run the measurement service with the default values and select the appropriate resource names. Press run.

image.png

The measurements in Frequency and time domain graphs should be visible.

image.png
## Adding a measurment step to TestStand 

## Measurements
### AC
### AC MultiChannel
### Linearity
### Gain and Offset
### Full Scale Error
### Channel to Channel Isolation
