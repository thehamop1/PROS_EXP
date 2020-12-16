cmake_minimum_required(VERSION 3.16)

project(CSUN_MATABOTS_ROBOT)
set(CMAKE_PROJECT_NAME CSUN_MATABOTS_ROBOT)
set(CMAKE_MODULE_PATH ${PROJECT_SOURCE_DIR}/cmake)

find_package( arm-gcc-toolchain )

set(CMAKE_RUNTIME_OUTPUT_DIRECTORY "${CMAKE_BINARY_DIR}/bin")
set(CMAKE_ARCHIVE_OUTPUT_DIRECTORY "${CMAKE_BINARY_DIR}/lib") 
set(CMAKE_LIBRARY_OUTPUT_DIRECTORY "${CMAKE_BINARY_DIR}/lib")

add_subdirectory(firmware)
add_subdirectory(include)
add_subdirectory(src)
add_subdirectory(Matabots)