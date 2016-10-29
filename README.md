# HoneyPyPi
Setup script to make your Raspberry Pi a HoneyPy honeypot.

### How To

This assumes you have Raspbian installed on your Raspberry Pi (https://www.raspberrypi.org/downloads/raspbian/). This script should be run as root. It will create a user `honey` and install HoneyPy under that user account.

#### Usage

```
# ./HoneyPyPi 
Usage:
./HoneyPyPi [-i] [-p] [-lp]

-i        Install everyting.
-p        Set/change HoneyPy service profile.
-lp       List profiles.
```

#### Install

`# ./HoneyPyPi -i`
