cmake_minimum_required(VERSION 2.8)

project(calculator)

set(SOURCE_EXE calculator2.cpp)

set(SOURCE_LIB calculator.cpp)

add_library(lib STATIC ${SOURCE_LIB})

add_executable(calculator ${SOURCE_EXE})

target_link_libraries(calculator lib)
