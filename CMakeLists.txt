cmake_minimum_required(VERSION 3.20)

project(hello-world)

add_executable(app main.cpp)

set(CPACK_DEBIAN_PACKAGE_MAINTAINER "Navarro, Pierre")
set(CPACK_BINARY_DEB "ON")
set(CPACK_BINARY_FREEBSD "OFF")
set(CPACK_BINARY_IFW "OFF")
set(CPACK_BINARY_NSIS "OFF")
set(CPACK_BINARY_RPM "OFF")
set(CPACK_BINARY_STGZ "OFF")
set(CPACK_BINARY_TBZ2 "OFF")
set(CPACK_BINARY_TGZ "ON")
set(CPACK_BINARY_TXZ "OFF")
set(CPACK_BINARY_TZ "OFF")

install(TARGETS app RUNTIME DESTINATION bin)
include(CPack)
