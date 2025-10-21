cmake_minimum_required(VERSION 3.16)
project(SerialPort)

# Add the serialport library as a static library
add_library(serialport STATIC
    src/SerialPort.cpp
)

# Specify the include directory
target_include_directories(serialport PUBLIC
    ${CMAKE_CURRENT_SOURCE_DIR}/include
)