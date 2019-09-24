cmake_minimum_required(VERSION 3.6)

add_compile_options("-O3")

add_executable(osmupdate osmupdate.c)
add_executable(osmfilter osmfilter.c)
add_executable(osmconvert osmconvert.c)

target_link_libraries(
  osmconvert
  z
)
