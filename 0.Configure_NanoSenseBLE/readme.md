# Configuring Arduino Nano Sense BLE

## What is Edge Impulse?

 Edge Impulse is a platform that enables you to collect sensor data from edge devices, preprocess and label the data, and train machine learning models. It supports various sensors like accelerometers, gyroscopes, magnetometers, and audio.

## Configuring Arduino Nano Sense BLE to work with Edge Impulse

1. To set up your Arduino Nano Sense BLE with Edge Impulse, follow the instructions provided on the Edge Impulse website. You can find specific guidance for the Arduino Nano 33 BLE Sense [here](https://docs.edgeimpulse.com/docs/development-platforms/officially-supported-mcu-targets/arduino-nano-33-ble-sense).

2. Adjusting the gain of the Arduino Nano BLE Sense microphone may be necessary to prevent audio clipping. This can be done by modifying the Edge Impulse firmware for Arduino Nano 33 BLE Sense.

   - Obtain the Edge Impulse firmware from their open-source repository [firmware-arduino-nano-33-ble-sense](https://github.com/edgeimpulse/firmware-arduino-nano-33-ble-sense).

   - Locate the file "ei_microphone.cpp" in the "src/sensors" folder of the firmware.  

   - Open the file in a text editor and change the value of "PDM.setGain" to 40. Update both occurrences of this line in the file. 

   - Save the file after making the changes.   

3. Build and flash the modified firmware to your Arduino Nano board by following the instructions provided in the [firmware-arduino-nano-33-ble-sense](https://github.com/edgeimpulse/firmware-arduino-nano-33-ble-sense) repository. If you encounter any issues, it is recommended to use the Linux path for building the firmware.

Alternatively, you can use the pre-built firmware files provided in the "2.PreBuilt_Firmware" folder, where different gain values have been set. Flashing these files directly to your Arduino Nano board can save you the trouble of modifying and building the firmware.

By following these steps, you will be able to configure your Arduino Nano Sense BLE to work seamlessly with Edge Impulse.

### **Enjoy working with Edge Impulse!**