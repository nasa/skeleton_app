cmake_minimum_required(VERSION 2.6.4)
project(CFE_SKELETON_APP C)

# Create the app module
add_cfe_app(skeleton_app fsw/src/skeleton_app.c)

target_include_directories(skeleton_app PUBLIC
  $<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}/fsw/platform_inc>
  $<INSTALL_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}/fsw/platform_inc> )
