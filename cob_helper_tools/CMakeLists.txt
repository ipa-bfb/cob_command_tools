cmake_minimum_required(VERSION 2.8.3)
project(cob_helper_tools)

find_package(catkin REQUIRED)

catkin_package()

#############
## Install ##
#############

install(PROGRAMS
  scripts/auto_init.py
  scripts/auto_recover.py
  scripts/fake_diagnostics.py
  scripts/fake_driver.py
  DESTINATION ${CATKIN_PACKAGE_BIN_DESTINATION}
)
