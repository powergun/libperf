
add_library(cperf SHARED
    libperf.c
    libperf.h)
set_target_properties(cperf
    PROPERTIES
    CXX_STANDARD 11
    POSITION_INDEPENDENT_CODE ON)


add_executable(cperf_example
    libperf.h
    libperf.c
    libperf_example.c)
set_target_properties(cperf_example
    PROPERTIES
    POSITION_INDEPENDENT_CODE ON)

