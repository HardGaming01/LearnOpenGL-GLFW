set(SRC_FILES HelloTriangle.cpp)

add_executable(HelloTriangle ${SRC_FILES})
target_link_libraries(HelloTriangle ${GLFW_LIBRARIES} GLAD)
