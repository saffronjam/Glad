cmake_minimum_required(VERSION 3.1.0)
project(Glad)

file(GLOB INCLUDES "include")
file(GLOB SRC_FILES "src/glad.c")

add_library(Glad ${SRC_FILES})

target_include_directories(Glad PRIVATE "${INCLUDES}")
set (Glad_INCLUDES "${INCLUDES}" PARENT_SCOPE)