set(SOURCES
    GLEScmImp.cpp
    GLEScmUtils.cpp
    GLEScmContext.cpp
    GLEScmValidate.cpp)

add_library(GLES_CM_translator SHARED ${SOURCES})
target_link_libraries(GLES_CM_translator GLcommon)

install(
  TARGETS GLES_CM_translator
  LIBRARY DESTINATION ${ANBOX_TRANSLATOR_INSTALL_DIR})
