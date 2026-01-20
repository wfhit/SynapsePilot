px4_add_module(
    MODULE modules__articulated_chassis__traction_controller
    MAIN traction_controller
    SRCS
        traction_controller.cpp
        traction_controller.hpp
        traction_controller_main.cpp
    MODULE_CONFIG
        module.yaml
    DEPENDS
        px4_work_queue
        PID
        mathlib
        perf
)
