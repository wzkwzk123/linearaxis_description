cmake_minimum_required(VERSION 2.8.3)
project(linearaxis_description)

find_package(catkin REQUIRED COMPONENTS roslaunch)
catkin_package()

if(CATKIN_ENABLE_TESTING)
  find_package(roslaunch REQUIRED)
  roslaunch_add_file_check(launch/display.launch)
endif()
install(DIRECTORY meshes launch rviz urdf
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION})
