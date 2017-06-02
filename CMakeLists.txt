cmake_minimum_required(VERSION 3.8)
project(CPlusPlusExperiment)

set(CMAKE_CXX_STANDARD 11)

find_package(SDL2 REQUIRED)
include_directories(${SDL2_INCLUDE_DIR})

set(SOURCE_FILES main.cpp)

add_executable(CPlusPlusExperiment ${SOURCE_FILES})

target_link_libraries(CPlusPlusExperiment ${SDL2_LIBRARY})