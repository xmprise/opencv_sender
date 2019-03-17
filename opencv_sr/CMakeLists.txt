cmake_minimum_required(VERSION 3.7)
project(opencv_sr)

set(CMAKE_CXX_STANDARD 11)

find_package(OpenCV REQUIRED)

set(EXT_LIBS opencv_core
        opencv_highgui
        opencv_imgproc
        opencv_imgcodecs)

set(SOURCE_FILES main.cpp)
add_executable(opencv_sr ${SOURCE_FILES})
target_link_libraries(opencv_sr ${EXT_LIBS})