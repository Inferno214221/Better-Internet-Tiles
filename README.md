# Better Internet Tiles Libre

This is a fork of the original Better Inter Tiles by @casperverswijvelt to remove every non-libre component and analytics

<img alt="GitHub" src="https://img.shields.io/github/license/D3SOX/Better-Internet-Tiles-Libre"> <img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/D3SOX/Better-Internet-Tiles-Libre"> <img alt="GitHub release (latest by date)" src="https://img.shields.io/github/v/release/D3SOX/Better-Internet-Tiles-Libre">
</a>

<a href="https://github.com/D3SOX/Better-Internet-Tiles-Libre/releases"><img alt="Get it on GitHub" src="https://github.com/D3SOX/Better-Internet-Tiles-Libre/assets/24937357/c3c0042b-e4c2-465f-8f1b-f0b7a943fb67" height=60px /></a>

You can use something like Obtainium to get updates

## About

This application aims to create a unified internet quick-settings tile, which is actually useful (I'm looking at you, Android 12). Next to this, **separate Wi-Fi and mobile data tiles are also available** if you just want to go back to the behaviour of Android 11 or lower.

Tapping the new unified internet tile will simply toggle between Wi-Fi and mobile data, which is exactly what I want it to do most of the time. This reduces the amount of taps needed from 3 (tap tile, disable wifi, enable data) to just 1 quick tap. In situations where you still want more control, long pressing the tile will redirect you to the relevant settings page.

**This has been tested and confirmed working on Pixel devices running Android 12, 13 and 14, but other devices will probably work too.**

## Shell access required
Shell access is required to enable/disable Wi-Fi and mobile data, as well as for reading the SSID of the current Wi-Fi network. This can be granted using regular root, or by using the Shizuku application. Shizuku can be started using either adb or wireless debugging (or root, but then you might as wel use direct root access instead). The Sui and Riru magisk modules can also be used as an alternative to the Shizuku application.

**Beware that if you do use Shizuku without root, you will need to start the Shizuku server each time you reboot the device.** You can do this without a PC using the wireless debugging method, so it is not that big of an issue, but it is something to keep in mind.

## Features
- An improved unified Internet tile where you can tap to toggle between Wi-Fi and mobile data (visually very similar to the stock Android 12 tile, but more functional)
- Separate Wi-Fi and mobile data tiles if you just want to go back to behaviour before Android 12
- NFC tile which was apparently also removed 🤷
- Ability to configure access to the tiles while the phone is locked

## How to install
- Download and install the app using the 'app-release.apk' file from the the [latest release in the GitHub repository](https://github.com/D3SOX/Better-Internet-Tiles-Libre/releases).
- Open the app, and click on the 'Request Shizuku access' or 'Request root access' button, depending on which method of Shell access you prefer.
- Only if you are using Shizuku:
  - You must start the Shizuku server each time the device is booted. Follow the instructions in the Shizuku application.
  - There is a persistent notification to allow a foreground service to start, so Shizuku can detect the process without having to manually open the 'Better Internet Tiles' application. You can just hide this notification without any issue.
- Edit your quicksettings layout, drag your desired tile to the top and remove the original internet tile.
If you are on Android 13 or higher, you can also add them using the shortcut buttons within the app.
- Enjoy easier switching between mobile data and WiFi with just a single tap!

## Contribute
Feel free to check out the source code and create an issue or pull request if you want to see more features added.
Less tech savvy but also want to contribute? Check out this project on [Weblate](https://hosted.weblate.org/guide/better-internet-tiles/translations/) to help out with translations!
