cmake_minimum_required(VERSION 3.3)

project(GLFWTutorial)

set(CMAKE_MODULE_PATH ${CMAKE_MODULE_PATH} "${CMAKE_SOURCE_DIR}/cmake")

message(STATUS "Find prefix is ${CMAKE_PREFIX_PATH}")

find_package(GLFW REQUIRED)
find_package(GLEW REQUIRED)
find_package(SDL2 REQUIRED)

include_directories(include)
include_directories(${GLFW_INCLUDE_DIR})
include_directories(${GLEW_INCLUDE_DIRS})

message(STATUS "GLFW Libraries is ${GLFW_LIBRARIES}")
message(STATUS "GLEW Libraries is ${GLEW_LIBRARIES}")

add_subdirectory(src)
