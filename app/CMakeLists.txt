add_executable(run_mapping_online run_mapping_online.cc)
target_compile_options(run_mapping_online PRIVATE ${OpenMP_CXX_FLAGS})
target_link_libraries(run_mapping_online
        ${PROJECT_NAME} gflags
        ${OpenMP_CXX_FLAGS}
        )
add_executable(run_mapping_offline run_mapping_offline.cc)
target_compile_options(run_mapping_offline PRIVATE ${OpenMP_CXX_FLAGS})
target_link_libraries(run_mapping_offline
        ${PROJECT_NAME} gflags
        ${OpenMP_CXX_FLAGS}
        )
