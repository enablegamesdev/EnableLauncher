# EnableLauncher

Created by [enAbleGames](https://www.enablegames.com/)

### Table of Contents
- [Introduction](#introduction)
- [Installation](#installation)
- [Installing and Playing Games](#games)
- [Body Tracking](#bodyTracking)

## <a id="introduction"></a>Introduction
The EnableLauncher is an app in which you can download and play all games in the enAbleGames catalog using your enAbleGames account.
It handles game controls by tracking your body motions from using Kinect, Orbbec Astra, webcam, color tracking, or from connecting to the EnableServer App.

If you do not already have an account, you can set one up with the following link:
[here](https://github.com/enablegamesdev/EnableLauncher/wiki/Account-Creation)

## <a id="installation"></a>Installation
You can download the installer from the [release page](https://github.com/enablegamesdev/EnableLauncher/releases).

After installing the Launcher, log in using your enAbleGames account.  It may take a few minutes to check for updates.  When the Launcher asks if you would like to download updates, select "Yes".  The Launcher will open the Patcher application in a new window.

After the Patcher is finished, the Launcher will re-open.  Log in again when you see the login screen, and you will see the Library page.

## <a id="games"></a> Installing and Playing Games

Select the game you want to download from the left side of the screen.  Click the "Update Game" button in the top-left corner of the screen.  It will launch the Patcher in another window.

![image](https://github.com/user-attachments/assets/68f12353-d1b2-48ec-9068-505cdc536059)

When the Patcher finishes installing your game, refresh the Launcher and press the Play button in the top-left corner to play your game.

## <a id="bodyTracking"></a>Body Tracking

### There are 4 types of controls in the EnableLauncher
- [Kinect/Astra](#kinect)
- [Webcam Tracking](#webcam)
- [The enableServer APP](#enableserver)
- [Color Tracking](#color)

![LauncherControls](https://github.com/user-attachments/assets/e8fbf618-6a03-460e-a083-24859791cea6)

## <a id = "kinect"></a> Kinect/Astra

To use the Kinect or Astra, you will need to install the appropriate drivers to your computer.  They can be found on the website via this link, along with instructions on how to set them up: [enAbleGames website](https://www.enablegames.com/manuals/startup-guide/)

Once you've installed the necessary drivers, plug in your Kinect or Astra, launch the EnableLauncher, and log in to your account. The Kinect or Astra will connect automatically once you load the library screen. If the Kinect is activated, its box in the Body Tracking panel will light up orange instead of blue.

Within the Body Tracking tab, there are three options for Kinect/Astra controls:
-Smooth Controls will create in-between frames between your body poses.  This can make the player's inputs smoother.
-Skip Frames allows you to skip every few frames, according to your setting.  This can speed up the rate of processing.
-Switch Player can be used if the Kinect/Astra is picking up another body on the camera.

The Kinect/Astra control mode offers some of the most accurate body controls, though it requires additional hardware to use and may be more taxing on your computer.


## <a id = "webcam"></a> Webcam Tracking
Webcam Tracking can be activated by pressing the “Start Webcam Tracking” button on the Body Tracking page of the EnableLauncher.  Make sure your webcam is active before using this mode.

By checking the “Only Move Upper Body” option, you can reduce latency in body tracking, though you will not be able to use your legs.

If you plug your camera in to your computer after the library screen has been loaded, press the "Refresh" button at the top of the screen to load it into the cameras menu of the "Holistic Webcam Controls" panel.

This method of control can be used on any piece of hardware with a camera, though it also requires a GPU card.  It may slow performance depending on the capabilities of the user’s device.


## <a id = "enableserver"></a> enableServer App
You can set up the app using the enableServer Manual via this link: [enableServer Manual](https://ambitious-dune-026773e10.5.azurestaticapps.net/e-ag-server-manual/)
This method requires a second device, but it may reduce latency in games since the body pose processing is not being handled by your computer.

If you have the enableServer app installed on a secondary device, you can control the EnableLauncher remotely.  You will need to connect your secondary device to the same wifi as the device running the EnableLauncher.

Connect to the EnableLauncher from the app
Using the button on the bottom left of enableServer, add the device and input the IP Address from the EnableLauncher, which can be found on the right side of the Options tab.  You can also manually scan the QR code from the EnableLauncher in the app.

The enableServer app can also communicate directly with games if the EnableLauncher is not running.  The connection QR code or IP address can be found through a game’s pause menu.


Connect to the app from the EnableLauncher
In the Options screen of the EnableLauncher, type your phone’s IP address in the field under “Receive Remote” button, then click the “Receive Remote” button. 





## <a id = "color"></a> Color Tracking
Color Tracking can be accessed from the Options menu under the “Controls” section.  Make sure your webcam is active before using this mode.  The body will track two colors from your webcam, which you choose by clicking the left and right mouse buttons on the screen.

This method is the least intensive of any control style, though it is highly limited in the types of motions the player can make.  It is not able to calculate accurate elbow motions or lower-body motions since it only calculates hand positions.

