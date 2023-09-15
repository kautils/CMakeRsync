### CMakeRsync
* rsync for mingw. 
* only support mingw currently.

### example 
```c++
include(rsync/rsync.cmake)
rsync_3_2_7_1(rsync)
if(EXISTS ${rsync})
    execute_process(COMMAND ${rsync} -h OUTPUT_VARIABLE var ERROR_VARIABLE err)
    message(${var})
endif()
```

