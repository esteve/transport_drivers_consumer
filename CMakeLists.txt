cmake_minimum_required(VERSION 3.5)
project(transport_drivers_consumer)

#dependencies
find_package(ament_cmake_auto REQUIRED)
ament_auto_find_build_dependencies()

message("==== ${udp_driver_LIBRARIES}")
ament_auto_add_library(${PROJECT_NAME} SHARED
        src/main.cpp
)

ament_auto_package()
