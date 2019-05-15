set(SRC_FILES HelloTriangle.cpp)

add_executable(1.HelloTriangle ${SRC_FILES})
target_link_libraries(1.HelloTriangle ${GLFW_LIBRARIES} GLAD)
