# uecg_windows
A compiled version of uECG Node JS app, tested on Windows 10 and 7. It should let you run the web app without installing NodeJS or python.
It's compiled using pkg and theoretically there should be one file only. But for now, for some reason it doesn't work without all the other NodeJS files, so please download the whole zip and run the app from the folder.

How to install and use with uECG (first time):

1. Insert black USB base into computer. It should have green and blue LEDs on.

2. After USB sound, the Windows should install drivers for CP2102 chip (it's the USB chip used on the base).

*(optional step)*

*3. If it didn't install drivers, download drivers here https://www.silabs.com/documents/public/software/CP210x_Windows_Drivers.zip and install them.*

 *- to install drivers, click on **CP210xVCPInstaller_x64.exe** from the zip you downloaded in step 3.*
 
4. Now, download zip with uECG windows app from this github (this one https://github.com/ultimaterobotics/uecg_windows/raw/main/uecg_win10.zip)

5. To launch app, click on green **uecg_app.exe** file. Black terminal will open and show that it sees the COM port, etc. It means it sees the USB base. Do not close the terminal while you use uECG, it is running the app. Also, at this point it may show a window asking about Firewall, just allow it. 

6. After that, in your browser, open this address http://127.0.0.1:8080 - you should see black/green uecg app.

7. Now, you need to turn on the uECG device. After it blinks with pink LED, press button on uECG **two times quickly**. It should blink with green and you will see signal in Windows app! Also, the USB base will slowly pulse with red LED when uECG is in correct mode.

8. To close the app, close the black terminal.

*(optional step)*

*9. Also, you can make a shortcut on the Desktop for the uecg_app.exe - just click on it, select **Send to -> Desktop (create shortcut)** and it will appear on Desktop.*


How to use with uECG every time (after first time):

1. Insert black USB base into computer. It should have green and blue LEDs on.
2. Click on green **uecg_app.exe** file from folder or Desktop, if you made a shortcut in step 9. Black terminal will open, do not close the terminal when you use app. 
3. Go to http://127.0.0.1:8080 in your browser
4. Turn on uECG device with on/off switch on the side and then with button, short press once.
5. Double press uECG button to switch into PC mode. You should see ECG signal in browser.
6. When you finish, turn off uECG with button (long press), then with switch. And close the black terminal.
