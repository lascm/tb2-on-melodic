# tb2-on-melodic

## Requirements

Base ROS-Desktop installation

`sudo apt install ros-melodic-desktop`

Additional packages required:

```
sudo apt install ros-melodic-ecl-threads \
                 ros-melodic-ecl-geometry \
                 ros-melodic-ecl-streams \
                 ros-melodic-kobuki-dock-drive \
                 ros-melodic-kobuki-driver \
                 ros-melodic-image-geometry \
                 ros-melodic-joy \
                 ros-melodic-depth-image-proc
```

## Clone the repo in `src` directory of a catkin workspace and build the packages.

### Unneseccary packages include a CATKIN_IGNORE in order to avoid problems building

`git clone https://github.com/lascm/tb2-on-melodic/`

#### Build using catkin

`catkin_make`

#### or using catking_tools

`catkin build`

#### Make sure udev rules are setup

`sudo apt install ros-melodic-kobuki-ftdi`

`rosrun kobuki_ftdi create_udev_rules`
