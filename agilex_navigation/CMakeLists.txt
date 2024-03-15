################################################################################
# Set minimum required version of cmake, project name and compile options
################################################################################
cmake_minimum_required(VERSION 3.0.2)
project(agilex_navigation)

################################################################################
# Find catkin packages and libraries for catkin and system dependencies
################################################################################
find_package(catkin REQUIRED COMPONENTS
  rospy
  std_msgs
  geometry_msgs
  sensor_msgs
  move_base_msgs
  move_base
  dwa_local_planner
  global_planner
)

################################################################################
# Declare catkin specific configuration to be passed to dependent projects
################################################################################
catkin_package(
  CATKIN_DEPENDS
    std_msgs
    geometry_msgs
    move_base_msgs
)

include_directories(
# include
  ${catkin_INCLUDE_DIRS}
)
