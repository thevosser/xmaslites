# xmaslites

Christmas lights project to keep me coding in a time where I'm not doing it professionally.  Using a Raspberry Pi Zero WH to host a Python Flask/NGINX simple webpage that changes values monitored by another Python script using Adafruit's Neopixel library to control a WS2812B 300 RGB LED strip.  Nothing complex, just something to keep programming.  I'll note, I started with Arduino, but moved to Raspberry Pi so I could easily have a web interface.  

### Materials
- Raspberry Pi ZeroWH (link)
- WS2812B 300 RGB LED strip (*[link](https://www.amazon.com/BTF-LIGHTING-Flexible-Individually-Addressable-Non-waterproof/dp/B01CDTELBE/ref=asc_df_B01CDTEJBG/?tag=hyprod-20&linkCode=df0&hvadid=242074984067&hvpos=&hvnetw=g&hvrand=14147673531154704499&hvpone=&hvptwo=&hvqmt=&hvdev=c&hvdvcmdl=&hvlocint=&hvlocphy=9018109&hvtargid=pla-372649960034&th=1)*)
- AC/DC Power Supply 5V 15A (*[link](https://www.amazon.com/ALITOVE-Transformer-Converter-5-5x2-1mm-100V-240V/dp/B01LXN7MN3/ref=sr_1_3?crid=UFBKFLI4N6O7&keywords=5v%2B15a%2Bpower%2Bsupply&qid=1637358542&sprefix=5v%2B15a%2B%2Caps%2C176&sr=8-3&th=1)*)
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
- Setup ajax on the website to modify light values
- setup select file for flask and led code to talk to each other
- clean up and refactor code for efficiency
- setup files to run on their on at startup
- setup nginx for flask site
- setup memcache and replace file
- install docker
- setup dockerfiles for both scripts
- setup nginx to run host docker flask


### References
- Neopixel library reference (*[link]()*)
- Adafruit neopixel tutorial (*[link]()*)
- Flask guide (Miguel's) (*[link](https://blog.miguelgrinberg.com/post/the-flask-mega-tutorial-part-i-hello-world)*)
- Flask NGINX Guide (*[link](https://flask.palletsprojects.com/en/2.0.x/deploying/uwsgi/)*)
- NGINX Flask Guide (*[link](https://unit.nginx.org/howto/flask/)*)
- Ubuntu Samba Share
- Raspberry Pi SSH/Wifi config
- Neopixel power guide (where did I read how much current was required?)
- Ajax guide
-  (*[link]()*)
