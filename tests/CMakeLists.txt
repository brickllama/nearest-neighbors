find_package(GTest REQUIRED)

add_executable(nearest-neighbors-tests
    point_tests.cpp
)

target_link_libraries(nearest-neighbors-tests
    PRIVATE
        GTest::gtest_main
)
