cmake_minimum_required(VERSION 3.14)
project(module)

set(CMAKE_CXX_STANDARD 17)

FILE(GLOB_RECURSE SOURCE_FILES *.cpp *.h)

add_library(${PROJECT_NAME} STATIC ${SOURCE_FILES})
