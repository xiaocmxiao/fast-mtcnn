cmake_minimum_required(VERSION 3.5)
project(fastmtcnn)

set(CMAKE_CXX_STANDARD 11)

find_package(OpenCV)

set(SOURCE_FILES mtcnn_opencv.cpp)
add_executable(fastmtcnn ${SOURCE_FILES})

target_link_libraries(fastmtcnn ${OpenCV_LIBS} )
