# jetson-nano-setup
Repository containing setup commands used to setup the NVIDIA Jetson Nano

## Update
```
sudo apt-get update
```

## Install nano
```
sudo apt-get install nano -y
```

## Install Python 3.6 e PIP
```
sudo apt-get install python3.6-dev python3-pip -y
```

## Install numpy
```
pip3 install numpy
```

## Clone CSI camera demo
```
git clone https://github.com/JetsonHacksNano/CSI-Camera
```

## Test CSI camera
```
python3 CSI-Camera/face_detection.py
```

## Clone script for installing swap file
```
git clone https://github.com/JetsonHacksNano/installSwapfile.git
```

## Install swap file (6GB)
```
./installSwapfile/installSwapfile.sh
```

## Restart
```
sudo reboot
```

## Clone jetson stats
```
git clone https://github.com/rbonghi/jetson_stats.git
```

## Install jetson stats
```
sudo ./jetson_stats/install_jetson_stats.sh
```

## Run jetson stats
```
sudo ./jetson_stats/jtop.sh
```

## Install jupyter
```
pip3 install jupyter
```

## Start jupyter
```
jupyter notebook --ip=0.0.0.0
```

## Install HDF5
```
sudo apt-get install libhdf5-serial-dev hdf5-tools
```

## Install tensorflow GPU
```
pip3 install --extra-index-url https://developer.download.nvidia.com/compute/redist/jp/v42 tensorflow-gpu==1.13.1+nv19.3 --user
```
## Install libcanberra to avoid warnings
```
sudo apt install libcanberra-gtk-module libcanberra-gtk3-module
```
