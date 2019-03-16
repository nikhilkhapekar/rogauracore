# rogauracore - RGB keyboard control for Asus ROG laptops

(c) 2019 Will Roberts

Linux-compatible Open-source libusb implementation similar to the Asus
Aura Core software.  Supports RGB keyboards with IDs
[0b05:1854](https://linux-hardware.org/index.php?id=usb:0b05-1854)
(GL553 and GL753) and
[0b05:1869](https://linux-hardware.org/index.php?id=usb:0b05-1869)
(GL503, FX503, GL703).

## Usage

```
Usage:
   rogauracore COMMAND ARGUMENTS

COMMAND should be one of:
   single_static
   single_breathing
   single_colorcycle
   multi_static
   multi_breathing
   red
   green
   blue
   yellow
   cyan
   magenta
   white
   black
   rainbow
```

## Building

### On Ubuntu from a release:

```
sudo apt install libusb-1.0-0 libusb-1.0-0-dev
tar xf rogauracore-1.0.tar.gz
cd rogauracore-1.0/
./configure
make
sudo make install
```

### From github:

Clone the github repo and enter the top-level directory.  Then:

```sh
autoreconf
./configure
make
```
