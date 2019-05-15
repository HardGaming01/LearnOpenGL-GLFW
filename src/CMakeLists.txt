include_directories(src)

add_library(GLAD STATIC glad.c)

add_subdirectory(1.HelloTriangle)
add_subdirectory(2.Shaders)
add_subdirectory(3.Texture)
add_subdirectory(4.Transform)
add_subdirectory(5.Coordinates)
add_subdirectory(6.Camera)
