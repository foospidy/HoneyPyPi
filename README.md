# HoneyPyPi
Setup script to make your Raspberry Pi a HoneyPy honeypot.

### How To

This assumes you have Raspbian installed on your Raspberry Pi (https://www.raspberrypi.org/downloads/raspbian/). This script should be run as root. It will create a user `honey` and install HoneyPy under that user account.

#### Usage

```
# ./HoneyPyPi 
Usage:
./HoneyPyPi [-i] [-p] [-lp]

-i        Install everything.
-p        Set/change HoneyPy service profile.
-lp       List profiles.
```

#### Install

`# ./HoneyPyPi -i`

#### Running HoneyPy

When you log into the `honey` account HoneyPy will automatically launch. You should first log into another account, either another user account or root, and run `screen` before switching to the `honey` user. Using `screen` will ensure the HoneyPy continues running if your terminal session is disconnected. Example steps:

- Login as `<your user account>` or `root`
- Run `screen`
- Switch user to honey, `su - honey`
