cmake_minimum_required(VERSION 3.0.0)

project(ML_Project VERSION 1.0.0)

add_library(libraries
src/data.cpp
src/data_handler.cpp
src/main.cpp)

add_executable(main
src/main.cpp)

target_include_directories(libraries PUBLIC include)
target_link_libraries(main PUBLIC libraries)




