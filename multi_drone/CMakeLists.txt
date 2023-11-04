cmake_minimum_required(VERSION 3.0.2)
project(multi_drone)
find_package(catkin REQUIRED COMPONENTS
  roscpp
  std_msgs
  geometry_msgs
  mavros
)

catkin_package()

include_directories(
  include
  ${catkin_INCLUDE_DIRS}
)

add_executable(${PROJECT_NAME}_node src/multi_drone_node.cpp)
target_link_libraries(${PROJECT_NAME}_node ${catkin_LIBRARIES})

