# terminal commands
## No.1:
```
source devel/setup.bash && roslaunch rotors_gazebo fast_with_vi_sensor.launch
```

## No.2: 
```
source devel/setup.bash && roslaunch vid_estimator vid_sim.launch
```

## No.3: 
```
source devel/setup.bash && roslaunch resilient_planner rotors_sim.launch
```

## No.4: 
```
export PYTHONPATH=$PYTHONPATH:/home/alex/TEST-202111/KinoGPMPC-1110/src/data_driven_mpc/ros_gp_mpc
source devel/setup.bash && roslaunch ros_gp_mpc gp_mpc_wrapper.launch environment:=gazebo flight_mode:=kino plot:=True
```
# VINS-FUISON
## No.1:
```
source devel/setup.bash && roslaunch realsense2_camera rs_camera_vins.launch
```
## No.2: 
```
source devel/setup.bash && roslaunch vins vins_rviz.launch
```
## No.3: 
```
source devel/setup.bash && rosrun vins vins_node /home/alex/TEST-202111/VINS-FUSION/src/VINS-Fusion/config/realsense_d435i/realsense_stereo_imu_config.yaml

```
```
source devel/setup.bash && rosrun vins vins_node /home/alex/TEST-202111/VINS-Fusion-PIX4/src/VINS-Fusion/config/realsense_d435i/realsense_stereo_imu_config.yaml

```
## No.4 (optional): 
```
source devel/setup.bash && rosrun loop_fusion loop_fusion_node /home/alex/TEST-202111/VINS-FUSION/src/VINS-Fusion/config/euroc/euroc_stereo_imu_config.yaml 

```
```
source devel/setup.bash && rosrun loop_fusion loop_fusion_node /home/alex/VINS-Fusion-PIX4/VINS-FUSION/src/VINS-Fusion/config/euroc/euroc_stereo_imu_config.yaml 

```
# VINS-MOMO
## No.1:
```
source devel/setup.bash && roslaunch realsense2_camera rs_camera.launch 
```
## No.2: 
```
source devel/setup.bash && roslaunch vins_estimator realsense_color.launch 
```
## No.3: 
```
source devel/setup.bash && roslaunch vins_estimator vins_rviz.launch

```
