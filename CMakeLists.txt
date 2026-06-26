cmake_minimum_required(VERSION 4.3)

set(CMAKE_CXX_STANDARD 26)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)
set(CMAKE_EXPORT_COMPILE_COMMANDS ON)

set(CMAKE_CXX_SCAN_FOR_MODULES ON)

project(nearest-neighbors LANGUAGES CXX)
add_subdirectory(nearest-neighbors)

option(TESTS "Building tests..." ON)
if(TESTS)
    add_subdirectory(tests)
endif()
