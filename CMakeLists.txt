cmake_minimum_required(VERSION 3.20)

set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/bin)

project(OpenGL)

add_subdirectory(glfw)

add_executable(OpenGL
        main.cpp
        )

target_link_libraries(OpenGL
        PRIVATE
        glfw -lGL
        )
