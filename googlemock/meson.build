
include      = include_directories('include', '.', is_system : true)
lib_sources  = files('src/gmock-all.cc')
main_sources = files('src/gmock_main.cc')

gmock_dep = declare_dependency(include_directories : [include],
	                           sources             : [lib_sources],
	                           dependencies        : [gtest_dep, dependency('threads')])

gmock_main_dep = declare_dependency(include_directories : [include],
                                    sources             : [lib_sources, main_sources],
                                    dependencies        : [gtest_dep, dependency('threads')])
