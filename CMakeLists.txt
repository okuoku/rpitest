# No toolchain file required
#
# FIXME: Enfoce PICO_BOARD=vgaboard ?

cmake_minimum_required(VERSION 3.13)

include(pico-sdk/pico_sdk_init.cmake)

project(rpitest C CXX)

set(PICO_SDK_POST_LIST_DIRS ${CMAKE_CURRENT_LIST_DIR}/pico-extras)

pico_sdk_init()

add_subdirectory(pico-playground)
