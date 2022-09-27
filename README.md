# Universal Help Solutions Problems Issues
General Chetsheet for various problems

## LibreOffice 7.2, 7.4 ...

* Very slow operation, unresponsive, almost impossible to work with etc. 27.9.2022

Clear the cache directory. (I use one in a RAM disk.)
Tools, Paths, Temporary files ...

На български: Инструменти - Настройки - Пътища: Временни файлове ...

## WSL2 GUI operations, Windows 10, Linux

https://www.google.com/search?client=opera&q=WSL+2+connect+to+Xserver&sourceid=opera&ie=UTF-8&oe=UTF-8

etc.

Install X-Window server on Windows:

__Vc-Xsrv__

Start WSL from Windows.
...

Disable ...

Linux: 

DISPLAY=$(cat /etc/resolv.conf | grep nameserver | awk '{print $2}'):0 terminator &
export LIBGL_ALWAYS_INDIRECT=1
export DISPLAY=$(awk '/nameserver / {print $2; exit}' /etc/resolv.conf 2>/dev/null):0
sudo apt install x11-apps
xcalc

//Run again later and check

Closing WSL, on Win console:

wsl --shutdown







