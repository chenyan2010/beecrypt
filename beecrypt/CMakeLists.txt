file( GLOB interface_files RELATIVE ${CMAKE_CURRENT_SOURCE_DIR} *.h)
file( GLOB implementation_files RELATIVE ${CMAKE_CURRENT_SOURCE_DIR} src/*.c)

source_group("Source" FILES ${implementation_files})
source_group("Interface" FILES ${interface_files})

add_library(beecrypt ${implementation_files} ${interface_files})
