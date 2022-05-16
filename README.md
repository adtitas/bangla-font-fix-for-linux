## Bangla Font Fix for Linux
Fonts from Win10_20H2_English_x64.iso (Extracted)<br>
If you want to install Windows 10 fonts on Linux, visit this [repo](https://github.com/adtitas/win10-fonts-for-linux).

### Introduction
If the Bangla font in your Linux system looks ugly to you (in browser or any app), then you've come to the right place.<br>
All you need to do is run only one command. Have a nice day!

### Installation Guide

> To set bangla font (nirmala  ui) + install windows fonts in linux system<br>

Copy the code and paste it to your terminal:
```console
git clone https://github.com/adtitas/win10-fonts-for-linux.git && sudo mkdir -p /usr/share/fonts/win10-fonts && sudo cp -n -r WindowsFonts/. /usr/share/fonts/win10-fonts/ && sudo chmod 644 /usr/share/fonts/win10-fonts && fc-cache && wget [] && mkdir -p ~/.config/fontconfig/conf.d && cp -n 50-linux-bangla.conf $_
```

> To set bangla font only (nirmala  ui)<br>

Copy the code and paste it to your terminal:
```console
mkdir -p ~/bangla-font-fix && wget -c https://raw.githubusercontent.com/adtitas/win10-fonts-for-linux/main/WindowsFonts/Nirmala.ttf -P ~/bangla-font-fix && wget -c https://raw.githubusercontent.com/adtitas/win10-fonts-for-linux/main/WindowsFonts/NirmalaB.ttf -P ~/bangla-font-fix && wget -c https://raw.githubusercontent.com/adtitas/win10-fonts-for-linux/main/WindowsFonts/NirmalaS.ttf -P ~/bangla-font-fix && sudo mkdir -p /usr/share/fonts/win10-fonts && sudo cp -n -r bangla-font-fix/. /usr/share/fonts/win10-fonts/ && sudo chmod 644 /usr/share/fonts/win10-fonts && fc-cache && wget -c [] -P ~/bangla-font-fix && mkdir -p ~/.config/fontconfig/conf.d && cp -n 50-linux-bangla.conf $_
```
### Notes
* If `git` isn't installed on your system, you may need to install it. Visit [here](https://git-scm.com/download/linux).
* If `wget` isn't installed on your system, you may need to install it. Visit [here](https://www.tecmint.com/install-wget-in-linux)

