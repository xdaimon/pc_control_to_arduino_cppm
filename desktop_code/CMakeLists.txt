cmake_minimum_required(VERSION 3.1)
project(main)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -O3 -std=c++11")

set(SOURCE_FILES
		main.cpp
		joystick.cpp
   )

include_directories(.)

add_executable(main ${SOURCE_FILES})

target_link_libraries(main serial pthread)

