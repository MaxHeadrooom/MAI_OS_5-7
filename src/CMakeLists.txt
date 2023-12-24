cmake_minimum_required(VERSION 3.20)
project(lab5-7)

set(CMAKE_CXX_STANDARD 17)

find_package(wrap_zmq)

add_executable(lab6 ClientProgramm.cpp)
target_link_libraries(lab6 zmq)

add_executable(server ServerProgramm.cpp)

target_link_libraries(server zmq)