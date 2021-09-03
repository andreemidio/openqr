cmake_minimum_required(VERSION 3.20)
project(OpenQR)

set(CMAKE_CXX_STANDARD 11)

find_package(OpenCV REQUIRED)
find_package(Threads)

add_executable(OpenQR main.cpp include/OpenQR.cpp include/OpenQR.h)


target_link_libraries(OpenQR ${OpenCV_LIBS})