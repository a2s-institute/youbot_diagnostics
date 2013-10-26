cmake_minimum_required(VERSION 2.8.3)
project(youbot_diagnostic_aggregator)
find_package(catkin REQUIRED)

catkin_package(
  CATKIN_DEPENDS 
    diagnostic_aggregator
)

install(DIRECTORY ros/launch/
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}/ros/launch
)
install(DIRECTORY ros/config/
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}/ros/config
)
