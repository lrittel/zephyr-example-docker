configure_file(version.h.in version.h @ONLY)

target_include_directories(app PRIVATE ${CMAKE_CURRENT_SOURCE_DIR})
target_include_directories(app PRIVATE ${CMAKE_CURRENT_BINARY_DIR})

target_sources(app PRIVATE
  main.c
)
