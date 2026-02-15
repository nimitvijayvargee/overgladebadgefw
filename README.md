# Overglade Badge Firmware
This is a slightly modified version of the original firmware on the Overglade Badges. 

Hardware Resources ([@KaiPereira](https://github.com/KaiPereira/)) : [Overglade-Badges](https://github.com/KaiPereira/Overglade-Badges/tree/master)

The E-Ink Display Driver is a modified version of [Waveshare's driver for micropython](https://github.com/waveshareteam/Pico_ePaper_Code/blob/main/python/Pico_ePaper-2.66.py), and heavily based on the works by [@mpkendall](https://github.com/mpkendall/) (and the badges for Undercity and Prototype).

> Note that while NFC is available as part of the hardware, it is independant of the software. The NFC chip is connected to the microcontroller via IIC, and can definitely be interfaced with the software. However, it is currently suggested to flash NFC via the app for [Attend](https://attend.hackclub.com/) (This is limited to people with access to participant information for privacy reasons). If your badge is flashed via attend, then you may modify the URL on it by visiting the badge URL tool [(badge.hackclub.com)](https://badge.hackclub.com/).

> :warning: A placeholder image.png is necessary for the badge to render properly. This can be ignored if a valid image is already put onto the badge via the badge flashing tool. The image requirements are the same.

Flashing can be done via `mpremote` to connect to and manipulate the filesystem. Alternatively, you can just upload the files within Thonny. The minimum required files are: `main.py`, `einkdriver.py`, `image.bmp`, `config.json` and `overglade.bmp`. Any other files will be ignored.