set(PLAT_SRCS "")
if(APPLE)
  list(APPEND PLAT_SRCS
       OVR_OSX_Display.cpp
       OVR_OSX_FocusObserver.mm
       OVR_OSX_FocusReader.mm)
endif()
add_library(LibOVR-Displays
            OVR_Display.cpp
            ${PLAT_SRCS})
