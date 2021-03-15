"# fake-access-points-using-scapy"
#Recommended you use Linux

#To use the scripts, clone into the repository
git clone https://github.com/Austinstevesk/fake-access-points-using-scapy.git
cd fake-access-points-using-scapy

#Install necessary packages
pip3 install -r requirements.txt

#Install aircrack
apt-get install aircrack-ng

#Enable monitor mode using aircrack-ng
root@austin:~# airmon-ng check kill

root@austin:~# airmon-ng start wlan0
    -Be careful with the interface, not all devices run on the wlan0 interface. Use ifconfig to get your corrent interface

#You are now set to run the file
$python3 fakeap.py
    -This creates one BSSID
$python3 multiplefakeaps.py
    -Creates five BSSIDs



