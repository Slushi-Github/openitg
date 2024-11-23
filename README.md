# HEY
This is just me trying to modify OpenITG for some ridiculous purpose, nothing special, don't try to make use of it XD

## Build OpenITG on Ubuntu x64:
```shell
# Install required dependencies
sudo apt install git build-essential autoconf automake \
libgl1-mesa-dev libglu1-mesa-dev libpng-dev \
libjpeg62-dev liblua5.1-0-dev libvorbis-dev libmad0-dev \
libusb-dev libxrandr-dev libavcodec-dev libswscale-dev \
libavformat-dev libasound2-dev libavutil-dev

# Clone the software
git clone https://github.com/Slushi-Github/openitg.git

# Change to the OpenITG directory
cd openitg

# Slushi fixes for compilation (I must always have trouble compiling this kind of stupid stuff XD)
# Solution from this: https://askubuntu.com/questions/178364/i-am-trying-to-build-libmtp-1-1-14-but-i-cannot-fix-this-error
sudo apt install gettext
./autogen.sh
./configure

# Build OpenITG
./build-home.sh
```