# linux4.4-pl2303hxn
Modified pl2303 driver based on Linux 4.4 generic, which supports pl2303hxn added in 2020 kernel update. For example this driver works in ubuntu 16


## Compiling and launching

This is a generic kernel module. As such, if confused, there are loads of resources online on how to use this

- installing deps:

sudo apt update
sudo apt-get install linux-headers-$(uname -r)
sudo apt-get install linux-source-4.4.0

- compiling

make # in the cloned repo

- running

sudo modprobe usbserial 
sudo rmmod pl2303
sudo insmod pl2303.ko # compiled .ko file
