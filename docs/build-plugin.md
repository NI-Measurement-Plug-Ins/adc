## Build EXE for each measurement
Breif explanation on how to create a build for dcvm measurement .exe's along with the digital server .exe by taking AC measurement as an example.
1. Open the adc_acMeasurement.lvproj from "data-converter-validation-module\source\measurements\ac" location
    
    ![alt text](images/adc_ac_lvproj.JPG)

2. Expand the build Specification and open adc_acMeasurement.

    ![alt text](images/adc_ac_buildSpec.JPG)

3. click 'build'.
    
    ![alt text](images/adc_ac_Build.JPG)

4. Once the build is completed, can able to see below window and with explore you can able to go to build created location
    
    ![alt text](images/adc_ac_buildCre.JPG)

5. The AC measurement build folder created under "data-converter-validation-module\Builds"
    
    ![alt text](images/dcvm_exe.JPG)

6. Go to "C:data-converter-validation-module\source\shared\digitalInterface\server" Open digital server and create .exe as steps mentioned above.

7.Continue to do for all measurements (Linearity, Gain and Offset, Channel to Channel Isolation, FSE)
    
Note: Please note that the /build folder must not be committed to repo and will be ignored by .gitignore upon commit.


## Build NIPKG for the plugin

1. Open the adc-measurements.pbs NI package build spec in "data-converter-validation-module\package"
    
    ![alt text](images/dcvm_ni_package.PNG)

2. Ensure the destination for the package installation is set to the below location:
    "C:\ProgramData\National Instruments\MeasurementLink\Services"

    ![alt text](images/dcvm_ni_package.PNG)

3. Click on 'Build Solution'.

    ![alt text](images/build_specc.PNG)

4. Once the build process is completed, the package build files and processing folder created in the package folder.
    
   
    ![alt text](images/package file.PNG)

5. Select the package file "data-converter-validation-module_1.0.0.0_windows_x64" to install the dcvm build into the machine.

    ![alt text](images/install_package.PNG)

    
Note: Please note that the built NIPM packages must not be committed to repo. The folders created upon building NI PKG (Packages, ProcessingStage) will be ignored by .gitignore upon commit.


## Create and Update NIPM Feeds
1. The NIPM packages for different measurement plugins are added to an NIPM feed. So the users can install new packages or receive updates on existing feeds by subscribing to the feed.

2. The feeds for Measurement plugins are maintained under the below repo.
https://github.com/NI-MeasurementLink-Plug-Ins/package-manager-feeds

3. Please follow the procedure mentioned in below document for adding new packages or updating new versions of existing packages to the feed.
https://github.com/NI-MeasurementLink-Plug-Ins/package-manager-feeds/blob/main/package-feed-updater/README.md



