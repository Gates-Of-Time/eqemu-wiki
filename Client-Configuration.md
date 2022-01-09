EQEmulator is a custom, completely from-scratch, open source server implementation for EverQuest, built mostly on C++.  EQEmulator is an open-source project, released under the GNU General Public License.

**EverQuest clients are the intellectual property of the Daybreak Game Company, LLC.**  Copies of Daybreak Game Company intellectual property are not sourced through the EQEmulator project, nor should you provide unlicensed copies through any EQEmulator asset.

This page is intended to assist you in configuring your client to connect to an EQEmu server.  

- [**All Operating Systems**](#all-operating-systems)
- [**Windows**](#windows)
- [**macOS Mojave**](#macos-mojave)
- [**macOS High Sierra**](#macos-high-sierra)
- [**Linux**](#linux)
- [**Troubleshooting**](#troubleshooting)

# All Operating Systems

* Navigate to your EverQuest directory and modify the eqhost file:

**Titanium** or **Secrets of Faydwer** Clients:

```
[LoginServer]
Host=login.eqemulator.net:5998
```

**Seeds of Destruction**, **Underfoot**, or **Rain of Fear** Clients:

```
[LoginServer]
Host=login.eqemulator.net:5999
```


# Windows



# macOS Mojave

The EverQuest client can be run through Wine on Mojave.  To configure your system, follow these steps:

1. Install Xcode:

	* Click the Apple Icon in the upper-left corner of your screen⋅⋅
	* Choose App Store...
	* Search for Xcode
	* Install Xcode

2. Install Command Line Tools:

	* Open Terminal (_/Applications/Utilities/Terminal.app_)
	* Copy and paste this command and execute:

```shell
xcode-select --install
```

3. Install Homebrew:

	* Open Terminal (_/Applications/Utilities/Terminal.app_)
	* Copy and paste this command and execute:

```shell
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

4. Create a symbolic link between X11 folders:

	* Open Terminal (_/Applications/Utilities/Terminal.app_)
	* Copy and paste this command and execute:

```shell
sudo ln -s /opt/X11 /usr/X11
```

5. Install XQuartz:

	* Open Terminal (_/Applications/Utilities/Terminal.app_)
	* Copy and paste this command and execute:

```shell
brew install Caskroom/cask/xquartz
```

6. Create a symbolic link between library folders:

	* Open Terminal (_/Applications/Utilities/Terminal.app_)
	* Copy and paste this command and execute:

```shell
sudo ln -s /usr/local/lib /usr/X11/lib/*
```

7. Install Wine

	* Open Terminal (_/Applications/Utilities/Terminal.app_)
	* Copy and paste this command and execute:

```shell
brew install wine
```

8. Install Winetricks

	* Open Terminal (_/Applications/Utilities/Terminal.app_)
	* Copy and paste this command and execute:

```shell
brew install winetricks
```

9. Configure Wine fonts

	* Open Terminal (_/Applications/Utilities/Terminal.app_)
	* Copy and paste this command and execute:

```shell
winetricks corefonts
```

10. Configure Font Smoothing

	* Open Terminal (_/Applications/Utilities/Terminal.app_)
	* Copy and paste this command and execute:

```shell
cat << EOF > /tmp/fontsmoothing
REGEDIT4

[HKEY_CURRENT_USER\Control Panel\Desktop]
"FontSmoothing"="2"
"FontSmoothingOrientation"=dword:00000001
"FontSmoothingType"=dword:00000002
"FontSmoothingGamma"=dword:00000578
EOF

WINE=${WINE:-wine} WINEPREFIX=${WINEPREFIX:-$HOME/.wine} $WINE regedit /tmp/fontsmoothing 2> /dev/null
```

11. Launch EverQuest

	* Open Terminal (_/Applications/Utilities/Terminal.app_)
	* Navigate to your EverQuest directory (IE _cd Applications/EverQuest/_)
	* Launch with the "patchme" option:

```shell
wine eqgame.exe patchme
```

12. Optional Launcher Script/Icon

	* Open TextEdit (_/Applications/TextEdit.app_)
	* Copy and paste the information below
	* Replace $WINEPREFIX with the location of your Prefix
	* Replace the path to your EverQuest folder
	* Save the file as "EverQuest.command"

```shell
#!/bin/bash
export WINEPREFIX="$WINEPREFIX/.wine"
export DYLD_FALLBACK_LIBRARY_PATH=/usr/X11/lib
export FREETYPE_PROPERTIES="truetype:interpreter-version=35"
cd "/path/to/my/everquest/folder/"
wine eqgame.exe patchme
```

# macOS High Sierra



# Linux


# Troubleshooting

1. Excessive GPU usage with MacOS Mojave

	* Open Terminal (_/Applications/Utilities/Terminal.app_)
	* Enter the command "wine regedit"
	* HKEY_CURRENT_USER -> Software -> Wine -> Direct3D
	* Create a DWORD Value (REG_DWORD) named "[csmt](https://wiki.archlinux.org/index.php/wine#CSMT)" and set the value to 0x0 (disable)