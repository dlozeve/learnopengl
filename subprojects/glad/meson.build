project('glad', 'c')
i = include_directories('include')

cc = meson.get_compiler('c') 
dl_dep = cc.find_library('dl', required : false)

l = shared_library('glad', 'src/glad.c',
		   include_directories : i,
		   dependencies : [dl_dep],
		   install : true)

glad_dep = declare_dependency(include_directories : i,
			      link_with : l)
