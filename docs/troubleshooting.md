# Troubleshooting Arduino ProX

Having a problem with Arduino ProX?

This guide covers common issues related to SDK installation, compilation, USB connections and uploading projects to Arduino, ESP32 and ESP8266 boards.

If your problem is not covered here, you can report it through the Arduino ProX GitHub repository.

---

## 🔍 Before Troubleshooting

Before trying advanced troubleshooting steps, make sure:

- Arduino ProX is updated to the latest available version.
- The correct board is selected.
- The required SDK is installed.
- Your Android device has sufficient free storage.
- Your USB cable supports data transfer.
- USB OTG is supported and enabled on your Android device.
- The development board is powered correctly.

---

# 📦 SDK Problems

## SDK is missing

If Arduino ProX reports that an SDK is missing:

1. Open **Settings**.
2. Find the SDK management section.
3. Install the required SDK.
4. Wait for the installation to finish.
5. Return to your project.
6. Try compiling again.

See the [SDK Management Guide](sdk.md).

---

## SDK installation fails

If an SDK installation does not complete:

### Check your internet connection

SDK packages may need to be downloaded before they can be installed.

Make sure your Android device has a stable internet connection.

### Check available storage

SDKs and build files can require significant storage space.

Free up storage if your device is running low on space.

### Try again

Close unnecessary applications and start the SDK installation again.

If the problem continues, try using the **Reinstall SDK** option in Arduino ProX settings.

---

## Reinstall SDK

If compilation worked previously but suddenly starts failing, reinstalling the relevant SDK may help.

Go to:

**Settings → Reinstall SDK**

Select the required SDK and wait for the process to finish.

After the reinstall completes, try compiling the project again.

---

# 🔨 Compilation Problems

## Compilation fails

If your project fails to compile:

1. Check the build output.
2. Read the first error reported by the compiler.
3. Verify that the correct board is selected.
4. Make sure the required SDK is installed.
5. Check that all required libraries are available.
6. Check your source code for syntax errors.

Avoid focusing only on the final error line. Earlier errors can often be the actual cause of the failure.

---

## Library not found

If the compiler reports that a library cannot be found:

1. Check the library name.
2. Make sure the library is installed or available to the project.
3. Verify the `#include` statement.
4. Check whether the library supports your selected board.
5. Compile the project again.

Example:

```cpp
#include <ExampleLibrary.h>
