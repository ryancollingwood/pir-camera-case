# The Pi Hut Raspberry Pi PIR Camera Case - setup and code examples

The PIR Camera Case ([Pi 4](https://thepihut.com) / [Pi Zero (Coming soon](https://thepihut.com)) is a case designed to hold your Raspberry Pi, an [Official Raspberry Pi Camera Module](https://thepihut.com/products/raspberry-pi-camera-module) and the included PIR sensor.

When used together, you have a great foundation for an indoors Raspberry Pi motion-sensing camera project. Combine with [MotionEyeOS](https://github.com/ccrisan/motioneyeos/wiki) for a superb Raspberry Pi IP surveillance system!

![PIR Camera Case](/images/PIR-Camera-Case-2.jpg)

This repository will show you how to [prepare your Raspberry Pi](https://github.com/ThePiHut/Raspberry-Pi-PIR-Camera-Case#prepare-your-raspberry-pi) and give you some [example code](https://github.com/ThePiHut/Raspberry-Pi-PIR-Camera-Case#example-code) to get you started.
## Prepare your Raspberry Pi

**Operating System**

We recommend the [Raspberry Pi OS](https://www.raspberrypi.org/downloads/) for this project/case, and this guide assumes you have the basic operating system loaded and ready.
You can also use other systems such as [MotionEyeOS](https://github.com/ccrisan/motioneyeos/wiki) for a live video surveillance style system.

**Case Asembly**

You will need to have [assembled the case](#) which includes connecting the Camera Module and PIR sensor.

**Enable the Camera Interface**

We need to make sure your Raspberry Pi is configured to use the Camera Module to enable it to take photos when instructed by our code.

We will enable the camera interface by opening a new terminal window and entering:
```bash
sudo raspi-config
```
This will show a screen similar to this:

![Raspi-Config](images/raspi-config-screen.jpg)

Now simply select 'Interfacing Options', 'Camera' then 'Yes' to enable the camera interface. Reboot your Raspberry Pi when prompted.

**Test the Camera**

Run a quick test before proceeding. With your Raspberry Pi connected to a monitor via a HDMI cable, in a terminal window enter the following command to take a quick basic picture with the camera:
```bash
raspistill -o test.jpg
```
If you don't see an image on the screen, check the camera connection, re-fit the cable if necessary, reboot and try again.
## Example Code

We have added examples below showing you how to control the individual components, alongside a combined code example showing a full motion-sensing camera project.

**Controlling individual components**
- [Simple PIR code](tutorials/status-zero/README.md)
- [Basic camera module terminal commands](tutorials/status-board/README.md)
- [Using the camera module in a script](tutorials/status-board/README.md)

**Motion sensing project example**
- [PIR + Camera code](tutorials/status-zero/README.md)
