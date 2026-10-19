if (NOT TARGET mcu-math)

    add_library(mcu-math INTERFACE)

    target_include_directories(mcu-math INTERFACE
        include
    )

    target_include_directories(mcu-math INTERFACE
        $<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}/src> 
    )

endif()