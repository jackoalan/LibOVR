set(PLAT_SRCS "")
if(APPLE)
  list(APPEND PLAT_SRCS
       OVR_OSX_Display.cpp)
endif()
add_library(OVR-Displays
            OVR_Display.cpp
            ${PLAT_SRCS})
