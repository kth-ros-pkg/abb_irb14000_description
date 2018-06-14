cmake_minimum_required(VERSION 2.8.3)
project(abb_irb14000_description)

find_package(catkin REQUIRED COMPONENTS roslaunch)

catkin_package(
    CATKIN_DEPENDS roslaunch
)

roslaunch_add_file_check(launch/export_urdf.launch)
roslaunch_add_file_check(launch/view_model.launch)

