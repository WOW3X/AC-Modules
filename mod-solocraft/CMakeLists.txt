CU_SET_PATH("CMAKE_MOD_SOLOCRAFT_DIR" "${CMAKE_CURRENT_LIST_DIR}")

AC_ADD_SCRIPT("${CMAKE_CURRENT_LIST_DIR}/src/mod_solocraft.cpp")

AC_ADD_SCRIPT_LOADER("Solocraft" "${CMAKE_CURRENT_LIST_DIR}/src/loader_solocraft.h")

CU_ADD_HOOK(AFTER_WORLDSERVER_CMAKE "${CMAKE_CURRENT_LIST_DIR}/src/cmake/after_ws_install.cmake")