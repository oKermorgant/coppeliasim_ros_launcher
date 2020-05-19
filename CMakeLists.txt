cmake_minimum_required(VERSION 2.8.3)
project(coppeliasim_ros_launcher)

find_package(catkin REQUIRED)

catkin_package()
 install(PROGRAMS
   coppelia_sim
   DESTINATION ${CATKIN_PACKAGE_BIN_DESTINATION})

 install(FILES
   coppelia_sim.launch
   DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}
 )
