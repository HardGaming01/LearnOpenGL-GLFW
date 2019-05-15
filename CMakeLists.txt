cmake_minimum_required(VERSION 3.3)

project(GLFWTutorial)

set(CMAKE_MODULE_PATH ${CMAKE_MODULE_PATH} "${CMAKE_SOURCE_DIR}/cmake")

if(MSVC)
  # Modify this path to point to your libraries if you are using microsoft compiler
  set(CMAKE_PREFIX_PATH "C:/CXXDev/vc++")
endif(MSVC)

find_package(GLFW REQUIRED)
find_package(GLM REQUIRED)

include_directories(include)
include_directories(${GLFW_INCLUDE_DIR})

message(STATUS "GLM Include directories is ${GLM_INCLUDE_DIR}")
message(STATUS "GLFW Libraries is ${GLFW_LIBRARIES}")

add_subdirectory(src)
