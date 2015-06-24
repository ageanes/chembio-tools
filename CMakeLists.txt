cmake_minimum_required(VERSION 2.8 FATAL_ERROR)
project(chembio CXX)

# use C++14 standard and the LLVM implementation of the C++ standard library
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++14 -stdlib=libc++")

add_subdirectory(src)
