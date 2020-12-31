cmake_minimum_required(VERSION 3.10.2 FATAL_ERROR)

#============================================================================
# Initialize the project
#============================================================================
project(ignition-blueprint VERSION 1.1.0)

#============================================================================
# Find ignition-cmake
#============================================================================
# If you get an error at this line, you need to install ignition-cmake
find_package(ignition-cmake2 2.6.2 REQUIRED)

#============================================================================
# Configure the project
#============================================================================
ign_configure_project()

# all list of blueprint packages

ign_find_package(ignition-common3 REQUIRED VERSION 3.9.0)
ign_find_package(ignition-fuel_tools3 REQUIRED VERSION 3.5.0)
ign_find_package(ignition-gazebo2 REQUIRED VERSION 2.26.0)
ign_find_package(ignition-gui2 REQUIRED VERSION 2.3.3)
ign_find_package(ignition-launch1 REQUIRED VERSION 1.10.1)
ign_find_package(ignition-math6 REQUIRED VERSION 6.7.0)
ign_find_package(ignition-msgs4 REQUIRED VERSION 4.9.0)
ign_find_package(ignition-plugin1 REQUIRED VERSION 1.1.0)
ign_find_package(ignition-physics1 REQUIRED VERSION 1.10.0)
ign_find_package(ignition-sensors2 REQUIRED VERSION 2.9.1)
ign_find_package(ignition-tools REQUIRED)
ign_find_package(ignition-transport7 REQUIRED VERSION 7.5.1)
ign_find_package(sdformat8 REQUIRED VERSION 8.9.1)


install(DIRECTORY gazebodistro DESTINATION ${IGN_DATA_INSTALL_DIR})
