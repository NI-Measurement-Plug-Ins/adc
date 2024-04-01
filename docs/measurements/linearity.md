# Linearity 

This service measures the Integral Nonlinearity (INL) and Differential Nonlinearity (DNL) of the DUT using histograms generated from three different types of input signals: sine, triangular, and ramp signals.
## Linearity Testsetup
![linearity](https://github.com/NI-MeasurementLink-Plug-Ins/adc/blob/main/docs/images/Linearity%20Test%20Setup.png)
## InstrumentStudio Panel
### Usage
In the Measurement section, enter the information for the Linearity measurement.  
![linearity](https://github.com/NI-MeasurementLink-Plug-Ins/adc/blob/main/docs/images/Linearity.PNG)

#### Tips
##### Sine Wave
1. The user can define the sine wave frequency and amplitude.
2. To hit all the ADC codes, it is recommended to have and the sine wave amplitude 10% greater than the input range of the ADC. The user can also configure the ADC sampling rate and the test duration. The sine wave frequency will be coerced to a value that is relatively prime to the sampling rate.
##### Triangle Wave
This method is like the sine wave approach except the generated signal is a triangle wave.
##### Ramp
This method is similar to the sine wave method except the generated signal is a non-repeating ramp.
