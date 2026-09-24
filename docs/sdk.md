# SDK Management in Arduino ProX

Arduino ProX uses platform-specific SDKs and development packages to compile projects for supported boards.

SDK management allows you to install or reinstall the required development environment for Arduino, ESP32 and ESP8266 projects.

## 📦 Supported SDKs

Arduino ProX provides support for development environments required by supported platforms, including:

- Arduino
- ESP32
- ESP8266

The available SDKs may vary depending on the version of Arduino ProX and the supported platform packages.

## 🚀 Installing an SDK

Before compiling a project, make sure the required SDK is installed.

To install an SDK:

1. Open **Arduino ProX**.
2. Open **Settings**.
3. Find the SDK management option.
4. Select the SDK required for your board or platform.
5. Start the installation.
6. Wait for the installation to complete.
7. Return to your project and try compiling again.

> SDK installation may require additional storage space. Make sure your Android device has sufficient free storage before starting the installation.

## 🔄 Reinstalling an SDK

If an SDK becomes corrupted or compilation starts failing unexpectedly, reinstalling the SDK can help restore the required development files.

Arduino ProX provides an SDK reinstall option in the app settings.

To reinstall an SDK:

1. Open **Arduino ProX**.
2. Go to **Settings**.
3. Scroll to the SDK management section.
4. Select **Reinstall SDK**.
5. Choose the required SDK if prompted.
6. Start the reinstall process.
7. Wait until the process finishes.
8. Restart or reopen your project if necessary.
9. Try compiling the project again.

## ⚠️ When Should You Reinstall an SDK?

Reinstalling an SDK may be useful when:

- Compilation suddenly stops working.
- SDK files appear to be missing.
- A board package cannot be loaded correctly.
- The SDK installation was interrupted.
- An SDK update did not complete correctly.
- Build errors continue after checking your project and libraries.

Before reinstalling, make sure the problem is actually related to the SDK.

## 💾 Storage Requirements

SDKs and development packages can require significant storage space.

Before installing or reinstalling an SDK:

- Make sure your Android device has enough free storage.
- Avoid starting an installation when storage is nearly full.
- Keep enough free space for temporary build files.

If an installation fails because of insufficient storage, free up space and try again.

## 🌐 SDK Installation Problems

SDK installation may require downloading development packages.

If the installation does not complete:

1. Check your internet connection.
2. Make sure the device has sufficient storage.
3. Close unnecessary applications.
4. Try the installation again.
5. If the problem continues, try reinstalling the SDK.

## 🔨 SDK and Compilation

The selected SDK must be compatible with the platform you are compiling for.

For example:

- Arduino project → Arduino development environment
- ESP32 project → ESP32 development environment
- ESP8266 project → ESP8266 development environment

Make sure you have selected the correct board before compiling.

## 🐛 Troubleshooting

### SDK is missing

Open Arduino ProX settings and install the required SDK.

### SDK installation failed

Check:

- Internet connection
- Available storage
- Android permissions
- Whether the installation was interrupted

Then try the installation again.

### Compilation fails after SDK installation

Check:

1. The correct board is selected.
2. The correct SDK is installed.
3. Required libraries are available.
4. Your code does not contain compilation errors.

If the problem continues, try **Reinstall SDK** from the settings.

### SDK reinstall did not solve the problem

Collect the following information:

- Android device model
- Android version
- Arduino ProX version
- Selected board
- SDK/platform
- Complete build error
- Screenshot of the error

Then open an issue in the Arduino ProX repository.

## 📋 Reporting SDK Issues

When reporting an SDK-related problem, please provide the complete error message instead of only saying:

> "SDK is not working."

Also mention:

- Which platform you were using
- Which board was selected
- What operation failed
- Whether the SDK was newly installed or reinstalled
- Whether the problem occurs with a new project

This information helps the Arduino ProX team investigate the issue.

## 📚 Related Guides

- [Getting Started](getting-started.md)
- [Arduino Development](arduino.md)
- [ESP32 Development](esp32.md)
- [ESP8266 Development](esp8266.md)
- [USB / OTG Guide](usb-otg.md)
- [Troubleshooting](troubleshooting.md)

---

**Arduino ProX**  
*Program Arduino, ESP32 and ESP8266 directly from Android.*
