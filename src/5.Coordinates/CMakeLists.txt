set(SRC_FILES Coordinates.cpp)

file(COPY shader
        DESTINATION ${CMAKE_CURRENT_BINARY_DIR})
file(COPY Assets
        DESTINATION ${CMAKE_CURRENT_BINARY_DIR})

add_executable(5.Coordinates ${SRC_FILES})
target_link_libraries(5.Coordinates ${GLFW_LIBRARIES} GLAD)
