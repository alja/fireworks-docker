# Fireworks Docker Solution

## macOS

### Docker

First install Docker Desktop

Once installed open a terminal and pull the docker image

    docker pull sgnoohc/fireworks:9.4.1

### XQuartz setting for Mac

Start XQuartz from command line using open -a XQuartz. In the XQuartz preferences, go to the “Security” tab and make sure you’ve got “Allow connections from network clients” ticked:

![XQuartzPreferenceSetting](docs/xquartz_preferences.png)

### Running cmsShow

Assuming the user already has a miniAOD file to view (with an appropriate CMSSW version)

    ./cmsShowDocker FILE.root
