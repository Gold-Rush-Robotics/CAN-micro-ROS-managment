# CAN-micro-ROS-managment

-! WORK IN PROGRESS REPO !- 

None of this is garunteed to work in its current state

## Pull the Dockerimage for building Zephr

X86-64
docker pull ghcr.io/gold-rush-robotics/zephyr-build:3

Arm
docker pull ghcr.io/gold-rush-robotics/zephyr-build:2arm


## Run the Docker container

X86-64
docker run -it --privileged ghcr.io/gold-rush-robotics/zephyr-build:3

Arm
docker run -it --privileged ghcr.io/gold-rush-robotics/zephyr-build:2arm


## Build code

```bash
west build -p always -b TEENSY40 <filepath>
```

## Flash via USB

```bash
west flash
```

