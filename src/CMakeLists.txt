cmake_minimum_required(VERSION 3.5)

add_library(uzlib tinflate.c tinfgzip.c tinfzlib.c adler32.c crc32.c
  defl_static.c genlz77.c)

target_include_directories(uzlib PUBLIC $(CMAKE_CURRENT_SOURCE_DIR))
