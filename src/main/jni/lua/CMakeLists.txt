
#set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -pie -fPIE")

add_definitions(-DLUA_DL_DLOPEN -DLUA_USE_C89 -DLUA_COMPAT_5_1 -DLUA_COMPAT_5_2 -DLUA_USE_LINUX)

#aux_source_directory(. DIR_LUA_SRCS)

add_library(lua STATIC lapi.c lauxlib.c lbaselib.c lbitlib.c lcode.c lcorolib.c lctype.c ldblib.c ldebug.c ldo.c ldump.c lfunc.c lgc.c linit.c liolib.c llex.c lmathlib.c lmem.c loadlib.c lobject.c lopcodes.c loslib.c lparser.c lstate.c lstring.c lstrlib.c ltable.c ltablib.c ltm.c lundump.c lutf8lib.c lvm.c lzio.c)
