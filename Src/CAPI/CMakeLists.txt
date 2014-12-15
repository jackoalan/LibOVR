set(GFX_SRCS "")
if(OVR_OPENGL)
  list(APPEND GFX_SRCS
       GL/CAPI_GL_DistortionRenderer.cpp
       GL/CAPI_GL_HSWDisplay.cpp
       GL/CAPI_GL_Util.cpp
       GL/CAPI_GLE.cpp)
endif()
add_library(OVR-CAPI
            CAPI_DistortionRenderer.cpp
            CAPI_FrameTimeManager.cpp
            CAPI_HMDRenderState.cpp
            CAPI_HMDState.cpp
            CAPI_HSWDisplay.cpp
            CAPI_LatencyStatistics.cpp
            ${GFX_SRCS})
