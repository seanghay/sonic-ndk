cmake_minimum_required(VERSION 3.4.1)

add_library(sonic SHARED
            sonicjni.c
            sonic.c)

# Include libraries needed for hello-jni lib
target_link_libraries(sonic
                      android
                      log)