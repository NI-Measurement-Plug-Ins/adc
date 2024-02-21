# Getting Started

## Adding a measurement panel to InstrumentStudio
Setting up the InstrumentStudio Panels
Open InstrumentStudio

![alt text](image-1.png)


Click Manual Layout, and select AC measurement service in the large panel. Click OK.

![alt text](image-2.png)

AC measurement UI will get displayed on a large panel as below screenshot.

![alt text](image-3.png)

Open a new tab, Under PXIChassis 1 -> SMU/Power supply PXIe-4145 -> large panel -> SMU/Power supply PXIe-4139 -> SMU/Power Supply 1

![alt text](image-4.png)

All panels are set.

Powering ON
Set 3.3 V and 5 V Supplies according to the actual board connections:


Turn on the Output for each SMU.

AC Measurement Software Workflow

Go to the C:\ProgramData\National Instruments\MeasurementLink\Services\Digital Server. Click on AD7606B_DPIserver.exe before running the measurement service.

![alt text](image-5.png)

Run the measurement service with the default values and select the appropriate resource names. Press run.

![alt text](image-6.png)

The measurements in Frequency and time domain graphs should be visible.
![alt text](image-7.png)

## Adding a measurment step to TestStand 

[[_TOC_]]
The following workflow provides an example to show how we can automate our measurements using TestStand from the Instrument Studio and also shows how monitoring can be done. 
### Setting up the InstrumentStudio Panels
1.  Open InstrumentStudio

    ![image.png](/.attachments/image-3a35e08b-0561-436c-8e84-eb3687465c7c.png =850x500)

2.  Click Manual Layout, and select AC measurement service in the large panel. Click OK.

    ![image.png](/.attachments/image-e7cadaa4-421c-42fc-9b80-7702083a107b.png =850x500)
3. AC measurement UI will get displayed on a large panel as below screenshot.

   ![image.png](/.attachments/image-6ee99ff3-1fee-41f4-9b4f-acdfb25090a3.png =850x500)

3. Open a new tab, Under PXIChassis 1 -> SMU/Power supply PXIe-4145 -> large panel -> SMU/Power supply PXIe-4139 -> SMU/Power Supply 1

    ![image.png](/.attachments/image-4959faaf-4e3e-412d-894d-1c06028c3f97.png =850x500)
4. All panels are set.




### Powering ON
1. Set 3.3 V and 5 V Supplies according to the actual board connections:

   ![image.png](/.attachments/image-43afe810-e1b2-4dc6-8015-9ff1acee25e7.png =850x500)

   In the example we are using two different supplies for AC and DC portions of the ADC: 
SMU 4145 -> Channel 0 -> 3.3V
SMU 4139 -> Channel 0 -> 5V  
Turn on the **Output** for each SMU. 

###AC Measurement Software Workflow
1. Run the measurement service with the default values and select the appropriate resource names. Press run.

    ![image.png](/.attachments/image-64c681f3-43c3-43fe-9104-67b29ecd034b.png =850x500)





###TestStand Support for Data Converter Validation Module
1. Open TestStand 21.0 or higher version. Open new sequence file or saved sequence file. 
 
   ![image.png](/.attachments/image-85b509f1-e076-4488-b9dc-42d2b782b395.png =700x).

2. To transfer the measurement configuration from the Instrument Studio to the TestStand, click on "COPY button" highlighted in the screenshot.

   ![image.png](/.attachments/image-f4ba64fc-b0e7-4cda-912b-a9d8529e144e.png =850x)

3. In InstrumentStudio, copy the measurement configuration from the InstrumentStudio to the TestStand select the "Copy Measurement Configuration"

   ![image.png](/.attachments/image-3d15a1c9-c694-4bd3-89ee-b6d75a82e07c.png =850x)

4. In TestStand, from the insertion Palette, select the measurement link step, add it to the sequence file, and click on the paste button as highlighted in the screenshot. Make Enable monitor to True.

   ![image.png](/.attachments/image-2527311f-c942-432c-8266-b7555a2102ab.png =850x)

5. The measurement configuration copied to the TestStand saved sequence file.

   ![image.png](/.attachments/image-bd0a2eed-a414-49fe-ba6b-0dc00327e8f1.png =850x)

6. Save the Sequence file and RUN the sequence. While running the sequence file in TestStand you can see measurement resultant graphs and results were updated in the InstrumentStudio as well.

   ![image.png](/.attachments/image-4726a668-0aa8-4596-8ae1-4c425822568c.png =850x)

7. The measurement results are updated in the Instrument Studio as below.

   ![image.png](/.attachments/image-9109658c-303e-4eda-acec-38ddfc8b1b63.png =850x)
## Measurements
### AC
### AC MultiChannel
### Linearity
### Gain and Offset
### Full Scale Error
### Channel to Channel Isolation
