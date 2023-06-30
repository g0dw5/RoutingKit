cmake_minimum_required(VERSION 3.14)
project(RoutingKit)

set(CMAKE_CXX_STANDARD 23)

include_directories(${CMAKE_SOURCE_DIR}/include/)

add_subdirectory(module)
add_subdirectory(osm)
add_subdirectory(main)
add_subdirectory(test)


