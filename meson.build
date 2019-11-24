project('learnopengl', 'cpp')

glfw = dependency('glfw3')

glad_sp = subproject('glad')
glad = glad_sp.get_variable('glad_dep')

executable('learnopengl', 'src/main.cpp',
	   dependencies : [glfw, glad])
