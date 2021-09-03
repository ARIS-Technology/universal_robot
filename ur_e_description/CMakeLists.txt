cmake_minimum_required(VERSION 3.5)
project(ur_e_description)

# find_package(catkin REQUIRED)
find_package(ament_cmake REQUIRED)

# catkin_package(
#  INCLUDE_DIRS include
#  LIBRARIES ur_e_description
#  CATKIN_DEPENDS urdf
#  DEPENDS system_lib
# )

install(DIRECTORY launch DESTINATION share/${PROJECT_NAME})
install(DIRECTORY urdf DESTINATION share/${PROJECT_NAME})
install(DIRECTORY meshes DESTINATION share/${PROJECT_NAME})

ament_package()