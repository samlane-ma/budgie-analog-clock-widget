RavenAnalogClockSources = ['ravenanalogclock.vala', 'ravenclockimage.vala', 'clocksettings.vala', 'dropdown.vala']

RavenAnalogClockDependencies = [
    dependency('gtk+-3.0', version: '>=3.18'),
    dependency('libpeas-gtk-1.0'),
    dependency('budgie-raven-plugin-1.0'),
    meson.get_compiler('c').find_library('m', required: false)
]

install_data('RavenAnalogClock.plugin', install_dir: LIB_INSTALL_DIR)

shared_library(widget_id, RavenAnalogClockSources, dependencies: RavenAnalogClockDependencies, install: true, install_dir: LIB_INSTALL_DIR)
