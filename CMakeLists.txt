cmake_minimum_required(VERSION 2.8)
Project("beecrypt")

if (NOT "${CMAKE_BUILD_TYPE}" STREQUAL "ReleaseNoOutFiles") 
    add_definitions(-DLITTLE_ENDIAN)
    add_definitions(-DHAVE_SYS_TIME_H)
    add_definitions(-DHAVE_GETTIMEOFDAY)
    add_definitions(-DHAVE_ASSERT_H)
    add_definitions(-DHAVE_FCNTL_H)
endif() 

include_directories(${CMAKE_SOURCE_DIR})
add_subdirectory(beecrypt)
