# uecg_windows
A compiled version of uECG Node JS app, tested on Windows 10 and 7. It should let you run the web app without installing NodeJS or python.
It's compiled using pkg and theoretically there should be one file only. But for now, for some reason it doesn't work without all the other NodeJS files, so please download the whole zip and run the app from the folder.

How to use:

1. Insert black USB base into computer. It should have green and blue LEDs on.

2. After USB sound, the Windows should install drivers for CP2102 chip (it's the USB chip used on the base).

3. If it didn't install drivers, download drivers here https://www.silabs.com/documents/public/software/CP210x_Windows_Drivers.zip and install them.
 - to install drivers, click on **CP210xVCPInstaller_x64.exe** from the zip you downloaded in step 3.
 
4. Now, download zip with uECG windows app from this github (this one https://github.com/ultimaterobotics/uecg_windows/raw/main/uecg_win10.zip)

5. To launch app, click on green **uecg_app.exe** file. Black terminal will open and show that it sees the COM port, etc. It means it sees the USB base. Do not close the terminal while you use uECG, it is running the app. Also, at this point it may show a window asking about Firewall, just allow it. 

6. After that, in your browser, open this address http://127.0.0.1:8080 - you should see black/green uecg app.

7. Now, you need to turn on the uECG device. After it blinks with pink LED, press button on uECG **two times quickly**. It should blink with green and you will see signal in Windows app! Also, the USB base will slowly pulse with red LED when uECG is in correct mode.

8. To close the app, close the black terminal.
