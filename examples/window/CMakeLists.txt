
set(SRCROOT ${PROJECT_SOURCE_DIR}/examples/window)

# all source files
set(SRC ${SRCROOT}/Window.cpp)

# define the window target
sfml_add_example(window GUI_APP
                 SOURCES ${SRC}
                 DEPENDS SFML::Window)

# external dependency headers
target_include_directories(window SYSTEM PRIVATE ${PROJECT_SOURCE_DIR}/examples/window)
