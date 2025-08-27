add_definitions(-DBASE_LOG_NAMESPACE=${PROJECT_NAME})

rock_find_qt4(OPTIONAL)
rock_find_qt5(OPTIONAL)

include(RockQt)

rock_qt_library(
                TARGETPREFIX vizkit3d_plugin_information
                QT4_SUFFIX ""
                HEADERS Vizkit3dPluginInformation.hpp
                SOURCES Vizkit3dPluginInformation.cpp
                DEPS_PKGCONFIG base-lib
                DEPS_PKGCONFIG_QT vizkit3d
                LIBS_QT4 Qt4::QtCore
                LIBS_QT5 Qt5::Core)

