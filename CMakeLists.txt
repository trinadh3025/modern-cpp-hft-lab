cmake_minimum_required(VERSION 3.20)

project(modern_cpp_hft_lab
    VERSION 0.1.0
    LANGUAGES CXX
)

# C++ Standard
set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)

#Compiler Warnings
If(CMAKE_CXX_COMPILER_ID MATCHES "GNU|Clang")
	
	add_compile_options(
		-Wall
		-Wextra
		-Wpedantic
		-Wconversion
		-Wsign-conversion
	)

endif()

# Exercises

add_executable(
    hello_modern_cpp
    01_modern_cpp/01_hello_modern_cpp/main.cpp
)
