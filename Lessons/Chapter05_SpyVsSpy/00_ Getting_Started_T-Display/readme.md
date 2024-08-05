
[![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/y5Ia0OuIZ_c/0.jpg)](https://www.youtube.com/watch?v=y5Ia0OuIZ_c)

Link to Library: CLICK HERE (make sure to configure ‘User_Setup_Select.h’ before use!)
Link to add to board manager urls (copy/paste into IDE): https://raw.githubusercontent.com/espressif/arduino-esp32/gh-pages/package_esp32_index.json


Today we will be getting started with programming our T-Display and setting it up so we can program it inside of the arduino IDE. To get started, we will need the following:

A USB-C Cable
The following library (TFT_eSPI) is installed AND configured. After you install the library from the included zip file, you will want to go to where the library is installed. You can find where that is by going to the “settings” tab in the IDE and then seeing the sketchbook location. You will need to go the libraries folder, select “TFT_eSPI”, and then open “User Setup Select.h” in a text editor. You’ll need to comment out the line (27 or so) //include , then UNCOMMENT line 25 (in case it changes, it’s #include to be specific)
Add the “ESP32 Dev Module” board to the board manager by going into the IDE settings, and pasting the following (included below to copy and paste) into the additional board manager url’s:
“https://raw.githubusercontent.com/espressif/arduino-esp32/gh-pages/package_esp32_index.json”
Then you will need to change the upload speed to 4608000 baud and use 40hz instead of 80hz. If the upload speed is to high, the upload will fail.
Before you plug in the board, make sure to hold down the button to the left of the usb-c input while you plug it in to make sure it gets into “boot mode”, which will allow you to flash new code to the board
Select an example from the TFT_eSPI library and hit upload
Profit?!?!

![image](https://github.com/user-attachments/assets/cd360a3b-9fbf-4607-bb61-b32c708ad2db)

Today we will be getting started with programming our T-Display and setting it up so we can program it inside of the arduino IDE. To get started, we will need the following:

1. A USB-C Cable
2. The following library (TFT_eSPI) is installed AND configured. After you install the library from the included zip file, you will want to go to where the library is installed. You can find where that is by going to the “settings” tab in the IDE and then seeing the sketchbook location. You will need to go the libraries folder, select “TFT_eSPI”, and then open “User Setup Select.h” in a text editor. You’ll need to comment out the line (27 or so) //include <user-setup.h>, then UNCOMMENT line 25 (in case it changes, it’s #include <User_Setups/Setup25_TTGO_T_Display.h> to be specific)
3. Add the “ESP32 Dev Module” board to the board manager by going into the IDE settings, and pasting the following (included below to copy and paste) into the additional board manager url’s:
“https://raw.githubusercontent.com/espressif/arduino-esp32/gh-pages/package_esp32_index.json”
4. Then you will need to change the upload speed to 4608000 baud and use 40hz instead of 80hz. If the upload speed is to high, the upload will fail.
5. Before you plug in the board, make sure to hold down the button to the left of the usb-c input while you plug it in to make sure it gets into “boot mode”, which will allow you to flash new code to the board
6. Select an example from the TFT_eSPI library and hit upload
7. Profit?!?!
