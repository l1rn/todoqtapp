cmake_minimum_required(VERSION 3.31)
project(untitled2)

set(CMAKE_PREFIX_PATH "/home/lirn/Qt/6.9.1/gcc_64" CACHE PATH "Path to Qt6 installation")

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

set(CMAKE_AUTOMOC ON)
set(CMAKE_AUTORCC  ON)
set(CMAKE_AUTOUIC  ON)

find_package(Qt6 REQUIRED COMPONENTS Core Widgets Gui)

add_executable(untitled2 main.cpp)

target_link_libraries(untitled2 PRIVATE Qt6::Core Qt6::Widgets  Qt6::Gui)

set(CMAKE_RUNTIME_OUTPUT_DIRECTORY "${CMAKE_BINARY_DIR}/bin")