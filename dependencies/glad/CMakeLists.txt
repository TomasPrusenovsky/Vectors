cmake_minimum_required(VERSION 3.26)
set(CMAKE_CXX_STANDARD 23)

include_directories(include)

add_library(
        glad
        include/glad/glad.h
        include/KHR/khrplatform.h
        src/glad.c
)

