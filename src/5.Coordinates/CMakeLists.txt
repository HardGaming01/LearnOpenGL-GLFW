set(SRC_FILES Coordinates.cpp)

file(COPY shader
        DESTINATION ${CMAKE_CURRENT_BINARY_DIR})
file(COPY Assets
        DESTINATION ${CMAKE_CURRENT_BINARY_DIR})

add_executable(Coordinates ${SRC_FILES})
target_link_libraries(Coordinates ${GLFW_LIBRARIES} GLAD)
