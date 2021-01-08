# fireworks-docker

## 1. Setup X11

#### Install XQuartz: 
<br>

https://dl.bintray.com/xquartz/downloads/XQuartz-2.7.11.dmg


#### XQuartz setting for Mac

Start XQuartz from command line using open -a XQuartz. In the XQuartz preferences, go to the “Security” tab and make sure you’ve got “Allow connections from network clients” ticked. Then restart XQuartz

![XQuartzPreferenceSetting](docs/xquartz_preferences.png)

#### Review setting
Check tcp listening and glx is enabled with plutil command
```
 plutil -p ~/Library/Preferences/org.macosforge.xquartz.X11.plist | grep  -E tcp\|glx
```

*If* that is not the case set it command line and reboot your desktop:
```
defaults write org.macosforge.xquartz.X11.plist nolisten_tcp -bool false
defaults write org.macosforge.xquartz.X11.plist enable_iglx -bool true
```
## 2. Install Docker
Install Docker Desktop
https://hub.docker.com/editions/community/docker-ce-desktop-mac

## 3. Run cmsShow 
Get cmsShowDocker script and run with desired version of cmsShow relelease
<br>
```
curl -O https://raw.githubusercontent.com/alja/fireworks-docker/main/cmsShowDocker
cmsShowDocker cmsShow-11.21
./cmsShow data.root
```

