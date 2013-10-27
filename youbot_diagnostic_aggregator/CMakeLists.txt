cmake_minimum_required(VERSION 2.8.3)
project(youbot_diagnostic_aggregator)
find_package(catkin REQUIRED)

catkin_package(
  CATKIN_DEPENDS 
    diagnostic_aggregator
)

install(DIRECTORY launch/
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}/launch
)
install(DIRECTORY config/
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}/config
)
