cmake_minimum_required(VERSION 3.12.0 )

project(cppunit-playground)

set (CMAKE_MODULE_PATH  ${CMAKE_MODULE_PATH}
                        ${CMAKE_CURRENT_SOURCE_DIR}/CMake)

include(CTest)

find_package(cppunit REQUIRED)
find_package(Threads REQUIRED)

add_definitions(-std=c++11)

add_subdirectory(src)

add_subdirectory(test)
