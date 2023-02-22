
project('budgie-analog-clock-widget',
        ['vala', 'c'],
        version: '0.1.0',
        meson_version: '>=0.40.0',
        license: 'GPL3')

widget_id = 'com.github.samlane-ma.budgie-analog-clock-widget'

# Global path variable
prefix = get_option('prefix')
libdir = join_paths(prefix, get_option('libdir'))
datadir = join_paths(prefix, get_option('datadir'))

PIXMAPS_DIR = join_paths(datadir, 'pixmaps')
LIB_INSTALL_DIR = join_paths(prefix, libdir, 'budgie-desktop', 'raven-plugins', widget_id)
SCHEMADIR = join_paths(prefix, 'share', 'glib-2.0', 'schemas')

install_data('schema/com.github.samlane-ma.budgie-analog-clock-widget.gschema.xml',
    install_dir: SCHEMADIR,
)

subdir('src')
subdir('icons')

message('Installing applet...')
meson.add_install_script('meson_post_install')
