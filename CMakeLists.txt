cmake_minimum_required(VERSION 3.0.0)
project(clox LANGUAGES C)

include(CTest)
enable_testing()

file(GLOB SOURCES ${CMAKE_SOURCE_DIR}/*.c)

add_executable(clox ${SOURCES})


set(CPACK_PROJECT_NAME ${PROJECT_NAME})
set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})
include(CPack)
