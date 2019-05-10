set(SRC_FILES Main.cpp ../glad.c)

add_executable(Stub ${SRC_FILES})
target_link_libraries(Stub ${GLFW_LIBRARIES})
