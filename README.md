# SteamDeck Logo Changer

A simple shell script to easily change the BGRT logo when the Steam Deck powers on!

Credits to Discord user balika011 for the idea! I scripted it to make it easy to change / restore the BGRT logo.

> **NOTE**\
> If you are going to use this script for a video tutorial, PLEASE reference on your video where you got the script! This will make the support process easier!
> And don't forget to give a shoutout to [@10MinuteSteamDeckGamer](https://www.youtube.com/@10MinuteSteamDeckGamer/) / ryanrudolf from the Philippines!
>

<b> If you like my work please show support by subscribing to my [YouTube channel @10MinuteSteamDeckGamer.](https://www.youtube.com/@10MinuteSteamDeckGamer/) </b> <br>
<b> I'm just passionate about Linux, Windows, how stuff works, and playing retro and modern video games on my Steam Deck! </b>
<p align="center">
<a href="https://www.youtube.com/@10MinuteSteamDeckGamer/"> <img src="https://github.com/ryanrudolfoba/SteamDeck-Logo-Changer/blob/main/10minute.png"/> </a>
</p>

<b>Monetary donations are also encouraged if you find this project helpful. Your donation inspires me to continue research on the Steam Deck! Clover script, 70Hz mod, SteamOS microSD, Secure Boot, etc.</b>

<b>Scan the QR code or click the image below to visit my donation page.</b>

<p align="center">
<a href="https://www.paypal.com/donate/?business=VSMP49KYGADT4&no_recurring=0&item_name=Your+donation+inspires+me+to+continue+research+on+the+Steam+Deck%21%0AClover+script%2C+70Hz+mod%2C+SteamOS+microSD%2C+Secure+Boot%2C+etc.%0A%0A&currency_code=CAD"> <img src="https://github.com/ryanrudolfoba/SteamDeck-Clover-dualboot/blob/main/QRCode.png"/> </a>
</p>

## Disclaimer
1. Do this at your own risk!
2. This is for educational and research purposes only!

## [Video Tutorial - How to Use this Script to Change the Steam Deck Logo](https://youtu.be/-pBlEceVZs8)
[Click the image below for a video tutorial!](https://youtu.be/-pBlEceVZs8)
</b>
<p align="center">
<a href="https://youtu.be/-pBlEceVZs8"> <img src="https://github.com/ryanrudolfoba/SteamDeck-Logo-Changer/blob/main/banner.png"/> </a>
</p>

## WARNING
This has been tested on BIOS 116 and BIOS118.

## What's New (as of September 21 2023)
1. initial release

## Prerequisites for SteamOS
1. sudo password should already be set by the end user. If sudo password is not yet set, the script will ask to set it up.

## Installation Steps
1. Go into Desktop Mode and open a konsole terminal.
2. Clone the github repo. \
   cd ~/ \
   git clone https://github.com/ryanrudolfoba/SteamDeck-Logo-Changer.git
3. Execute the script! \
   cd ~/SteamDeck-Logo-Changer \
   chmod +x steamdeck-logo-changer.sh \
   ./steamdeck-logo-changer.sh
   
4. The script will check if sudo passwword is already set.\
![image](https://github.com/ryanrudolfoba/SteamDeck-Logo-Changer/assets/98122529/1180b8a2-3c98-47ef-8fb1-1adc1f5ed470)

   a. If the sudo password is already set, enter the current sudo password and the script will continue to run and the main menu will be displayed. \
   ![image](https://github.com/ryanrudolfoba/SteamDeck-Logo-Changer/assets/98122529/004395f6-d69b-48d2-9a8a-b9621668901b)

   b. If wrong sudo password is provided the script will show an error message. Re-run the script and enter the correct sudo password!\
   ![image](https://github.com/ryanrudolfoba/SteamDeck-Logo-Changer/assets/98122529/9566eb35-174b-43d5-b203-00ec3954db76)
         
   c. If the sudo password is blank / not yet set, the script will prompt to setup the sudo password. Re-run the script again to continue.\
   ![image](https://github.com/ryanrudolfoba/SteamDeck-Logo-Changer/assets/98122529/1cf6bb68-f9c8-48b0-91ec-ef75d1ddd9ea)


6. Main menu. Make your selection.\
![image](https://github.com/ryanrudolfoba/SteamDeck-Logo-Changer/assets/98122529/4717ac87-82cf-4fad-872f-7688953b4865)

7. Click the Logo button and then press OK. A list of available logos will be displayed. Choose the one that will be set as the default logo and press OK. \
![image](https://github.com/ryanrudolfoba/SteamDeck-Logo-Changer/assets/98122529/4075909c-6a8d-4242-be83-e70f217d4e7f)
![image](https://github.com/ryanrudolfoba/SteamDeck-Logo-Changer/assets/98122529/75161f11-3e21-4f35-89b0-dbdf7a161dcc)
![image](https://github.com/ryanrudolfoba/SteamDeck-Logo-Changer/assets/98122529/7368f6ac-25f3-40a8-af47-bb8c00c076e5)

     
8. Press the EXIT button then press OK to close the application.
9. Reboot the Steam Deck for changes to take effect! 

## I want to use my own logos!
If you want to use your own logos it is very easy!
* Grab your favorite logo / picture and make sure it is in the PNG format.
* The resolution should not exceed 1280x800.
* Place them in the logos folder.
* Run the script and it will automatically pick up the new logos!

## How to Restore the Default Logo
1. To restore the default logo, run the script and click the Restore button then press OK.
![image](https://github.com/ryanrudolfoba/SteamDeck-dualboot/assets/98122529/3d32c1e3-4fca-40f1-9897-76f4d016a851)
![image](https://github.com/ryanrudolfoba/SteamDeck-dualboot/assets/98122529/8f6be37e-09cc-4746-86e1-c6daff03a35d)

2. Reboot the Steam Deck for changes to take effect!
