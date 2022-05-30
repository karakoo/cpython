cmake_minimum_required(VERSION 3.0)
project(cpython)

file(GLOB SOURCE_FILES
		Python/*.c
		Parser/*.c
		Objects/*.c
		Modules/*.c)

include_directories(Include)
include_directories(Include/internal)
include_directories(Include/cpython)

add_executable(cpython ${SOURCE_FILES})