cmake_minimum_required(VERSION 3.10)
project(huff)

set(CMAKE_EXPORT_COMPILE_COMMANDS 1)
set(CMAKE_BUILD_TYPE Debug)

file(GLOB src
  src/*.h 
  src/*.c
)

add_executable(huff 
  ${src}
)

target_include_directories(huff PUBLIC src/)

