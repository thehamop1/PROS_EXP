set(MATABOTS_SRCS
    main.cpp
)


add_executable(MATABOTS ${MATABOTS_SRCS})


include_directories(MATABOTS ${CMAKE_SOURCE_DIR}/include)
target_link_libraries(MATABOTS ${PROS_LIB})