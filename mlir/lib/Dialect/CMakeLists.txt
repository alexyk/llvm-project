add_subdirectory(AffineOps)
add_subdirectory(FxpMathOps)
add_subdirectory(GPU)
add_subdirectory(Linalg)
add_subdirectory(LLVMIR)
add_subdirectory(LoopOps)
add_subdirectory(OpenMP)
add_subdirectory(QuantOps)
add_subdirectory(SDBM)
add_subdirectory(Shape)
add_subdirectory(SPIRV)
add_subdirectory(StandardOps)
add_subdirectory(VectorOps)


set(LLVM_OPTIONAL_SOURCES
  Traits.cpp
)

add_llvm_library(MLIRDialect
  Traits.cpp

  ADDITIONAL_HEADER_DIRS
  ${MLIR_MAIN_INCLUDE_DIR}/mlir/Dialect

  LINK_LIBS
  MLIRIR
  LLVMSupport
  )
