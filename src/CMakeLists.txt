add_definitions(-DBASE_LOG_NAMESPACE=${PROJECT_NAME})

rock_find_qt4()
rock_find_qt5()

if(ROCK_QT_VERSION_4)
    rock_library(vizkit3d_plugin_information
                 HEADERS Vizkit3dPluginInformation.hpp
                 SOURCES Vizkit3dPluginInformation.cpp
                 DEPS_PKGCONFIG vizkit3d base-lib
                 LIBS Qt4::QtCore)
endif(ROCK_QT_VERSION_4)

if(ROCK_QT_VERSION_5)
    rock_library(vizkit3d_plugin_information-qt5
                 HEADERS Vizkit3dPluginInformation.hpp
                 SOURCES Vizkit3dPluginInformation.cpp
                 DEPS_PKGCONFIG vizkit3d-qt5 base-lib
                 LIBS Qt5::Core)
endif(ROCK_QT_VERSION_5)
