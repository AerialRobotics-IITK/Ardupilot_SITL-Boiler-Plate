cmake_minimum_required(VERSION 3.0.2)
project(single_drone)
find_package(catkin REQUIRED COMPONENTS
  roscpp
  std_msgs
  geometry_msgs
  mavros
)

catkin_package()

include_directories(${catkin_INCLUDE_DIRS})

add_executable(${PROJECT_NAME}_node src/single_drone_node.cpp)
target_link_libraries(${PROJECT_NAME}_node ${catkin_LIBRARIES})
