cmake_minimum_required(VERSION 2.8.11)
project (rootproject)

set(CMAKE_BINARY_DIR ${CMAKE_SOURCE_DIR}/build)

set(EXECUTABLE_OUTPUT_PATH ${CMAKE_BINARY_DIR})
set(LIBRARY_OUTPUT_PATH ${CMAKE_BINARY_DIR})

set(PROJECT_INCLUDE_DIR ${PROJECT_SOURCE_DIR}/include)

include_directories("${PROJECT_INCLUDE_DIR}")
include_directories("${PROJECT_SOURCE_DIR}")

message( "CMAKE_BINARY_DIR is ${CMAKE_BINARY_DIR}" )
message( "CMAKE_SOURCE_DIR is ${CMAKE_SOURCE_DIR}" )
add_subdirectory(sdl2)
add_subdirectory(game)

