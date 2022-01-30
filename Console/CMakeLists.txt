cmake_minimum_required(VERSION 3.10)
set (project "Console")
project(${project} CXX)
my_find_src_files (src_files ${project})
add_executable (${project} ${src_files})

my_inc_import_RisLib(${project})
my_inc_import_CommonLib(${project})

my_lib_import_CommonLib(${project})
my_lib_import_RisLib(${project})

install(TARGETS ${project} DESTINATION "C:/aaa_prime/UCon")
return()
