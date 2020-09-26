cmake_minimum_required(VERSION 3.0.2)
project(turtlebot2_training)

find_package(catkin REQUIRED COMPONENTS
  rospy
)

catkin_package()

install(DIRECTORY launch DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION} PATTERN "start_training.launch" EXCLUDE)
install(DIRECTORY config DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION})