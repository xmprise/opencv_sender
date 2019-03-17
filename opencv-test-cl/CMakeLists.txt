cmake_minimum_required(VERSION 3.7)
project(opencv_test_cl)

set(CMAKE_CXX_STANDARD 11)

find_package(OpenCV REQUIRED )

set(EXT_LIBS opencv_core
        opencv_imgcodecs
        opencv_highgui
        opencv_imgproc
        opencv_calib3d
        opencv_features2d)
set(SOURCE_FILES main.cpp)

add_executable(opencv_test_cl ${SOURCE_FILES})
target_link_libraries(opencv_test_cl ${EXT_LIBS})
