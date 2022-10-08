add_llvm_component_library(LLVMObfuscation
  CryptoUtils.cpp
  Substitution.cpp
  StringObfuscation.cpp
  BogusControlFlow.cpp
  Utils.cpp
  SplitBasicBlocks.cpp
  Flattening.cpp

  ADDITIONAL_HEADER_DIRS
  ${LLVM_MAIN_INCLUDE_DIR}/llvm/Transforms/Obfuscation

  DEPENDS
  intrinsics_gen
)