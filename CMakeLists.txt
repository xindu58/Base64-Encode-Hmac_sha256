cmake_minimum_required(VERSION 3.22.0)   #版本号
project(hmac-sha256)  #定义工程名字
#包含头文件
include_directories(./)
add_library(hmac-sha256 SHARED base64.cpp hmac.cpp hmac_sha2.c sha2.c)

add_executable(main main.cpp base64.cpp hmac.cpp hmac_sha2.c sha2.c)

