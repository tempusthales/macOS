# Install Brew.sh for macOS Sonoma 14.0 RC

## Download Command Line Tools for Xcode Beta from:
[https://download.developer.apple.com/Developer_Tools/Command_Line_Tools_for_Xcode_15_Release_Candidate/Command_Line_Tools_for_Xcode_15_Release_Candidate.dmg](https://download.developer.apple.com/Developer_Tools/Command_Line_Tools_for_Xcode_15_Release_Candidate/Command_Line_Tools_for_Xcode_15_Release_Candidate.dmg)

## Install Brew.sh on macOS Sonoma

There are two ways to install Brew; via Command Line or via macOS Pkg:

* Command Line: We first need to open Terminal. You can open Terminal by searching for it in Spotlight Search or by navigating to the Applications>Utilities folder. Once Terminal is open, you can use the following command to install Brew:

`/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`

OR

* The macOS .pkg installer also installs Homebrew to its default prefix (`/opt/homebrew` for Apple Silicon and `/usr/local` for macOS Intel) for the same reasons as above. It’s available on **[Homebrew/brew’s latest GitHub release](https://github.com/Homebrew/brew/releases/download/4.1.11/Homebrew-4.1.11.pkg)**

After the installation of Brew is complete, you will receive a "Installation Successful" message, indicating that the Brew installation process has finished. To check the version of Brew, you can try using the command "brew -v" in Terminal. If you encounter an error such as "zsh: command not found: brew," the next step will help you resolve this issue.

## Modify the Brew PATH

In certain versions, Brew is installed in the directory `/usr/local/bin` for Intel-based Macs, while on M1/M2 Macs, Brew is installed in the directory `/opt/homebrew/bin`. This difference can lead to an error message stating "zsh: command not found: brew" when using the Brew command. To resolve this issue, we need to adjust the PATH of the Brew installation directory to the appropriate value. You can utilize the following commands in Terminal to modify the Brew PATH:

```
cd ~/
touch .zprofile
echo 'eval "$(/opt/homebrew/bin/brew shellenv)"' >> $HOME/.zprofile
eval "$(/opt/homebrew/bin/brew shellenv)"
```

## TL;DR

By executing these commands, the PATH configuration will be updated, ensuring that Brew is accessible from the correct location.

After installing Brew, you can easily install any application or package using the following commands:

```
brew install package_name
brew uninstall package_name
brew list
```

If you encounter any problems with Brew on macOS Sonoma, you can use the following command to uninstall Brew:

`/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/uninstall.sh)"`

Currently, there is no official version of Brew that specifically supports macOS Sonoma. However, you can still install older versions of Brew on macOS Sonoma, and we have successfully tested the installation of various applications and packages using Brew on macOS Sonoma.
