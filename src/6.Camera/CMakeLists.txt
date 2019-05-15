set(SRC_FILES Camera.cpp)

file(COPY shader
        DESTINATION ${CMAKE_CURRENT_BINARY_DIR})
file(COPY Assets
        DESTINATION ${CMAKE_CURRENT_BINARY_DIR})

add_executable(6.Camera ${SRC_FILES})
target_link_libraries(6.Camera ${GLFW_LIBRARIES} GLAD)

add_executable(6.Camera2 Camera_with_class.cpp)
target_link_libraries(6.Camera2 ${GLFW_LIBRARIES} GLAD)
