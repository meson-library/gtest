
include      = include_directories('include', '.', is_system : true)
lib_sources  = files('src/gtest-all.cc')
main_sources = files('src/gtest_main.cc')

gtest_dep = declare_dependency(include_directories : include,
	                           sources             : lib_sources,
	                           dependencies        : dependency('threads'))

gtest_main_dep = declare_dependency(include_directories : include,
	                                sources             : [lib_sources, main_sources],
	                                dependencies        : dependency('threads'))
