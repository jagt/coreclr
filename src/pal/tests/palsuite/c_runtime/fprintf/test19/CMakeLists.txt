cmake_minimum_required(VERSION 2.8.12.2)

set(CMAKE_INCLUDE_CURRENT_DIR ON)

set(SOURCES
  test19.c
)

add_executable(paltest_fprintf_test19
  ${SOURCES}
)

add_dependencies(paltest_fprintf_test19 CoreClrPal)

target_link_libraries(paltest_fprintf_test19
  pthread
  rt
  m
  CoreClrPal
)
