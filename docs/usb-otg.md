# USB OTG Programming with Arduino ProX

Arduino ProX can communicate with supported Arduino, ESP32 and ESP8266 boards through a wired USB connection using Android USB OTG.

This guide explains how to connect a development board to an Android device and troubleshoot common USB OTG problems.

## 🔌 What is USB OTG?

USB OTG (On-The-Go) allows an Android device to act as a USB host and communicate with external USB devices such as development boards.

With a compatible OTG connection, you can connect your Arduino, ESP32 or ESP8266 board directly to your Android device.

## 📱 What You Need

Before connecting your board, make sure you have:

- An Android phone or tablet with USB OTG support
- Arduino ProX installed
- A supported development board
- A compatible USB OTG adapter or OTG cable
- A USB data cable

> Make sure your USB cable supports data transfer. Some USB cables are designed only for charging.

## 🔗 Connecting Your Board

### USB-C Android Devices

For an Android device with a USB-C port, you can generally use:

**Android device → USB-C OTG adapter/cable → USB cable → Development board**

### Micro-USB Android Devices

For devices with a Micro-USB port, you may need:

**Android device → Micro-USB OTG adapter → USB cable → Development board**

The exact cable or adapter depends on the connectors used by your Android device and development board.

## 🚀 Connecting a Board

Follow these steps:

1. Connect the OTG adapter or OTG cable to your Android device.
2. Connect the development board using a suitable USB data cable.
3. Power on the board if required.
4. Open Arduino ProX.
5. Select the appropriate board.
6. Start the compile or upload process.
7. If Android asks for USB permission, allow Arduino ProX to access the connected USB device.

## 🔐 USB Permission

Android may display a USB permission dialog when a development board is connected.

If a permission request appears:

1. Check that the connected device is your development board.
2. Allow Arduino ProX to access the USB device.
3. Continue with the upload process.

If the board is disconnected and connected again, Android may request permission again depending on the device and USB configuration.

## ⚡ Power Considerations

Some development boards draw power directly from the USB connection.

Depending on the Android device and board, the phone may need to supply power to the connected USB device.

If the board does not power on or repeatedly disconnects:

- Check the USB cable.
- Try another OTG adapter.
- Make sure the Android device supports OTG.
- Check whether the board requires more power than the Android device can provide.
- If necessary, use a suitable externally powered USB setup.

## 🧪 Test the Connection

After connecting the board:

1. Open Arduino ProX.
2. Select the correct board.
3. Check whether the USB device is detected.
4. Compile a simple project.
5. Start the upload process.

If the board is detected and the upload completes successfully, the USB OTG connection is working correctly.

## 🐛 Troubleshooting

### Board is not detected

Try the following:

1. Disconnect the board.
2. Disconnect the OTG adapter.
3. Reconnect the OTG adapter to the Android device.
4. Connect the board again.
5. Check for an Android USB permission dialog.
6. Open Arduino ProX and try again.

### Android does not show a USB permission dialog

Check:

- OTG is supported by your Android device.
- The OTG adapter is working.
- The USB cable supports data transfer.
- The board is powered.
- The USB connector is properly inserted.

Try another USB cable or OTG adapter if available.

### Board keeps disconnecting

Possible causes include:

- Poor-quality USB cable
- Loose connection
- Insufficient USB power
- Faulty OTG adapter
- Power consumption of the connected board or peripherals

Try using another cable or adapter and disconnect unnecessary USB peripherals.

### Upload fails even though the board is detected

Check:

- Correct board is selected.
- Correct SDK is installed.
- USB connection is stable.
- Required drivers or board support are available through the selected platform.
- The board is in the correct upload mode if required.

Some development boards may require pressing a **BOOT**, **FLASH**, or similar button during the upload process.

### Upload gets stuck

Try:

1. Cancel the current operation.
2. Disconnect the board.
3. Reconnect the board.
4. Verify the selected board.
5. Start the upload again.
6. If required, use the board's BOOT/FLASH button during upload.

## 🔧 Tips for Reliable USB OTG Programming

For the best experience:

- Use a good-quality USB data cable.
- Use a reliable OTG adapter.
- Keep the USB connection stable during uploading.
- Avoid moving the phone or board while uploading.
- Make sure your Android device has sufficient battery.
- Disconnect unnecessary USB devices.
- Keep Arduino ProX updated.

## 📋 Before Reporting a USB Issue

If USB OTG programming is not working, collect the following information:

- Android device model
- Android version
- Arduino ProX version
- Board name
- USB cable type
- OTG adapter type, if applicable
- Whether Android detects the USB device
- Error message from Arduino ProX
- Screenshot of the error, if possible

This information can help identify whether the problem is related to the Android device, USB connection, board configuration or Arduino ProX.

## 🐞 Report a Problem

If the problem continues, open an issue in the Arduino ProX repository and include the information above.

## 📚 Related Guides

- [Getting Started](getting-started.md)
- [Arduino Development](arduino.md)
- [ESP32 Development](esp32.md)
- [ESP8266 Development](esp8266.md)
- [SDK Management](sdk.md)
- [Troubleshooting](troubleshooting.md)

---

**Arduino ProX**  
*Program Arduino, ESP32 and ESP8266 directly from Android.*
