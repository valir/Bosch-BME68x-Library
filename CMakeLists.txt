if(CONFIG_USE_SENSOR_BME680)
  set(BME68X_SRCS
    src/bme68xLibrary.cpp
    src/bme68x/bme68x.c)
endif()

idf_component_register(
  SRCS
    ${BME68X_SRCS}
  INCLUDE_DIRS
    src/bme68x
    src
  REQUIRES arduino)
