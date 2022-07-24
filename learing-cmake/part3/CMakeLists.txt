cmake_minimum_required(VERSION 3.19.0)

project(LearnCMakePart3 VERSION 1.0)

add_executable(${PROJECT_NAME} main.cpp "Adder/adder.cpp" "Adder/adder.h")

add_subdirectory(Adder)

target_link_libraries(${PROJECT_NAME} adder)