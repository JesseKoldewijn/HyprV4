<h1 align="center">Welcome to alacritty-DotFiles 👋</h1>

> Alacritty config used on my personal systems. Feel free to fork and/or clone.

# Notes

-   There is a starship prompt config included under the "plugins" directory.

-   Clink injection flow for windows is added as well as a windows commands work-around (more Unix/Linux like commands flow)

# Install

## Windows

1. ### Install winget

-   [Download winget](https://www.microsoft.com/p/app-installer/9nblggh4nns1)

2. ### Install chololatey

-   To install chocolatey, open a admin powershell session and type in the following command: \
    `Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))`

3. ### Install alacritty

-   `winget install Alacritty.Alacritty`

3. ### Install clink

-   `winget install chrisant996.Clink`

4. ### Autorun clink

-   USER - Default: `clink autorun install`
-   SYSTEM (admin-cmd required) - Default: \
    `clink autorun install -a`
-   USER - No welcome message: `clink autorun install -- -q`
-   SYSTEM (admin-cmd required) - No welcome message: \
    `clink autorun install -a -- -q`

5. ### Inject starship

-   Move copy-paste the starship.lua file from the plugin/win/clink dir to: \ `%LOCALAPPDATA%/clink`

6. ### Configure starship

-   Install `vi` to allow easily editing the starship config.
-   Run `starship config` in a terminal/alacritty window.
-   Paste the config from plugins/starship.toml or any other starship config you want to use into the `vi` editor session it opened.

## Linux

TBD

## Author

👤 **Jesse Koldewijn**

-   Website: https://jkinsight.nl
-   Github: [@JesseKoldewijn](https://github.com/JesseKoldewijn)

## Show your support

Give a ⭐️ if this project helped you!
