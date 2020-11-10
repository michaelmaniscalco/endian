add_library(endian INTERFACE
    src/include/endian.h
    src/include/endian_type.h
    src/include/endian_swap.h
    src/include/byte_swap.h)

target_include_directories(endian INTERFACE 
  $<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}/src>
  $<INSTALL_INTERFACE:include/endian>
)

