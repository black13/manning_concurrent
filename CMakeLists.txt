cmake_minimum_required (VERSION 2.6)
project (Test)
SET(CMAKE_CXX_FLAGS ${CMAKE_CXX_FLAGS} "-std=c++11 -pthread")

find_package (Threads)
add_executable (list_1.1 ./list_1.1.cpp)
target_link_libraries (list_1.1 ${CMAKE_THREAD_LIBS_INIT})

