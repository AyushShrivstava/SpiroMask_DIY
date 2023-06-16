# Configuring Arduino Nano Sense BLE to work with Edge Impulse.

## What is edge impulse?

With Edge Impulse, you can collect sensor data from edge devices, preprocess and label the data, and then use it to train machine learning models. The platform supports a wide range of sensor inputs, including accelerometers, gyroscopes, magnetometers, audio, and more. It also offers various signal processing and feature extraction capabilities to derive meaningful insights from the collected data.

## Setting up Arduino Nano Sense BLE.

Follow the steps available on Edge Impulse website to configure your Arduino Nano Sense BLE to work with Edge Impulse.
link to the website -> [Arduino Nano 33 BLE Sense](https://docs.edgeimpulse.com/docs/development-platforms/officially-supported-mcu-targets/arduino-nano-33-ble-sense)

## Setting the gain of the Arduino Nano BLE sense microphone.

We had to change the gain of the Microphone as the gain set in ```Edge Impulse firmware for Arduino Nano 33 BLE Sense``` was too high for our purposes and Audio samples were getting clipped. To change the gain of the microphone, we had to change the value of ```MIC_GAIN``` in ```Edge Impulse firmware for Arduino Nano 33 BLE Sense``` to 40 (or 30). This can be done by following the steps below:

1. Get the Edge Impulse firmware from their open sourse repository [firmware-arduino-nano-33-ble-sense](https://github.com/edgeimpulse/firmware-arduino-nano-33-ble-sense). The repository is also mentioned in the [Arduino Nano 33 BLE Sense](https://docs.edgeimpulse.com/docs/development-platforms/officially-supported-mcu-targets/arduino-nano-33-ble-sense) page of Edge Impulse website. (This information is provided here just in case the link changes in future.) A version of this also available in this repository in the folder [1.Arduino_Firmware]()

2. To set the gain of the hardware microphone, open the file ```"1.Arduino_Firmware\src\sensors\ei_microphone.cpp"``` in a text editor and change the value of ```PDM.setGain``` to 40 (or 30). Please be aware there will twice such lines in the file. Change both of them. 


3. Follow the steps mentioned in the [firmware-arduino-nano-33-ble-sense](https://github.com/edgeimpulse/firmware-arduino-nano-33-ble-sense) repository to build and flash the firmware. It is advised to follow the linux path as windows version of the build script did not work for us.

    **NOTE**: We have provided a few copies of the file with the gain set to various values in the folder [2.PreBuilt_Firmware](). You can use these files and directly flash them to the Arduino Nano board.



### **Enjoy working with Edge Impulse.**