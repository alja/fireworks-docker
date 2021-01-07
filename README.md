# fireworks-docker

## Install XQuartz: 
<br>

https://dl.bintray.com/xquartz/downloads/XQuartz-2.7.11.dmg

# Setup XQuartz:
    Start XQuartz and then go to settings (Apple + ,) and go to Security tab, and make sure you've got "Allow connections from network clients" ticked.
# Then restart iQuartz.

## XQuartz setting for Mac

Start XQuartz from command line using open -a XQuartz. In the XQuartz preferences, go to the “Security” tab and make sure you’ve got “Allow connections from network clients” ticked:

![XQuartzPreferenceSetting](docs/xquartz_preferences.png)



docker pull sgnoohc/fireworks:9.4.1
git clone https://github.com/sgnoohc/cmsdas2021visualization.git
cd cmsdas2021visualization
sh get_sample_commands.sh YOUR_LPC_USERNAME
./cmsShowDocker rootfiles/dy.root

