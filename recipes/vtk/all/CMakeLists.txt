cmake_minimum_required(VERSION 3.4)
project(cmake_wrapper)

set (CXX_STANDARD_REQUIRED ON)
set (CMAKE_CXX_STANDARD 17)

if(WIN32 AND BUILD_SHARED_LIBS)
  set(CMAKE_WINDOWS_EXPORT_ALL_SYMBOLS ON)
endif()

add_subdirectory(source_subfolder)
