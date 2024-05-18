# CANSyntheticDataGenerator
Synthetic Data Generator for Controller Area Network CAN for study Sensors and ECUs communications methods

# Commands to Run
```
sudo apt-get update
sudo apt-get upgrade
git clone https://github.com/zombieCraig/ICSim.git
sudo apt-get install libsdl2-dev libsdl2-image-dev
sudo modprobe can
sudo modprobe vcan
sudo ip link add dev vcan0 type vcan
sudo ip link set up vcan0
cd ICSim
make all
./icsim vcan0
./controls vcan0
candump vcan0
cansniffer vcan0
./icsim -r vcan0
./controls -s [seed] vcan0
./controls -s [seed] -l 2 vcan0
```

Props to ZombieCraig's Repo and ICSim software for linux: https://github.com/zombieCraig/ICSim.git
