set(SRC_FILES Transform.cpp)

file(COPY shader
        DESTINATION ${CMAKE_CURRENT_BINARY_DIR})
file(COPY Assets
        DESTINATION ${CMAKE_CURRENT_BINARY_DIR})

add_executable(Transform ${SRC_FILES})
target_link_libraries(Transform ${GLFW_LIBRARIES} GLAD)
