set(SRC_FILES Shader.cpp)

file(COPY shader
        DESTINATION ${CMAKE_CURRENT_BINARY_DIR})

add_executable(2.Shaders ${SRC_FILES})
target_link_libraries(2.Shaders ${GLFW_LIBRARIES} GLAD)
