cmake_minimum_required(VERSION 3.50)
project(libcal)

add_executable(libcal_test test/libcal_test.cpp)

add_custom_target(
    clean-all
    COMMAND ${CMAKE_COMMAND} -E rm -rf ${CMAKE_BINARY_DIR}/*
    COMMENT "Cleaning all build files"
)