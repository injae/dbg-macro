cmake_minimum_required(VERSION 3.6)

include(cmake/cppm_tool.cmake)
cppm_project()
include(HunterGate)
HunterGate(
   URL "https://github.com/ruslo/hunter/archive/v0.23.214.tar.gz"
   SHA1 "e14bc153a7f16d6a5eeec845fb0283c8fad8c358"
)
project(dbg-macro VERSION 0.0.1 LANGUAGES C CXX)
cppm_setting()

cppm_cxx_standard(17)
cppm_compiler_option(DEFAULT)



cppm_target_define(dbg-macro INTERFACE )


cppm_target_dependencies(dbg-macro 
)

cppm_target_install(dbg-macro)

