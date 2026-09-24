# ESP32 Development with Arduino ProX

Arduino ProX lets you write, compile and upload ESP32 sketches directly from your Android device.

This guide explains how to set up an ESP32 project, select the correct board, compile your code and upload it to your ESP32 board.

## 📱 What You Need

Before starting, make sure you have:

- An Android phone or tablet
- Arduino ProX installed
- An ESP32 development board
- A compatible USB cable
- USB OTG support or a compatible USB connection

## 🚀 Getting Started

### 1. Open Arduino ProX

Launch Arduino ProX on your Android device.

Create a new project or open an existing Arduino project.

### 2. Select ESP32

Open the board selection menu and select the ESP32 platform.

Choose the ESP32 board that matches your hardware.

For example:

- ESP32 Dev Module
- DOIT ESP32 DEVKIT V1
- Other supported ESP32 boards

> Always select the board that matches your actual hardware. Different ESP32 boards can have different hardware configurations.

## 📦 Install the ESP32 SDK

Arduino ProX requires the appropriate ESP32 development package to compile ESP32 projects.

If the required SDK is not installed:

1. Open Arduino ProX settings.
2. Find the SDK or board package management option.
3. Install the required ESP32 SDK.
4. Wait for the installation to complete.
5. Return to your project and select the ESP32 board again.

### Reinstalling the SDK

If ESP32 compilation starts failing unexpectedly or the SDK appears to be corrupted:

1. Open **Settings** in Arduino ProX.
2. Find **Reinstall SDK**.
3. Select the appropriate SDK.
4. Start the reinstall process.
5. Wait until the installation is complete.
6. Try compiling the project again.

## 🧩 Configure the ESP32 Board

After selecting your ESP32 board, Arduino ProX may provide configuration options depending on the selected board and ESP32 platform.

Common configuration options can include:

- Board
- Flash size
- Partition scheme
- Upload speed
- CPU frequency
- Flash mode
- PSRAM
- Other board-specific options

Only change these options when you know they are appropriate for your hardware.

## ✍️ Write Your Code

Create or open your `.ino` sketch and write your ESP32 code using the Arduino ProX code editor.

For example:

```cpp
void setup() {
    Serial.begin(115200);
}

void loop() {
    Serial.println("Hello from ESP32!");
    delay(1000);
}
