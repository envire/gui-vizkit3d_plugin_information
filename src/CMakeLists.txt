add_definitions(-DBASE_LOG_NAMESPACE=${PROJECT_NAME})
rock_library(vizkit3d_plugin_information
             HEADERS Vizkit3dPluginInformation.hpp
             SOURCES Vizkit3dPluginInformation.cpp
             DEPS_PKGCONFIG vizkit3d base-lib QtCore)    
