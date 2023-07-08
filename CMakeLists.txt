cmake_minimum_required(VERSION 3.25)
project(opengl_base)

set(CMAKE_CXX_STANDARD 14)

find_package(glfw3 REQUIRED)
find_package(glew REQUIRED)
find_package(OpenGL REQUIRED)
find_package(glm REQUIRED)
find_package(assimp CONFIG REQUIRED)

add_executable(opengl_base src/main.cpp)

target_link_libraries(opengl_base PRIVATE GLEW::GLEW glfw opengl32 glm::glm assimp::assimp)
