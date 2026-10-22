cmake_minimum_required(VERSION 3.21)

project(HungarianVocabulary VERSION 0.1.0 LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)

find_package(Qt6 6.5 REQUIRED COMPONENTS Widgets)
qt_standard_project_setup()

qt_add_executable(HungarianVocabulary MACOSX_BUNDLE
    src/main.cpp
)

set_target_properties(HungarianVocabulary PROPERTIES
    MACOSX_BUNDLE_BUNDLE_NAME "Hungarian Vocabulary"
    MACOSX_BUNDLE_BUNDLE_VERSION ${PROJECT_VERSION}
    MACOSX_BUNDLE_SHORT_VERSION_STRING ${PROJECT_VERSION}
)

target_link_libraries(HungarianVocabulary PRIVATE Qt6::Widgets)
