cmake_minimum_required(VERSION 2.6.4)
project(CFE_SKELETON_APP C)

include_directories(fsw/mission_inc)
include_directories(fsw/platform_inc)

# Create the app module
add_cfe_app(skeleton_app fsw/src/skeleton_app.c)

