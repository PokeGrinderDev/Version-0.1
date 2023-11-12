# PokeGrinder Version-1.0

This program uses computer code to perform actions the same way that you would.\
The goal of this program is not to cheat, trick or manipulate the game.\
It is built to assist with the boring repetitive tasks, so game play is more fun.\
This program is not perfect, it may make some mistakes.\
Any use of this program is at your own risk.\
This program is free use with no restrictions.\
A lot of time and effort has been spent to create and improve this program.\
If you find this in any way helpful, please consider supporting this program via the embedded link.

# Features:
Automated spinning of pokestops and gyms\
Automated sending of gifts to friends\
Automated leveling of buddies\
Automated feeding of berries to gyms\
Automated trading between two devices

# Requirements:
An Android device\
A USB cable\
Pokemon GO
Scrcpy

# Initial setup:
Enable developer mode on your device (google for detailed instructions)\
Enable USB debugging\
Download and unzip PokeGrinder\
Connect your device via USB\
Run scrcpy\
Run PokeGrinder

# How to use the program:
Note: It is best to check that your friends are always sorted by 'Can receive a gift' descending and your pokemon are always sorted by 'CP' descending.

## How to find and spin pokestops:
If you have a pokestop or gym within range of your home/school/work, you can set up the program to detect and spin them\
I recommend to always zoom out and use the compass to always have a consistent north or south facing map\
Check your inventory for gifts and enter the amount in the 'Current Gifts' spinbox\
Start by checking the 'Find Stops?' checkbox and pressing 'Loop Start'\
This will tell the program to find stops but not try to spin them\
I recommend this approach until you get your screenshots set up well\
Note: If your .png images are too generic you will create false matches and if your images are too specific you will be unable to consistently detect them\
Check the pokestop_result.png file in your program folder\
Use 'Paint' or another editing software to clip an area of the pokestop for the program to detect\
Save the image as 'Poke1.png' or 'Gym1.png', it is fine to overwrite the existing file\
Repeat until you are happy with the results (Ex, if you have two pokestops, the program regularly detects two pokestops)\
Check the 'Spin Stops?' checkbox and the loop will start spinning the stops too

## How to level your buddies:
Create a tag called 'Bud1' with your buddy and two of your lowest CP pokemon\
Do the same for all of the buddies you wish to level, creating 'Bud2', 'Bud3', 'Bud4' etc.  You can use the same low level pokemons\
If you have less than 20 buddies you wish to level, set the 'Buddy limit' under 'Advanced Options' to stop at your desired buddy\
Make sure that your current buddy is 'Bud1', or edit the 'Current Buddy #' as desired\
Check the 'Level Buddy?' checkbox and press 'Loop Start'

## How to berry gyms:
Click on any friendly gym, through in game map or the 'Pokemon in Gyms' section\
Press the 'Feed Berries to Gym' button

## How to trade between two devices:
I recommend to create a tag for pokemon you want to trade and doing one manual trade to set it up\
Make sure that you are will not be prompting a special trade, the program is set to not do a special trade\
Both devices need to be connected via USB and on each others friend page\
Press 'Two Device Trading'

# Advanced details:
Device Info - This area is used for running multiple devices.\
The 'My Primary Device' textbox does not do anything but allows you to create a custom label for your instance.\
The 'Device #' spinbox tells the loop which device to run commands to.

Single Device Loop - This area is used to tell the 'Loop Start/Stop' what actions you want it to run.\
'Find Stops?' will look for stops and gyms, but not spin them.  Allowing you to configure your device without a long delay between spins.\
'Spin Stops?' will try to spin any stops and gyms that are found.\
'Level Buddy?' will try to level your buddy.

Set Current Status - This area is used to tell the program your current state and allows you to pick up where you left off, if you are resuming a session.\
'Total Spins' tracks how many spins you have attempted in this session.\
'Current Gifts' tracks how many gifts are in your inventory.  This should be manually set before you 'Loop Start' if you are already full of gifts.\
'Current Buddy' tracks your current buddy.  The program starts at 1, but it does not check to make sure your current buddy is 'Bud1'.\
'Buddy Active' tracks if you buddy is on map or not.  Zero is not active, and one is active.\
'Buddy Battle' tracks the number of battles you have done with your buddy.

Advanced Options - This area allows you to customize and set limits to your 'Loop Start/Stop'\
'Limit Gifts?' allows you to prevent sending gifts to friends with a specific nickname, set as 'cd' by default or 'no_gift.png'.\
'Spin Limit' tells the loop to stop spinning stops after a set amount of spins.\
'Buddy Limit' tells the loop to stop leveling buddy after a set amount of buddies.\
'Trade Limit' tells the 'Two Device Trading' to stop after a set amount of trades.

Other Features - These are specific functions run seperately from the 'Loop Start/Stop'.\
'Feed Berries to Gym' will attempt to feed 60 berries to a friendly gym.  Must already be in the gym screen.\
'Two Device Trading' will attempt to trade pokemon between two connected devices.  Must already be on the player friend page.

Action Log - Allows you to view the history of actions performed to help ensure the reliable running of the program.

# FAQ:
Q: Can I be banned for using this program?\
A: You risk being banned for using any third party software.  So far, we have not heard of anyone being banned for this.

Q: Do I need to have my screen on?\
A: Yes, you cannot play the game with your screen off.

Q: Do I need to keep my phone connected via USB?
A: No actually.  You can run scrcpy with parameters to connect wirelessly.  You can google it to find out how.

Q: Can I Find and Spin Stops as well as Level Buddy at the same time?\
A: Yes, but it will level your buddies a lot slower as sending gifts will be prioritized.

Q: Can I run this on multiple devices at the same time?\
A: Yes, you can connect as many devices as you like.

Q: What happens if I try to use my device while the program is running?\
A: I would not recommend it. The program will attempt clicks and swipes to re-orient itself.

Q: What if someone calls me or I need to use my phone?\
A: You can stop the loop, and the script will stop after it is finished running the current task.  If you need to use your device immediately, close the program or unplug the USB cable.

Q: My phone gets hot after extended use, what can I do?\
A: Turn the screen brightness to the lowest setting and keep your phone in a cool place.  Do not run the program too long if your phone gets hot.

Q: Can this program be used while walking around and playing Pokemon GO?\
A: This program is intended to be run while your device is connected via USB to a computer.  I wouldn't recommend walking around like that.

Q: Do I need to have a rooted phone?\
A: No, you do not need to have a rooted phone.  Any android device can run this.

Q: I get an error from scrcpy, what should I do?\
A: Most errors can be ignored.  Scrcpy is useful if you wish to watch along on your PC, but it is not required to be open.  It is used to initialize the connection to the device.

Q: I can do all of these things faster on my own.  Why do I need this program?\
A: Yes the program will likely never be more efficient than a human, but it will allow you to focus on more important things.

Q: Can you make the program catch pokemon too?\
A: Yes, but I don't plan to add that functionality.  The goal isn't to automate the entire game, just the boring parts.
