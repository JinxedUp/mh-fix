# Mineheart unable to join fix
A simple troubleshooting guide for players who are unable to connect to the server.

## ✅ 1. Make sure you are using the correct minecraft version
Mineheart currently supports multiple 1.21 versions, try joining with the latest version available

## ✅ 2. check if the server is online
Sometimes temporary maintenance or restarts can cause connection issues

Before troubleshooting, its best to:
- Check the server's Discord announcements
- The error you got while attempting to join


# Actual troubleshooting part

## ✅ 3. fix “Unable to Connect to World” (Bedrock)
If youre on bedrock and unable to join try to:
1. Close minecraft fully
2. Restart your device
3. Add the server again manually:
- Name: MineHeart
- IP: play.mineheart.net
- Port: 19132

## ✅ 4. Flush DNS (Recommended)
if you get stuck on "Connecting..." or "loading terrain" this often fixes it
1. Press **Win + R** at the same time
2. Type "cmd" in the window that pops up
3. Press Enter
4. inside of the cmd type and run "ipconfig /flushdns"

## ✅ 5. Disable VPN / Mobile Hotspot
VPNs, Hotel wifi or mobile hotspots can block certain ports, try switching to another network

# Connection timed out: getsockopt
That's the most common issue weve had so far with players so it needs its own special category.

## ✅ 1. Restart your router + your PC
Simple but its an 50% chance this works

## ✅ 2. Disable Windows Firewall temporarily
Windows Firewall sometimes block outbound minecraft connections (this should be done only temporarily and at your owns risk)

1. Open Windows Defender Firewall
2. Press on "Turn Windows Defender Firewall on or off"
3. Turn off Firewall 
4. Try joining the server again
- if it works,add Minecraft as an allowed app

## ✅ 3. Make sure Java/Minecraft is allowed in Firewall
1. Search "allow an app through Windows firewall"
2. Find Java Platform SE Binary AND Minecraft launcher
3. Allow BOTH Private + Public networks

## ✅ 4. Check if your PC is using a VPN/Proxy
a vpn or proxy can break Minecraft connections.
Turn off VPN or Proxy

## ✅ 5. Flush DNS
Your PC may be resolving the wrong IP.
1. open cmd as admin then run these commands in order:
```
ipconfig /flushdns
ipconfig /release
ipconfig /renew
```

## ✅ 6. Delete Minecraft cache
1. press "Win + R" at the same time
2. type in the box "%appdata%/.minecraft" and press enter
3. delete the folders named "assets" and "libraries"
4. restart minecraft


## ✅ 7. Redownload Minecraft and Minecraft Launcher
Try to delete your Minecraft version then your Minecraft launcher, restart your PC then redownload both and try rejoining

## ✅ 8. Reset the network stack
open cmd as admin and run in order:
```
netsh winsock reset
netsh int ip reset
ipconfig /flushdns
ipconfig /release
ipconfig /renew
```

# 🟦 If all else fails
If none of the above helped, open a support ticket and include:
- Your username
- your version (java/bedrock + version number)
- screenshot of the error
- your region

- other information (Eg. if other people on the same network as you can join with different devices)

(join the help server with the following link: https://discord.gg/EAuJbbsx2s)
This helps staff resolve your issue much faster.

## IF STAFF CANT HELP YOU EITHER
If all attempts you done here or with staff have failed, there are only 2 ways left to fix this:
1.
- Contact your ISP (Internet Provider) and explain this issue

2.
- Reinstall windows completly from the start (this might not fix it but it has the highest chances)


### Last Updated: *November 25 2025*  
Maintained by: **Jinxedup_** (MineHeart Staff)
