cmake_minimum_required(VERSION 3.7)
project(main)

set(CMAKE_MODULE_PATH ${CMAKE_MODULE_PATH} "/usr/lib/")
find_package(cpprestsdk REQUIRED)

add_executable(main main.cpp)
target_link_libraries(main PRIVATE cpprestsdk::cpprest)