cmake_minimum_required(VERSION 3.16.3)

project(P2000_SDR)

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED True)

set(SRC_DIR "src")

set(src_files "${SRC_DIR}/main.cpp")
set(header_files)

message(STATUS "Using source files: ${src_files}")
message(STATUS "Using header files: ${header_files}")

if(NOT src_files)
    message(FATAL_ERROR "No source files found!")
endif()

add_executable(P2000_SDR ${src_files} ${header_files})
