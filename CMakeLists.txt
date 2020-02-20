# ogpf - an object-based gnuplot wrap for fortran
# based on https://github.com/kookma/ogpf.git
# "ogpf is Object based interface to GnuPlot from Fortran 2003, 2008 and later"
#

cmake_minimum_required (VERSION 3.0)

# main project
project(ogpf)
enable_language(Fortran)

# release type
set(CMAKE_BUILD_TYPE Release)

# main source
add_subdirectory (src)

# tests
add_subdirectory (demo)