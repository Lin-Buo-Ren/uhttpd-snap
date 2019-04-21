# Unofficial Snap Packaging for uhttpd
<!--
	Use the Staticaly service for easy access to in-repo pictures:
	https://www.staticaly.com/
-->
![(Placeholder) Icon of uhttpd](https://cdn.staticaly.com/gh/Lin-Buo-Ren/snapcrafters-template-plus/bea3bc56/snap/gui/my-awesome-app.png "(Placeholder) Icon of uhttpd")

**This is the unofficial snap for uhttpd**, *"A laughably-small HTTP server"*. It works on Ubuntu, Fedora, Debian, and other major Linux distributions.

[![Build Status Badge of the `uhttpd` Snap](https://build.snapcraft.io/badge/Lin-Buo-Ren/uhttpd-snap.svg "Build Status of the `uhttpd` snap")](https://build.snapcraft.io/user/Lin-Buo-Ren/uhttpd-snap)

<!-- Uncomment and modify this when you have a screenshot
![Screenshot of the Snapped Application](local/screenshots/screenshot.png "Screenshot of the Snapped Application")
-->

Published for <img src="http://anything.codes/slack-emoji-for-techies/emoji/tux.png" align="top" width="24" /> with 💝 by Snapcrafters

## Installation
([Don't have snapd installed?](https://snapcraft.io/docs/core/install))

### In a Terminal
    # Install the snap #
    sudo snap install --channel=beta uhttpd
    #sudo snap install uhttpd
    
    # Launch the application #
    snap start uhttpd

    # Put some files to the document root directory #
    sudo sh -c 'printf "<h1>Hello uhttpd snap</h1>\n" > /var/snap/uhttpd/common/index.html'
    
    # Profit #
    xdg-open http://localhost:80

### The Graphical Way
[![Get it from the Snap Store](https://snapcraft.io/static/images/badges/en/snap-store-black.svg)](https://snapcraft.io/uhttpd)

## Configuration
### Customize the listening port(Default: 80)
    sudo snap set uhttpd listening-port=8080

### Customize the serving directory(Default: /var/snap/uhttpd/common) (EXPERIMENTAL, likely won't work)
    sudo snap set uhttpd document-root-dir=/media/USB

## What is Working
* Launch
* Serve static content
* Show directory listing

## What is NOT Working...yet 
Check out the [issue tracker](https://github.com/Lin-Buo-Ren/uhttpd-snap/issues) for known issues.

## Support
* Report issues regarding using this snap to the issue tracker:  
  <https://github.com/Lin-Buo-Ren/uhttpd-snap/issues>
* You may also post on the Snapcraft Forum, under the `snap` topic category:  
  <https://forum.snapcraft.io/c/snap>
