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
