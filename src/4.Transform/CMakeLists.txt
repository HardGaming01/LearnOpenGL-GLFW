set(SRC_FILES Transform.cpp)

file(COPY shader
        DESTINATION ${CMAKE_CURRENT_BINARY_DIR})
file(COPY Assets
        DESTINATION ${CMAKE_CURRENT_BINARY_DIR})

add_executable(4.Transform ${SRC_FILES})
target_link_libraries(4.Transform ${GLFW_LIBRARIES} GLAD)
