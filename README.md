# rosa_msgs
Custom ROS Messages for the RoSA project

# Types
Custom ROS Messages for the RoSA project

    FacialHeader.msg
    FacialData.msg
	Cube.msg
	ProjectionObject.msg
    Joint.msg   
        Contains Kinect v2 Joint: Type, X,Y,Z
    Body.msg
        Contains Kinect v2 Joints, IsTracked?
    KinectBodies.msg
        Contains Kinect v2 Bodies

# How to install
$ cd ~/catkin_ws/src
$ git clone https://github.com/DoStraTech/rosa_msgs.git
$ cd ..
$ catkin_make
$ source devel/setup.bash
$ rosmsg package rosa_msgs
