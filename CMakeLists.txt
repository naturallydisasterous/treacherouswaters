cmake_minimum_required(VERSION 3.10)
project(TreacherousWaters)

set(CMAKE_CXX_FLAGS "-lglfw -lGL ")

find_package(GLEW REQUIRED)
include_directories(${GLEW_INCLUDE_DIRS})
link_libraries(${GLEW_LIBRARIES})

# Build

add_executable(tw 
  client/main.cpp
  )
