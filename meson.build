project('ding',
  version: '47',
  license: 'GPL3'
)

gnome = import ('gnome')
i18n = import('i18n')

prefix = get_option('prefix')
datadir = join_paths (prefix, get_option('datadir'))
schema_dir = join_paths(datadir, 'glib-2.0', 'schemas')

extensions_dir = join_paths(prefix, 'share', 'gnome-shell', 'extensions', 'ding@rastersoft.com')

install_data([
    'autoAr.js',
    'askRenamePopup.js',
    'createThumbnail.js',
    'dbusInterfaces.js',
    'dbusUtils.js',
    'desktopGrid.js',
    'desktopIconItem.js',
    'desktopIconsUtil.js',
    'desktopManager.js',
    'ding.js',
    'emulateX11WindowType.js',
    'enums.js',
    'extension.js',
    'fileItem.js',
    'fileItemMenu.js',
    'fileUtils.js',
    'gnomeShellOverride.js',
    'metadata.json',
    'notifyX11UnderWayland.js',
    'prefs.js',
    'preferences.js',
    'prefswindow.js',
    'promiseUtils.js',
    'stackItem.js',
    'showErrorPopup.js',
    'stylesheet.css',
    'templatesScriptsManager.js',
    'thumbnails.js',
    'visibleArea.js'
  ],
  install_dir: extensions_dir
)

subdir(
  'po'
)
subdir(
  'schemas'
)

meson.add_install_script('meson_post_install.py')
