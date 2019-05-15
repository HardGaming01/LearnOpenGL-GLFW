set(SRC_FILES Camera.cpp)

file(COPY shader
        DESTINATION ${CMAKE_CURRENT_BINARY_DIR})
file(COPY Assets
        DESTINATION ${CMAKE_CURRENT_BINARY_DIR})

add_executable(Camera ${SRC_FILES})
target_link_libraries(Camera ${GLFW_LIBRARIES} GLAD)

add_executable(Camera2 Camera_with_class.cpp)
target_link_libraries(Camera2 ${GLFW_LIBRARIES} GLAD)
