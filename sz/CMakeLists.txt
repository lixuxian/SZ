aux_source_directory(src sz_sources)

add_library (SZ SHARED ${sz_sources})
target_link_libraries (SZ zlib zstd)

install (TARGETS SZ LIBRARY DESTINATION lib)
