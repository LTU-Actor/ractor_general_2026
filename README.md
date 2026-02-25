# README
This folder is simply a tool to help devs install and code for the IGVC 2026 project (change ts english is not even my first language)

Description of the project. talk about IGVC, our car, years won, a bit of everything idk

## Setup
```bash
sudo apt install ros-jazzy-desktop      # Install ROS2. Check [documentation](https://docs.ros.org/en/jazzy/Installation/Ubuntu-Install-Debs.html) for any problems
mkdir rACTOr2026                        # Create a parent folder named rACTOR2026
cd rACTOr2026                           # Enter the parent folder
python3 -m venv .venv                   # Create a virtual environment
source .venv/bin/activate               # Activate the virtual environment
pip install -r requirements.txt         # Install dependencies
source /opt/ros/jazzy/setup.bash        # Source the ROS2 environment
        # If you have vcstool installed
        git clone https://github.com/LTU-Actor/ractor-general-2026
        vcs import < <Folder_name.repos>    #Import the repositories needed (Check below for the folder structure)
        # If you don't
        mkdir <Folder_name>
        cd <Folder_name>
        git clone https://github.com/LTU-Actor/<repo_name>
```

## Repos organization
```txt
rACTOr2026/
│
├── control/
│   │
│   ├── control_tower_ros2/
│   │
│   └── ibus_reader/
│
├── driving/
│   │
│   ├── mqtt_wheel_bridge/
│   │
│   ├── nav2_schoolbus/
│   │
│   └── schoolbus_odrive_config/
│
├── vision/
│   │
│   ├── blob_follow_ros2/
│   │
│   ├── cloud_regions_cpp/
│   │
│   ├── cloud_regions_python/
│   │
│   ├── image_hsv_masker/
│   │
│   ├── pothole_detector/
│   │
│   ├── route_yolo_ros2/
│   │
│   ├── routecam_ros2/
│   │
│   └── usbcam_simple_ros2/
│
├── misc/
│   │
│   ├── IGVC-WT32ETH01/
│   │
│   ├── rACTOr_pi_launches/
│   │
│   └── schoolbus_description/
│
└── ractor_general_2026/
```
