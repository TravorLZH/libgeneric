cmake_minimum_required(VERSION 3.5)
project(libgeneric)

set(CMAKE_C_STANDARD 99)
set(CMAKE_BUILD_TYPE Debug)
set(LIBRARY_OUTPUT_PATH ${EXECUTABLE_OUTPUT_PATH})
set(ARCHIVE_OUTPUT_PATH ${LIBRARY_OUTPUT_PATH})

include_directories(${CMAKE_CURRENT_SOURCE_DIR}/include)
add_subdirectory(src)
add_subdirectory(Test)

enable_testing()