set(SRC_FILES Texture.cpp ../glad.c)

file(COPY shader
        DESTINATION ${CMAKE_CURRENT_BINARY_DIR})
file(COPY Assets
        DESTINATION ${CMAKE_CURRENT_BINARY_DIR})

add_executable(Texture ${SRC_FILES})
target_link_libraries(Texture ${GLFW_LIBRARIES})
