include_directories(.)

add_executable(
  pghr13

  pghr13.cpp
)
target_link_libraries(
  pghr13

  snark
)
target_include_directories(
  pghr13

  PUBLIC
  ${DEPENDS_DIR}/libsnark
  ${DEPENDS_DIR}/libsnark/depends/libfqfft
)

include_directories(.)

add_executable(
  range

  range.cpp
)
target_link_libraries(
  range

  snark
)
target_include_directories(
  range

  PUBLIC
  ${DEPENDS_DIR}/libsnark
  ${DEPENDS_DIR}/libsnark/depends/libfqfft
)

include_directories(.)

add_executable(
  groth16

  groth16.cpp
)
target_link_libraries(
  groth16

  snark
)
target_include_directories(
  groth16

  PUBLIC
  ${DEPENDS_DIR}/libsnark
  ${DEPENDS_DIR}/libsnark/depends/libfqfft
)
