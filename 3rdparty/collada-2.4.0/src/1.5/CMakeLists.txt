file(GLOB dom_files ${CMAKE_CURRENT_SOURCE_DIR}/dom/*.cpp)
add_library(colladadom150 STATIC ${dom_files})
set_target_properties(colladadom150 PROPERTIES COMPILE_FLAGS "${COLLADA_COMPILE_FLAGS}" LINK_FLAGS "${libpcrecpp_LDFLAGS_OTHERS}")
