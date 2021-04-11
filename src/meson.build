gtkinventoryproject_sources = [
  'main.cpp',
  'gtkinventoryproject-window.cpp',
]

gtkinventoryproject_deps = [
  dependency('gtkmm-3.0', version: '>= 3.18'),
]

gnome = import('gnome')

gtkinventoryproject_sources += gnome.compile_resources('gtkinventoryproject-resources',
  'gtkinventoryproject.gresource.xml',
  c_name: 'gtkinventoryproject'
)

executable('gtkinventoryproject', gtkinventoryproject_sources,
  dependencies: gtkinventoryproject_deps,
  install: true,
)
