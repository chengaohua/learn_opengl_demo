cmake_minimum_required(VERSION 3.9)
project(openglDemo)

set(CMAKE_CXX_STANDARD 11)
find_package(glfw3 REQUIRED)
add_executable(hello_window_clear hello_window_clear/hello_window_clear.cpp src/glad/glad.c)
target_link_libraries(hello_window_clear GLEW  GL glfw rt m dl)