# Hardened_Firefox_Forte
Firefox user.js hardening configuration to prevent anti-tracking, privacy and security when browsing the internet.

How to Install the user.js script in your browser:
Firstly ensure you have Secure_Ip_Tor_Changer from https://github.com/privateboss0/Secure_Tor_Ip_Changer installed and running or you will have to make some modifications to this script.

1) Close your Browser:

2) Download the user.js script into your download directory

a. git clone https://github.com/privateboss0/Hardened_Firefox_Forte 

4) Create a new Firefox profile to prevent any issues with your browser using the command:

b. firefox -CreateProfile privatesecure

6) Verify the profile was created using the command below. A dialog box should appear with various profiles including the one you just created. *privatesecure*

c. firefox -ProfileManager

8) Click on your created profile privatesecure and check the button *Use the selected profile without asking at startup* if it is unchecked

9) Go into Firefox hidden directory. The directory will be a random 8 strings with a .privatesecure
    
e. cd ~/.mozilla/firefox/xxxxxxxx.privatesecure

11) Copy the user.js file from your downloads to the firefox folder

f. cp /home/kali/Downloads/Secure_Docs/user.js ~/.mozilla/firefox/xxxxxxxx.privatesecure

NOTE: If you have integrated firejail and app-armor for additional browser security and microsegmentation For Step 3 and 4 use

i)  firejail firefox -ProfileManager

ii) firejail firefox -CreateProfile secure
