
idf_component_register(
  SRCS
    src/bme68xLibrary.cpp
    src/bme68x/bme68x.c
  INCLUDE_DIRS
    src/bme68x
    src
  REQUIRES arduino)
