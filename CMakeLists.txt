cmake_minimum_required(VERSION 3.10)
project(OpenGL__Work)

set(CMAKE_CXX_STANDARD 11)

# Find and link OpenGL and GLUT
find_package(OpenGL REQUIRED)
find_package(GLUT REQUIRED)

add_executable(OpenGL__Work main.cpp)

# Link the libraries
target_link_libraries(OpenGL__Work PRIVATE OpenGL::GL GLUT::GLUT)
