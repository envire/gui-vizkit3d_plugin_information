cmake_minimum_required(VERSION 3.1)
project(vizkit3d_plugin_information VERSION 0.1
    DESCRIPTION "Library to enumerate and load vizkit3d plugins based on supported type")

find_package(Rock)

rock_init()
rock_feature(NOCURDIR)
rock_standard_layout()
