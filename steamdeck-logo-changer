#!/bin/bash

clear

echo Steam Deck Logo Changer - script by ryanrudolf
echo https://github.com/ryanrudolfoba/SteamDeck-Logo-Changer
echo Discord user balika011 for the idea!
sleep 2

# Password sanity check - make sure sudo password is already set by end user!
if [ "$(passwd --status $(whoami) | tr -s " " | cut -d " " -f 2)" == "P" ]
then
	PASSWORD=$(zenity --password --title "sudo Password Authentication")
	echo $PASSWORD | sudo -kS ls &> /dev/null
	if [ $? -ne 0 ]
	then
		echo sudo password is wrong! | \
		zenity --text-info --title "Steam Deck Logo Changer" --width 400 --height 200
		exit
	fi

else
	echo -e "$RED"Sudo password is blank! Setup a sudo password first and then re-run script!
	passwd
	exit
fi

while true
do
Choice=$(zenity --width 750 --height 250 --list --radiolist --multiple 	--title "Steam Deck Logo Changer  - https://github.com/ryanrudolfoba/SteamDeck-Logo-Changer"\
	--column "Select One" \
	--column "Option" \
	--column="Description - Read this carefully!"\
	FALSE Logo "Change the logo that will be displayed when powering on the Steam Deck."\
	FALSE Restore "Restore the default original logo."\
	TRUE EXIT "***** Exit this script *****")

if [ $? -eq 1 ] || [ "$Choice" == "EXIT" ]
then
	echo User pressed CANCEL / EXIT. Goodbye!
	exit

elif [ "$Choice" == "Restore" ]
then
	echo $PASSWORD | sudo -kS rm /esp/efi/steamos/steamos.png
	zenity --warning --title "Steam Deck Logo Changer" --text "Logo has been restored to the default!" --width 400 --height 75

elif [ "$Choice" == "Logo" ]
then
Logo_Choice=$(zenity --title "Steam Deck Logo Changer" --width 400 --height 400 --list \
	--column "Logo  Name" $(ls -l $(pwd)/logos/*.png | cut -d "/" -f 6) )
	if [ $? -eq 1 ]
	then
		echo User pressed CANCEL. Goodbye!
		exit
	else
		echo $PASSWORD | sudo -kS cp $(pwd)/logos/$Logo_Choice /esp/efi/steamos/steamos.png
		zenity --warning --title "Steam Deck Logo Changer" --text "Logo has been changed to $Logo_Choice!" --width 400 --height 75
	fi
fi
done
