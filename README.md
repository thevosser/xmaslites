# xmaslites

Christmas lights project to keep me coding in a time where I'm not doing it professionally



### Materials
- Raspberry Pi ZeroWH (link)
- WS2812B 300 RGB LED strip (link)
- AC/DC Power Supply 5V 15A
  - Not enough to light strip to full brightness
- Lead wires

### Concepts
- Linux to Windows Samba Share
- Python
- Python VENV
- Flask
- BASH
- NGINX
- Docker
  - Maybe, GPIO can be exposed, safer than running sudo for python script
- memcache (maybe, better than using a file)

### Steps
- Setup Raspbian Minimal to SD Card
  - setup ssh and wifi on card before boot for headless
- power on Pi and ssh into it
- hostname setup (or do we do this on the SD card?)
  - recommend new windows terminal or using Ubuntu WSL (really both is best)
- apt update
- install python
- installl pip
- install flask, venv, dotenv, neopixel, board-gpio, samba
- setup samba share
- write code on windows for neopixels
- test on PI
- setup flask in folder
- write flask code on Windows
- setup simple website on Windows
- setup select file for flask and led code to talk to each other
- clean up and refactor code for efficiency
- setup files to run on their on at startup
- setup nginx for flask site
- setup memcache and replace file
- install docker
- setup dockerfiles for both scripts
- setup nginx to run host docker flask


### References
- Neopixel library reference
- Adafruit neopixel tutorial
- Flask guide (Miguel's)
- 
