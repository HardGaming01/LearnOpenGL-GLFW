set(SRC_FILES Shader.cpp ../glad.c)

file(COPY shader
        DESTINATION ${CMAKE_CURRENT_BINARY_DIR})

add_executable(Shaders ${SRC_FILES})
target_link_libraries(Shaders ${GLFW_LIBRARIES})
