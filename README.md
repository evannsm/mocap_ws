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


