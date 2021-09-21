# To build the package

After downloading and setting up your catkin workspace, type in catkin_make under that catkin_ws directory.
This will build the package again.

Below are given commands to launch the rviz file.

# Launch could be done in a few ways

## Launch with use_xacro:=true

Under the urdf directory type in
roslaunch navvis_description display.launch use_xacro:= true 

The rviz will launch the robot.xacro file. The wheels would appear as directed in the lab. The use_xacro is an arguement specified in the robot.xacro file, which gives you the option to launch the xacro file and not the urdf file if it is set to true.

## Launch with use_xacro:=true use_gui:=false

Under the urdf directory type in
roslaunch navvis_description display.launch use_xacro:=true use_gui:=false

The rviz will launch the robot.xacro file with the wheels as well as the joint_state_publisher_gui. This window helps you rotate the wheels using the sliders. It could be a bit hard to notice the rotation. 

## Launch with use_xacro:=true use_gui:=true

Under the urdf directory type in
roslaunch navvis_description display.launch use_xacro:=true use_gui:=true

The rviz will launch the robot.xacro file with the wheels but not the joint_state_publisher_gui window.

### Please note the arguement use_gui is misleading (should be named not_use_gui)
### The urdf_from_xacro.urdf should be treated as new robot.urdf, have committed both just in case. 
