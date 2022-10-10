cmake_minimum_required(VERSION 3.20)

project(hello_world)

add_executable(app main.cpp)

set(CPACK_DEBIAN_PACKAGE_MAINTAINER "Navarro, Pierre")

install(TARGETS app RUNTIME DESTINATION bin)
include(CPack)