include_directories(
  ${CMAKE_SOURCE_DIR}/lib/Target/PowerPC
  ${CMAKE_BINARY_DIR}/lib/Target/PowerPC
  )

set(LLVM_LINK_COMPONENTS
  Support
  Target
  PowerPCCodeGen
  )

add_llvm_unittest(PowerPCTests
  AIXRelocModelTest.cpp
  )
