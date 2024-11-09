cmake_minimum_required(VERSION 3.0)
 
project(Demo)
 
set(OpenCV_DIR "/usr/local/include/opencv4") #对应上面刚查的目录
 
find_package(OpenCV 4.9 REQUIRED)
message("find ${OpenCV_VERSION}")
add_executable(Demo test.cpp)
target_link_libraries(Demo ${OpenCV_LIBRARIES})


