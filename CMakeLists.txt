cmake_minimum_required(VERSION 3.23)
project(course C)

set(CMAKE_C_STANDARD 99)

add_executable(course main.c)

add_subdirectory(libs)
target_link_libraries(course algorithms)
target_link_libraries(course data_structures)