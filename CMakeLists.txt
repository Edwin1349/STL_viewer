cmake_minimum_required(VERSION 3.16)

project(STL_viewer LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

add_executable(STL_viewer main.cpp)

include(GNUInstallDirs)
install(TARGETS STL_viewer
    LIBRARY DESTINATION ${CMAKE_INSTALL_LIBDIR}
    RUNTIME DESTINATION ${CMAKE_INSTALL_BINDIR}
)
