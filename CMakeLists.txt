cmake_minimum_required(VERSION 3.28)
project(ItestPure)

find_package(Boost REQUIRED)

include_directories(${Boost_INCLUDE_DIRS})

set(CMAKE_CXX_STANDARD 20)

add_executable(ItestPure main.cc)

target_link_libraries(ItestPure ${Boost_LIBRARY_DIRS})
