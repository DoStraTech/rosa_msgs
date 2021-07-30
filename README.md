# rosa_msgs
Custom ROS Messages for the RoSA project

# Types
Custom ROS Messages for the RoSA project

    FacialHeader.msg
    FacialData.msg
	Cube.msg:
        letters     string
        color       string
        x           float
        y           float
        layer       int
	ProjectionObject.msg
    Joint.msg   
        Contains Kinect v2 Joint: JointType, X,Y,Z as float
	
	JointType:
        SpineBase = 0,
        SpineMid = 1,
        Neck = 2,
        Head = 3,
        ShoulderLeft = 4,
        ElbowLeft = 5,
        WristLeft = 6,
        HandLeft = 7,
        ShoulderRight = 8,
        ElbowRight = 9,
        WristRight = 10,
        HandRight = 11,
        HipLeft = 12,
        KneeLeft = 13,
        AnkleLeft = 14,
        FootLeft = 15,
        HipRight = 16,
        KneeRight = 17,
        AnkleRight = 18,
        FootRight = 19,
        SpineShoulder = 20,
        HandTipLeft = 21,
        ThumbLeft = 22,
        HandTipRight = 23,
        ThumbRight = 24
    Body.msg
        Contains Kinect v2 Joints as Joint[], IsTracked as bool?
	
    KinectBodies.msg
        Contains Kinect v2 Bodies as Body[]

# How to install
$ cd ~/catkin_ws/src
$ git clone https://github.com/DoStraTech/rosa_msgs.git
$ cd ..
$ catkin_make
$ source devel/setup.bash
$ rosmsg package rosa_msgs
