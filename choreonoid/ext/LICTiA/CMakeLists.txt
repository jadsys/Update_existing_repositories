if(NOT ENABLE_GUI)
  return()
endif()

option(BUILD_LICTIA "Building the LICTIA files" ON)
if(NOT BUILD_LICTIA)
  return()
endif()

add_subdirectory(controller)

if(UNIX)
  add_custom_target(
    symlink_to_LICTiA ALL
    COMMAND ${CMAKE_COMMAND} -E create_symlink
    ${CMAKE_CURRENT_SOURCE_DIR} ${CNOID_BINARY_SHARE_DIR}/LICTiA)
endif()

install(DIRECTORY
  model
  DESTINATION ${CNOID_SHARE_SUBDIR}/LICTiA)

