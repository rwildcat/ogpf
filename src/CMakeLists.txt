# make library
add_library (ogpf STATIC ogpf.f90)

# any targets that link to this lib must also need that include directory
target_include_directories (ogpf PUBLIC ${CMAKE_BINARY_DIR}/src)

# install targets:
install (TARGETS ogpf DESTINATION lib)

# install .mod header
install (FILES ${CMAKE_BINARY_DIR}/src/ogpf.mod DESTINATION include)
