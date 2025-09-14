# mocap_ws

Create workspace:
```bash
mkdir ~/mocap_ws && cd ~/mocap_ws
```

Clone this repo and move it into ~/mocap_ws/src:
```bash
git clone git@github.com:evannsm/mocap_ws.git
mv mocap_ws src && cd src
git submodule update --init --recursive
```

Now compile out-of-source with ROS2:
```bash
cd ~/mocap_ws/
colcon build --symlink-install
```

A standard error output is to be expected and is safe to ignore:
```
Finished <<< mocap4r2_optitrack_driver [9.61s]                                                                                                         
--- stderr: rqt_mocap4r2_control                                                                          
/home/egmc/mocap_ws/src/mocap4r2/mocap4r2_control/rqt_mocap4r2_control/include/rqt_mocap4r2_control/SystemController.hpp:0: Note: No relevant classes found. No output generated.
---
```
