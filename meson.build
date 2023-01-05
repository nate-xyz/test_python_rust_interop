project('test_python_rust_interop', 'rust', 
          version: '0.1.0',
    meson_version: '>= 0.59.0',
  default_options: [ 'warning_level=3', 'werror=false', ],
)

i18n = import('i18n')
gnome = import('gnome')

subdir('data')
subdir('src')
subdir('po')

gnome.post_install(
     glib_compile_schemas: true,
    gtk_update_icon_cache: true,
  update_desktop_database: true,
)
