set(PLAT_SRCS "")
if(APPLE)
  list(APPEND PLAT_SRCS
       OVR_mach_exc_OSX.c
       OVR_ThreadsPthread.cpp)
endif()
add_library(OVR-Kernel
            OVR_Alg.cpp
            OVR_Allocator.cpp
            OVR_Atomic.cpp
            OVR_CRC32.cpp
            OVR_DebugHelp.cpp
            OVR_File.cpp
            OVR_FileFILE.cpp
            OVR_Lockless.cpp
            OVR_Log.cpp
            OVR_Math.cpp
            OVR_RefCount.cpp
            OVR_SharedMemory.cpp
            OVR_Std.cpp
            OVR_String_FormatUtil.cpp
            OVR_String_PathUtil.cpp
            OVR_String.cpp
            OVR_SysFile.cpp
            OVR_System.cpp
            OVR_ThreadCommandQueue.cpp
            OVR_Timer.cpp
            OVR_UTF8Util.cpp
            ${PLAT_SRCS})
