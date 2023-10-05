# Unibot Wi-Fi guide

## Download and install Arduino IDE
[Guide.md | Download and install Arduino IDE](Guide.md#download-and-install-arduino-ide)

## Wi-Fi setup
Setup Windows Mobile hotspot like this:  
- Set your own Wi-Fi name and password
- Set band to 2.4 GHz  
<img src=https://i.imgur.com/Ghh0aka.png alt="Image" width="600"/>

## Control Panel setup
Set up sharing with your main connection:
- Turn on Windows Mobile hotspot
- Go to `Control Panel\Network and Internet\Network Connections`
- Go to your main network's properties
- Go to `Sharing`
- Turn on `Allow other network users to connect through this computer's Internet connection`
- Select your Wi-Fi hotspot from the dropdown
- Click `OK`  
<img src=https://i.imgur.com/kHX00BN.png alt="Image" width="400"/>

## Upload ino file to board
- Connect the board to the PC
- Open `Unibot/src/wifi/wifi.ino` with Arduino IDE
- Go to `Tools > Board` and select the board you are using 
- Go to `Tools > Port` and select the correct port
- In `wifi.ino` change variables `ssid` and `password` to match your Wi-Fi name and password
- Click `Upload`

## Check board IP
- Turn on Mobile hotspot in Windows (Also check [Control Panel setup](#control-panel-setup))
- Connect the board to the PC
- Open Mobile hotspot settings
- You should see the board and its IP in the connected devices

## Configure config
[Guide.md | Configure config](Guide.md#configure-config)

## Run Unibot
[Guide.md | Run Unibot](Guide.md#run-unibot)