cmake_minimum_required(VERSION 3.16)

project(mynet LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

add_executable(mynet
    src/main.cpp
)

target_include_directories(mynet PRIVATE include)

target_compile_options(mynet PRIVATE
    -Wall
    -Wextra
    -Wpedantic
)
