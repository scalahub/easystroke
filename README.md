# easystroke
X11 gesture recognition application

To build on Ubuntu 16.04:

- Install dependencies:
```
sudo apt-get install g++ libboost-serialization-dev libgtkmm-3.0-dev libxtst-dev libdbus-glib-1-dev intltool xserver-xorg-dev
```

- Patch the code based on [this discussion](https://askubuntu.com/questions/932946/need-help-with-c-application-on-ubuntu-gnome-17-04). The patch file is [here](https://github.com/scalahub/easystroke/blob/master/sigc.patch)
```
patch -p1 -i sigc.patch
```

- Build the code
```
make -j2
```
