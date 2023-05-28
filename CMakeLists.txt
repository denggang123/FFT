cmake_minimum_required(VERSION 3.0)

project(FFT)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -Wall")

set(CMAKE_BUILD_TYPE Debug)

include_directories(include)

set(SRC_LIST
	main.c
    src/zx_fft.c
    src/zx_math.c
    )

add_executable(main ${SRC_LIST})
