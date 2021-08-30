cmake_minimum_required(VERSION 2.8.3)
project(rosa_msgs)

find_package(catkin REQUIRED COMPONENTS
  rospy
  std_msgs
  geometry_msgs
  sensor_msgs
  message_generation
)

add_message_files(
  FILES
    FacialHeader.msg
    FacialData.msg
    CubeAction.msg
    RobotAction.msg
    Cube.msg
    ProjectionObject.msg
    Joint.msg
    Body.msg
    KinectBodies.msg
    Detection.msg
    Detections.msg
    HandBox.msg
    UserData.msg
)

#catkin_python_setup()

generate_messages(
  DEPENDENCIES
    geometry_msgs
    sensor_msgs
    std_msgs
)

catkin_package(
)

include_directories(
  ${catkin_INCLUDE_DIRS}
)




