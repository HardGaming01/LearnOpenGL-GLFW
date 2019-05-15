set(SRC_FILES Shader.cpp)

file(COPY shader
        DESTINATION ${CMAKE_CURRENT_BINARY_DIR})

add_executable(Shaders ${SRC_FILES})
target_link_libraries(Shaders ${GLFW_LIBRARIES} GLAD)
