# Gain And Offset
This service measures the Gain and Offset of the ADC DUT. When the voltage range is configured and the number of steps for the measurement. At each step, the signal generator outputs a DC voltage. The DC voltage is measured by both the DMM and ADC. The measured value for each is stored and the process repeats until the last voltage is reached. The gain and offset are determined by least squares fit using the DMM and ADC voltage measurements.
## Gain and Offset Testsetup
![Gain and Offset](https://github.com/NI-MeasurementLink-Plug-Ins/adc/blob/main/docs/images/Gain%20and%20Offset%20Test%20Setup.png)
## InstrumentStudio Panel
### Usage
In the Measurement section, enter the information for the Gain and Offset.  
![Gain and Offset](https://github.com/NI-MeasurementLink-Plug-Ins/adc/blob/main/docs/images/Gain%20and%20offset.PNG)
