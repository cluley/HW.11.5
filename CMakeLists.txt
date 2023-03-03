cmake_minimum_required(VERSION 3.22.0)

set(CMAKE_CXX_STANDARD 14)
set(CMAKE_CXX_STANDARD_ REQUIRED True)

project(Figures_Domain)

set(CMAKE_WINDOWS_EXPORT_ALL_SYMBOLS ON)
add_library(Figures SHARED figure.cpp triangle.cpp quadrangle.cpp rTriangle.cpp eTriangle.cpp iTriangle.cpp rectangle.cpp square.cpp parallelogram.cpp rhombus.cpp)

add_executable(Figures_Usage main.cpp)
target_link_libraries(Figures_Usage Figures)