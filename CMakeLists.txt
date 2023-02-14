project(MainProject)

cmake_minimum_required(VERSION 2.4)

add_executable(main example/test.cc)

add_subdirectory(src)

#include_directories(src)

target_link_libraries(main CuckooFiltSupport)

