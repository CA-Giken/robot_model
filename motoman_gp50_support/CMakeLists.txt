cmake_minimum_required(VERSION 2.8.3)

project(motoman_gp50_support)

find_package(catkin REQUIRED)

catkin_package()

if (CATKIN_ENABLE_TESTING)
  find_package(roslaunch REQUIRED)
endif()

install(DIRECTORY config meshes urdf
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION})
