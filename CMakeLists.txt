cmake_minimum_required(VERSION 3.3)

project(GLFWTutorial)

set(CMAKE_MODULE_PATH ${CMAKE_MODULE_PATH} "${CMAKE_SOURCE_DIR}/cmake")

message(STATUS "Find prefix is ${CMAKE_PREFIX_PATH}")

find_package(GLFW REQUIRED)

include_directories(include)
include_directories(${GLFW_INCLUDE_DIR})

message(STATUS "GLFW Libraries is ${GLFW_LIBRARIES}")

add_subdirectory(src)
