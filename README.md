# SETS - STO Equipment and Trait Selector
A Star Trek Online build tool in Python. Please refer to the [website](https://stobuilds.com/apps/sets) for information on how this app is used and included features.

## Description
Build management and sharing tool for STO.
Builds can be exported to a PNG or JSON file that can be opened by another person using SETS.

## Installation
### Images library
All installation methods require an images library containing the game icons. The app will download these automatically, but as this takes a very long time, it is recommended to download the newest compressed image library from the [release](https://github.com/STOCD/SETS/releases) page. Once downloaded this has to be decompressed and placed in into the `.config/images` folder.
```
SETS
 +- .config
 |  `- images
 |    `- <lots of images>
 +- SETS.exe / main.py
 +- ...
```

### Executable for Windows
Download the zipped app from the [release](https://github.com/STOCD/SETS/releases) page. Unzip it into a folder where you want your app to live. To speed up the image downloading process, obtain the images library as detailed above. Double-clicking `SETS.exe` will start the app.

You can create a desktop shortcut by rightclicking on `SETS.exe` and clicking on "Create shortcut" in the context menu. Then move the created shortcut to your desktop. To create a start menu entry, open the start menu folder by rightclicking on an arbitrary app in your start menu and clicking on "Open file location". Then move the created shortcut to the folder that opened.


### Script (Cross-Platform)
*The commands below are for Windows. If you want to install the app on Linux, use `python3` instead of `python`. A more comprehensive guide for installing the script version can be found on the [website](https://stobuilds.com/apps/sets/installation).*

First, create a folder to house your app. Open a command prompt and navigate *inside* the created folder.

Download the source code. This can be done using `git` or manual download:
- Manual Download: On the GitHub page of [this repository](https://github.com/STOCD/SETS), click on the green `CODE` button and select "Download ZIP". Save the archive and unpack it so that the files and folders seen on the repository page are *directly* inside your app folder.
- Git: run `git clone https://github.com/STOCD/SETS.git .`

Install dependencies by running `python -m pip install .`.

To speed up the image download process on first start of the app, download the latest image archive from [releases](https://github.com/STOCD/SETS/releases). Create a `.config` folder and unpack the images archive into it. The images should be in `<app_root>\.config\images\`.

*Ubuntu* users might need to install the `libxcb-cursor0` package for this app to work: `sudo apt install libxcb-cursor0`

To run the app, navigate to your apps folder. Then:
- Windows: Use `python main.py` to start the app.
- Linux: Use `python3 main.py` to start the app.

## Contributing
If you find any information or images missing, please check or update the [official wiki](https://stowiki.net) -- where SETS gets this information. You can report wiki issues on the [Star Trek Online Community Discord Server](https://discord.gg/eApUvTRr5q) in the "#wiki-discussion" channel or on the [STOBuilds Discord Server](https://discord.gg/kxwHxbsqzF) in the "#wiki-update-talk" channel.

For application-related issues or suggestions, please visit the [STOBuilds Discord](https://discord.gg/kxwHxbsqzF) ("#sets-support" channel).
