# Arduino Development with Arduino ProX

Arduino ProX lets you write, compile and upload Arduino projects directly from your Android device.

Arduino ProX supports Arduino boards across the Arduino platform, allowing you to work with Arduino projects without requiring a traditional desktop IDE for supported workflows.

## 📱 What You Need

Before getting started, make sure you have:

- An Android phone or tablet
- Arduino ProX installed
- A supported Arduino board
- A compatible USB cable
- USB OTG support or a compatible USB connection

## 🚀 Getting Started

### 1. Open Arduino ProX

Launch Arduino ProX on your Android device.

Create a new project or open an existing Arduino project.

### 2. Select Your Arduino Board

Open the board selection menu and select the Arduino board you are using.

Make sure the selected board matches your actual hardware.

Arduino ProX supports Arduino boards across the Arduino platform.

## 📦 Install the Required SDK

Arduino ProX requires the appropriate development SDK for compiling your Arduino project.

If the required SDK is not installed:

1. Open Arduino ProX settings.
2. Find the SDK management option.
3. Install the required SDK.
4. Wait for the installation to complete.
5. Return to your project.

### Reinstalling the SDK

If compilation starts failing unexpectedly or the SDK appears to be damaged:

1. Open **Settings** in Arduino ProX.
2. Find **Reinstall SDK**.
3. Select the required SDK.
4. Start the reinstall process.
5. Wait until the installation is complete.
6. Try compiling the project again.

## ✍️ Write Your Arduino Code

Create or open your `.ino` sketch and write your code using the Arduino ProX code editor.

Example:

```cpp
void setup() {
    pinMode(LED_BUILTIN, OUTPUT);
}

void loop() {
    digitalWrite(LED_BUILTIN, HIGH);
    delay(1000);

    digitalWrite(LED_BUILTIN, LOW);
    delay(1000);
}
