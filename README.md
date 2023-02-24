# Linux Permission Script
A script for granting Linux permissions to the RadarIQ sensor when accessed via the USB port.

## Usage
```
git clone https://github.com/radariq/linux-permission-script
cd linux-permission-script
chmod +x setup.sh
./setup.sh
```

Disconnect and reconnect the RadarIQ sensor.

Check the permissions have been granted

```ls -la /dev | grep ttyACM*```

The result will look something like this depending on what other devices you have plugged in to the USB port.
```
lrwxrwxrwx  1   root    root    radariq->ttyACM0
lrwxrwxrwx  1   root    dialout ttyACM0

```