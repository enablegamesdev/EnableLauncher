# EnableLauncher

Created by [enAbleGames](https://www.enablegames.com/)

### Table of Contents
- [Introduction](#introduction)
- [Installation](#installation)
- [Installing and Playing Games](#games)
- [Body Tracking](#bodyTracking)
- [Game Filters](#gameFilters)
- [Resources/Log Out](#resources)

/## <a id="introduction"></a>Introduction

The EnableLauncher is an app from which you can download and play all games in the enAbleGames catalog.
It handles game controls by tracking your body motions from using Kinect, Orbbec Astra, webcam, color tracking, or from connecting to the EnableServer App.

To use the app, you will need an enAbleGames account. If you do not already have an account, you can set one up with the following link:
[Account-Creation](https://github.com/enablegamesdev/EnableLauncher/wiki/Account-Creation)



## <a id="installation"></a>Installation

You can download the installer from the [release page](https://github.com/enablegamesdev/EnableLauncher/releases).

After installing the Launcher, log in using your enAbleGames account.  It may take a few minutes to check for updates.  When the Launcher asks if you would like to download updates, select "Yes".  The Launcher will open the Patcher application in a new window.

After the Patcher is finished, the Launcher will re-open.  Log in again when you see the login screen, and you will see the Library page.



## <a id="games"></a> Installing and Playing Games

Select the game you want to download from the left side of the screen.  Click the orange "Update Game" button in the top-left corner of the screen.  It will launch the Patcher in another window.

![image](https://github.com/user-attachments/assets/68f12353-d1b2-48ec-9068-505cdc536059)

When the Patcher finishes installing your game, refresh the Launcher using the blue "Refresh" button at the top of the screen, and press the "Play" button in the top-left corner to play your game.

There are also buttons for "Update All" and "Reinstall All", as well as the "Reinstall Game" button.  The buttons for "all" will cue updates for all games in the patcher, the "Reinstall" buttons will delete either all games or the currently selected game, respectively. 

Information about the currently selected game can be viewed on the enAbleGames website via the first tab, wich will display the name of that game.



## <a id="bodyTracking"></a>Body Tracking

### There are 4 types of controls in the EnableLauncher:
- Kinect/Astra
- Webcam Tracking
- The enableServer App
- Color Tracking

![LauncherControls](https://github.com/user-attachments/assets/e8fbf618-6a03-460e-a083-24859791cea6)



**Kinect/Astra**

To use the Kinect or Astra, you will need to install the appropriate drivers to your computer.  They can be found on the website via this link, along with instructions on how to set them up: [enAbleGames website](https://www.enablegames.com/manuals/startup-guide/)

Once you've installed the necessary drivers, plug in your Kinect or Astra, launch the EnableLauncher, and log in to your account. The Kinect or Astra will connect automatically once you load the library screen. If the Kinect is activated, its box in the Body Tracking panel will light up orange instead of blue.

Within the Body Tracking tab, there are three options for Kinect/Astra controls:
-Smooth Controls will create in-between frames between your body poses.  This can make the player's inputs smoother.
-Skip Frames allows you to skip every few frames, according to your setting.  This can speed up the rate of processing.
-Switch Player can be used if the Kinect/Astra is picking up another body on the camera.

The Kinect/Astra control mode offers some of the most accurate body controls, though it requires additional hardware to use and may be more taxing on your computer.



**Webcam Tracking**

Webcam Tracking can be activated by pressing the “Start Webcam Tracking” button on the Body Tracking page of the EnableLauncher.  Make sure your webcam is active before using this mode.

By checking the “Only Move Upper Body” option, you can reduce latency in body tracking, though you will not be able to use your legs.

There are different modes that also limit the data tracked, such as "full" for full body controls, "pose_and_hand" to control both body and hnad motions, etc. These can be switched between for more accurate data or better performance.

If you plug your camera in to your computer after the library screen has been loaded, press the "Refresh" button at the top of the screen to load it into the cameras menu of the "Holistic Webcam Controls" panel.

This method of control can be used on any piece of hardware with a camera, though it also requires a GPU card.  It may slow performance depending on the capabilities of the user’s device.



**enableServer App**

The enableServer App is the standalone software that can handle motion capture using any camera on your PC, Mac, or mobile devices, including webcams. The Supported Platforms are:

- iOS
- PC
- macOS

If you have the enableServer app installed on a secondary device, you can remotely control the EnableLauncher on your computer.  You will need to connect your secondary device to the same wifi as the device running the EnableLauncher.
This method requires a second device, but it may reduce latency in games since the body pose processing is not being handled by your computer.

**_Connect to the EnableLauncher from the app_**

Ensure your devices running the enableServer and tbe EnableLauncher/games are on the same network or device.

In the initial menu, select your control mode.  For best performance on an iOS device, select "OSC".  Note that this control mode can only use your device's back cameras.
the Holistic version has more flexibility in tracking mode, including hand tracking and face tracking, and can use both back and front cameras but have longer latency.  However, it may have less accurate data since it is only using a single camera to calculate body data.  Below, we will demonstrate connecting to the app using the OSC mode.
_UNet is Deprecated. Do not use it unless asked to. OSC is the standard ARKit version, and Holistic is the Holistic version._

![IMG_0006](https://github.com/user-attachments/assets/bc71037f-a74b-42df-8f85-17fde6f75ab1)
Once you are in the camera scene, press the button on the bottom left of enableServer.  From here, you can manually scan the QR code from the EnableLauncher in the app by clicking the square button in the bottom right, or you can manually input the IP address by tapping the "+" button and typing the IP address of your computer in the field above the "Launcher/Game" toggle.

The enableServer app can also communicate directly with games if the EnableLauncher is not running.  The connection QR code or IP address can be found through a game’s pause menu.  Make sure to set the "Launcher/Game" toggle to the appropriate setting when you are trying to connect directly to a game.

If you are successfully connected, a widget will appear showing the IP address you are connected to, and the User Name of your Enable Games account if you connect automatically with the launcher. Click on the widget to start sending the tracking data.  It will change from red to green if it is sending.

You can connect to multiple devices running the launcher and game simultaneously, but you can only connect to one game on one PC.

**_Connect to the app from the EnableLauncher_**

If you are trying to connect your secondary device to the EnableLauncher and your network supports UDP Broadcasting, you can type your secondary device’s IP address in the field under the “Receive Remote” button, then click the “Receive Remote” button.

**_Using Holistic Motion Tracking_**

![IMG-0528](https://github.com/user-attachments/assets/1c10a2cd-b325-4e73-985e-b5edda338b21)

To use Holistic Motion Tracking, you must choose the camera you are using and then press the Start/Stop button. There are five modes you can choose from:
- full: Tracking pose, hand, and face
- pose and face
- pose and hand: choose this if you want to track the rotation of the wrists
- pose only
- face only
- We recommend you only track the elements you use to decrease the latency.

Face tracking is currently not supported on iOS.

**_Known Issues_**

-On iOS, if you put your device to sleep when using eAgServer, you need to restart the app to resume the tracking.
-Check your firewall settings if you have problem on connecting.



**Color Tracking**

Color Tracking can be accessed from the Options menu under the “Controls” section.  Make sure your webcam is active before using this mode.  The body will track two colors from your webcam, which you choose by clicking the left and right mouse buttons on the screen.

This method is the least intensive of any control style, though it is highly limited in the types of motions the player can make.  It is not able to calculate accurate elbow motions or lower-body motions since it only calculates hand positions.



## <a id="introduction"></a>Introduction

![Filters Menu](https://github.com/user-attachments/assets/299719d1-de26-4efc-a9c8-d91166bc3879)

In the filters menu, you can search for games by type.  Check the box on the left side of the column to search by that category.  Change the values of that category on the right side.



****
