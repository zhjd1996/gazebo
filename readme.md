一、安装方法：
假设你的工作空间，名为catkin_ws：
1、将四个文件夹移到，catkin_ws/src下。
2、在catkin_ws/下执行：catkin_make
3、在catkin_ws/下执行：source ./devel/setup.bash

二、
1、rplidar_ros文件夹，为rplidar雷达的程序包；
2、其他三个文件夹：是三个功能包集（stack），内部包含多个功能包（package），如：
	turtlebot_apps内包含turtlebot_navigation(用于导航相关)等

	turtlebot_simulator内包含turtlebot_gazebo（用于gazebo仿真）等
	
	turtlebot-kinetic内包含turtlebot_bringup（启动机器人）、turtlebot_description（仿真所需的3D模型）、turtlebot_teleop（遥控机器人）等
	
	具体内容可以去ros wiki上查看。
三、部分指令
1、启动gazebo仿真
roslaunch turtlebot_gazebo turtlebot_world.launch
2、建图
roslaunch turtlebot_navigation gazebo_gmapping.launch
