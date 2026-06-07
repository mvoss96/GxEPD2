# GxEPD2 E-Paper Display Library
# https://github.com/mvoss96/GxEPD2
# GPL-3.0 License

cmake_minimum_required(VERSION 3.5)

file(GLOB_RECURSE GXEPD2_SRCS "${CMAKE_CURRENT_LIST_DIR}/src/*.cpp")

idf_component_register(SRCS ${GXEPD2_SRCS}
                       INCLUDE_DIRS "src"
                       REQUIRES arduino-esp32 Adafruit_GFX)

project(GxEPD2)
