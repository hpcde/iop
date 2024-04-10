cmake_minimum_required(VERSION 3.18)

project(iop)

set(CMAKE_CXX_STANDARD 11)

include(config.cmake)
include(dependency.cmake)

add_subdirectory(src)
