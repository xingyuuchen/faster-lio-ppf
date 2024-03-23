add_library(${PROJECT_NAME}
        laser_mapping.cc
        pointcloud_preprocess.cc
        options.cc
        utils.cc
        )

add_dependencies(${PROJECT_NAME} ${PROJECT_NAME}_gencpp livox_ros_driver_gencpp)

target_compile_options(${PROJECT_NAME} PRIVATE ${OpenMP_CXX_FLAGS})
target_link_libraries(${PROJECT_NAME}
        ${catkin_LIBRARIES}
        ${PCL_LIBRARIES}
        ${PYTHON_LIBRARIES}
        tbb
        glog
        yaml-cpp
        ${OpenMP_CXX_FLAGS}
        )

target_include_directories(${PROJECT_NAME} PRIVATE ${PYTHON_INCLUDE_DIRS})
