cmake_minimum_required(VERSION 2.8)
project( video )
find_package( OpenCV 3 REQUIRED )
add_executable( video video.cpp )
target_link_libraries( video ${OpenCV_LIBS} pthread portaudio asound)
