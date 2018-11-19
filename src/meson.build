simpletexteditor_sources = [
  'main.cpp',
  'simpletexteditor-window.cpp',
]

simpletexteditor_deps = [
  dependency('gtkmm-3.0', version: '>= 3.18'),
]

gnome = import('gnome')

simpletexteditor_sources += gnome.compile_resources('simpletexteditor-resources',
  'simpletexteditor.gresource.xml',
  c_name: 'simpletexteditor'
)

executable('simpletexteditor', simpletexteditor_sources,
  dependencies: simpletexteditor_deps,
  install: true,
)
