set(PLAT_SRCS "")
if(APPLE)
  list(APPEND PLAT_SRCS
       Util_SystemGUI_OSX.mm
       Util_SystemInfo_OSX.mm)
endif()
add_library(OVR-Util
            Util_ImageWindow.cpp
            Util_Interface.cpp
            Util_LatencyTest2Reader.cpp
            Util_Render_Stereo.cpp
            Util_SystemGUI.cpp
            Util_SystemInfo.cpp
            ${PLAT_SRCS})
