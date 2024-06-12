# Portenta X8 Flask Video Streamer

## Dependencies and Steps:

- Install and run Ubuntu 22.04 Docker image:

```
docker run -it --rm --privileged --network=host -v /dev/:/dev/ --env UDEV=1 --device /dev:/dev --entrypoint /bin/bash ubuntu:22.04
```
- Update and install git:

```
apt-get update
apt-get install -y git
```
- Clone repository:

```
git clone https://github.com/mcmchris/portenta-x8-flask-streamer.git
cd portenta-x8-flask-streaming
```
- Install pip to install other packages:

```
apt-get install python3-pip -y
pip install opencv-python
pip install Flask
```

- Install required tools:

```
apt install -y gcc g++ make build-essential nodejs sox gstreamer1.0-tools gstreamer1.0-plugins-good gstreamer1.0-plugins-base gstreamer1.0-plugins-base-apps vim v4l-utils usbutils udev

apt-get install libgl1
```

## Connect a USB Camera

Connect a USB camera to any of the USB-A connectors available on your carrier.

## Run the script

- Run the Python script:

```
python3 streaming.py
```

- Type the IP + Port prompted on your favorite browser as follows:

`http://<Portenta-IP>:4912/`

- Enjoy