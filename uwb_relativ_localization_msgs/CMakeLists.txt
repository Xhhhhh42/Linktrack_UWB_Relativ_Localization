cmake_minimum_required(VERSION 3.0.2)
project(uwb_relativ_localization_msgs VERSION 1.0.0)


find_package(catkin REQUIRED COMPONENTS
  roscpp
  geometry_msgs
  message_generation
  std_msgs
)

## Generate messages in the 'msg' folder
add_message_files(
  FILES
  relativ_loca.msg
)


## Generate actions in the 'action' folder
# add_action_files(
#   FILES
#   Action1.action
#   Action2.action
# )

## Generate added messages and services with any dependencies listed here
generate_messages(
  DEPENDENCIES
  geometry_msgs   std_msgs
)

catkin_package(
#  INCLUDE_DIRS include
#  LIBRARIES mapbag_editor_msg
#  CATKIN_DEPENDS geometry_msgs message_generation std_msgs
#  DEPENDS system_lib
)

###########
## Build ##
###########

## Specify additional locations of header files
## Your package locations should be listed before other locations
include_directories(
# include
  ${catkin_INCLUDE_DIRS}
)
