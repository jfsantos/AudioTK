
FILE(GLOB
  ATK_DISTORTION_TEST_SRC
  *.cpp
)

FILE(GLOB
  ATK_DISTORTION_TEST_HEADERS
  *.h*
)

SET(ATK_DISTORTION_TEST_DEFINITIONS)
SET(ATK_DISTORTION_TEST_INCLUDE)
SET(ATK_DISTORTION_TEST_LIBRARIES ATKDistortion ATKEQ ATKTools ATKMock ATKCore ${Boost_UNIT_TEST_FRAMEWORK_LIBRARY})

SET(ATK_DISTORTION_TEST_NAME ATKDistortion_test)
SET(ATK_DISTORTION_TEST_TESTNAME Distortion)
SET(ATK_DISTORTION_TEST_FOLDER Distortion_test)

ATK_add_test(ATK_DISTORTION_TEST)
