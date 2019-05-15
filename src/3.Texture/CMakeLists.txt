set(SRC_FILES Texture.cpp)

file(COPY shader
        DESTINATION ${CMAKE_CURRENT_BINARY_DIR})
file(COPY Assets
        DESTINATION ${CMAKE_CURRENT_BINARY_DIR})

add_executable(3.Texture ${SRC_FILES})
target_link_libraries(3.Texture ${GLFW_LIBRARIES} GLAD)
