cmake_minimum_required(VERSION 3.4)
project(RenameIncludeHierarcy)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")

include_directories(dir1)

set(SOURCE_FILES main.cpp file1.cpp dir1/file11.c dir1/header12.h ../header11.h dir2/file21.cpp dir2/header21.h)
add_executable(RenameIncludeHierarcy ${SOURCE_FILES})