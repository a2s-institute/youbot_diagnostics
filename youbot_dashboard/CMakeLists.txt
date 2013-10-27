cmake_minimum_required(VERSION 2.8.3)
project(youbot_dashboard)
find_package(catkin REQUIRED)

catkin_package()
catkin_python_setup()


install(FILES plugin.xml
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}
)

install(PROGRAMS ros/scripts/youbot_dashboard
  DESTINATION ${CATKIN_PACKAGE_BIN_DESTINATION}
)

install(DIRECTORY ros/launch/
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}/ros/launch
)

install(DIRECTORY common/images/
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}/common/images
)
