project(lib_psf_project)

include_directories ("${PROJECT_SOURCE_DIR}/src")
include_directories ("${PROJECT_SOURCE_DIR}/..")
add_library(psf SHARED psf.c)

install(TARGETS psf DESTINATION lib)
install(FILES psf.h DESTINATION include)

