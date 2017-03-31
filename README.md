# Ansible Role: MimeApps

Edit Cinnamon 3.x.x MimeApps

## Requirements

Tested on Fedora with Cinnamon.

## Role Variables

```yml
mimeapps_user: root
```

```yml
default_associations:
  - { type: x-scheme-handler/http,    app: chromium-browser.desktop }
  - { type: x-scheme-handler/https,   app: chromium-browser.desktop }
  - { type: x-scheme-handler/about,   app: chromium-browser.desktop }
  - { type: x-scheme-handler/unknown, app: chromium-browser.desktop }
  - { type: application/xml,          app: atom.desktop             }
  - { type: image/svg+xml,            app: eog.desktop              }
  - { type: image/png,                app: eog.desktop              }
  - { type: image/jpeg,               app: eog.desktop              }
  - { type: image/vnd.microsoft.icon, app: eog.desktop              }
  - { type: text/html,                app: chromium-browser.desktop }
  - { type: text/plain,               app: atom.desktop             }
  - { type: text/markdown,            app: atom.desktop             }
  - { type: video/x-msvideo,          app: vlc.desktop              }
  - { type: video/quicktime,          app: vlc.desktop              }
  - { type: video/mpeg,               app: vlc.desktop              }
  - { type: video/mp4,                app: vlc.desktop              }
  - { type: audio/x-vorbis+ogg,       app: vlc.desktop              }
  - { type: audio/mpeg,               app: vlc.desktop              }
  - { type: audio/midi,               app: vlc.desktop              }
  - { type: audio/x-wav,              app: vlc.desktop              }
  - { type: audio/x-mpegurl,          app: vlc.desktop              }
```

```yml
added_associations:
  - { type: application/xml, app: atom.desktop;chromium-browser.desktop             }
  - { type: image/svg+xml,   app: atom.desktop;chromium-browser.desktop;eog.desktop }
```

## Dependencies

None

# License

MIT

# Author Information

Apostolos Tovletoglou [ansible-role-mimeapps](https://github.com/tovletoglou/ansible-role-mimeapps)
