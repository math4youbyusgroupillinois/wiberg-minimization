add_library(Factorization factor_simultaneous.cc factor_wiberg.cc observation_to_row_map.cc solve_V.cc solve_V_j.cc)

add_executable(factor_wiberg_test factor_wiberg_test.cc)
target_link_libraries(factor_wiberg_test Factorization LinearSystem MatrixUtility Clp CoinUtils)

add_executable(factor_simultaneous_test factor_simultaneous_test.cc)
target_link_libraries(factor_simultaneous_test Factorization LinearSystem MatrixUtility Clp CoinUtils)