add_llvm_library(MLIRTranslation
  Translation.cpp

  ADDITIONAL_HEADER_DIRS
  ${MLIR_MAIN_INCLUDE_DIR}/mlir/Translation

  LINK_LIBS
  LLVMSupport
)
