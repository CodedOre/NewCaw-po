project(
  'Cawbird-po',
  version:        '1.9.0',
  meson_version:  '>= 0.56.0',
)

# Fail if not a subproject of Cawbird
if not meson.is_subproject()
    message('WARNING: This project is only intended to be used as a subproject!')
endif

# Load meson modules
i18n  = import('i18n')

# Translate the project
i18n.gettext(
  'Cawbird',
  preset: 'glib',
  args: [
    '--from-code=UTF-8',
    '--add-comments=TRANSLATORS',
    '--package-name=' + meson.project_name(),
    '--package-version=' + meson.project_version(),
    '--msgid-bugs-address=https://github.com/ibboard/cawbird/issues/new',
    '--copyright-holder=2021 Frederick Schenk'
  ]
)
