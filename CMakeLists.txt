add_executable(Person
  main.c)

target_include_directories(Person
  PUBLIC ${PROJECT_BINARY_DIR}
         ${PROJECT_SOURCE_DIR}
         ${CMAKE_CURRENT_SOURCE_DIR})

set_target_properties(Person PROPERTIES
  FOLDER "${PROJECT_NAME}/Person"
  OUTPUT_NAME ${PROJECT_NAME}-Person
  PROJECT_LABEL "Person")
