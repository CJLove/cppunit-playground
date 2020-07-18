cmake_minimum_required(VERSION 3.12.0 )

project(basicMathTest)

include_directories ( ../src 
                      ${CPPUNIT_INCLUDE_DIR}
                    )

add_executable(basicMathTest basicMathTest.cpp )

target_link_libraries(basicMathTest basicMath ${CPPUNIT_LIBRARY} )

add_test(basicMathTest basicMathTest)