cmake_minimum_required(VERSION 3.5)
project("Beef")

if(NOT CMAKE_BUILD_TYPE)
  set(CMAKE_BUILD_TYPE "Debug")
  message(STATUS "Build type not specified: Use Debug by default.")
endif(NOT CMAKE_BUILD_TYPE)

add_subdirectory(extern/hunspell)
add_subdirectory(BeefySysLib)
add_subdirectory(IDEHelper)
add_subdirectory(BeefBoot)
add_subdirectory(BeefRT)
