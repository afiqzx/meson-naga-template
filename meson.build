project('server', 'cpp')

cmake = import('cmake')

option_var = cmake.subproject_options()
option_var.add_cmake_defines({'BUILD_CTL': false})

drogon_proj = cmake.subproject('drogon', options: option_var)
drogon = drogon_proj.dependency('drogon')

trantor_proj = cmake.subproject('trantor')
trantor = trantor_proj.dependency('trantor')

executable('server', 'server/main.cpp', dependencies: [drogon, trantor])
