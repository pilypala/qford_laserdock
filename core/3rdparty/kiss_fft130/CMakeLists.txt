cmake_minimum_required(VERSION 3.11)

set(CMAKE_AUTOMOC OFF)

# library
add_library(kiss_fft130)
set_property(TARGET kiss_fft130 PROPERTY POSITION_INDEPENDENT_CODE ON)

target_sources(kiss_fft130 PRIVATE
    _kiss_fft_guts.h
    kiss_fft.c
    kiss_fft.h
    kissfft.hh
    tools/kiss_fftr.c
    tools/kiss_fftr.h
    )
