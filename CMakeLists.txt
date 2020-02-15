cmake_minimum_required(VERSION 3.15)
project(Skeleton)

set(CMAKE_CXX_STANDARD 11)

find_package(OpenGL)
find_package(GLEW)
find_package(GLUT)

include_directories(${OPENGL_INCLUDE_DIRS} ${GLEW_INCLUDE_DIRS} ${GLUT_INCLUDE_DIRS})
add_compile_options(-Werror -Wall)

add_executable(Skeleton
        framework.cpp
        framework.h
        Skeleton.cpp)

target_link_libraries(Skeleton ${OPENGL_LIBRARIES} ${GLEW_LIBRARIES} ${GLUT_LIBRARIES})