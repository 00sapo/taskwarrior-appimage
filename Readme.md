Taskwarrior 3 AppImage to use it cross-distro.

This can be used on distro that are stuck to Taskwarrior 2.

It is based on Arch Linux, thanks to [ArchImage](https://github.com/ivan-hc/ArchImage) script.

An automatic workflow updates it every 36 hours, so it is always bringing latest security updates from Arch Linux and the latest version of Taskwarrior.

## Installation

Just download the AppImage from the release section. To keep it updated, rely on some third-party system. I recommend `mise`. The following are some examples of tools to manage Github releases.

[Mise](https://mise.jdx.dev/)
```toml
# in you mise config file, e.g. ~/.config/mise/config.toml
"github:00sapo/taskwarrior-appimage" = { version_prefix = "build-", version = "latest", bin = "task" }
```

[AM](https://github.com/ivan-hc/AM)
```bash
am -e https://github.com/00sapo/taskwarrior-appimage task
```
