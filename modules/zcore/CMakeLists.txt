﻿include_directories(${PROJECT_SOURCE_DIR})
include_directories(${PROJECT_SOURCE_DIR}/modules)
if (WIN32)
	# 头文件目录，OpenCV + Kinect SDK 2.0
	set(OPENCV_INCLUDE "$ENV{OPENCV_DIR}/build/include;$ENV{OPENCV_DIR}/build/include/opencv2")
	set(KINECT_INCLUDE "$ENV{KINECTSDK20_DIR}/inc")
	include_directories(${OPENCV_INCLUDE})
	include_directories(${KINECT_INCLUDE})
endif()