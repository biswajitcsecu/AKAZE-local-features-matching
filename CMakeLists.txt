


cmake_minimum_required(VERSION 3.10)

project( akaze_local_features_matching)

find_package(OpenCV REQUIRED)
find_package(VISP REQUIRED)
include_directories(${VISP_INCLUDE_DIRS})

include_directories(${OpenCV_INCLUDE_DIRS})

add_executable( akaze_local_features_matching akaze_local_features_matching.cpp )

include_directories(${VISP_INCLUDE_DIRS})

target_link_libraries( akaze_local_features_matching ${OpenCV_LIBS} ${VISP_LIBRARIES})


 
