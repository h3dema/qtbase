# Generated from broadcastsender.pro.

cmake_minimum_required(VERSION 3.14)
project(broadcastsender LANGUAGES CXX)

set(CMAKE_INCLUDE_CURRENT_DIR ON)

set(CMAKE_AUTOMOC ON)
set(CMAKE_AUTORCC ON)
set(CMAKE_AUTOUIC ON)

set(INSTALL_EXAMPLEDIR "examples/network/broadcastsender")

find_package(Qt6 COMPONENTS Core)
find_package(Qt6 COMPONENTS Gui)
find_package(Qt6 COMPONENTS Network)
find_package(Qt6 COMPONENTS Widgets)

add_qt_gui_executable(broadcastsender
    main.cpp
    sender.cpp sender.h
)
target_link_libraries(broadcastsender PUBLIC
    Qt::Core
    Qt::Gui
    Qt::Network
    Qt::Widgets
)

install(TARGETS broadcastsender
    RUNTIME DESTINATION "${INSTALL_EXAMPLEDIR}"
    BUNDLE DESTINATION "${INSTALL_EXAMPLEDIR}"
    LIBRARY DESTINATION "${INSTALL_EXAMPLEDIR}"
)
