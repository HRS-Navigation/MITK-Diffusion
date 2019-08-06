mitk_create_module(
  SUBPROJECTS MITK-Diffusion
  INCLUDE_DIRS ${CMAKE_CURRENT_BINARY_DIR} ReaderWriter ObjectFactories
  DEPENDS MitkConnectomics MitkDiffusionCore MitkSceneSerialization
  AUTOLOAD_WITH MitkCore
  PACKAGE_DEPENDS
    PUBLIC DCMTK
    PRIVATE tinyxml
)

