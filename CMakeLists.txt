cmake_minimum_required(VERSION 2.8.4)
project(SOIL)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")

set(SOURCE_FILES
    src/original/stb_image-1.09.c
    src/original/stb_image-1.16.c
    src/image_DXT.c
    src/image_DXT.h
    src/image_helper.c
    src/image_helper.h
    src/SOIL.c
    src/SOIL.h
    src/stb_image_aug.c
    src/stb_image_aug.h
    src/stbi_DDS_aug.h
    src/stbi_DDS_aug_c.h
    src/test_SOIL.cpp)

add_executable(SOIL ${SOURCE_FILES})