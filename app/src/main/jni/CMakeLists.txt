cmake_minimum_required(VERSION 3.4.1)

set(CMAKE_VERBOSE_MAKEFILE on)

link_libraries(log)

add_executable(libhelper.so ${CMAKE_CURRENT_SOURCE_DIR}/helper.c)


link_libraries(jnigraphics)

add_library(pinger SHARED pinger.cpp ping.cpp os_generic.cpp CNFGFunctions.c CNFGDriver.cpp)