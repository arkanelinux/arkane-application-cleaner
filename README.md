# arkane-application-cleaner

Hide unwanted .desktop files.

## Details

The application-cleaner is a script which runs using a pacman hook whenever a new application is installed adding a .desktop file. It will loop over a list of provided configuration files and append the content of each config to the matching .desktop file.

You can find a pkgbuild file [here](https://github.com/arkanelinux/pkgbuild/blob/main/arkane-application-cleaner/PKGBUILD).

## Configure

Add config files with the below content to `/etc/arkane/application-cleaner/`. The filename should match the name of the .destkop file in `/usr/share/applications`.

```bash
contain='NotShowIn=GNOME;KDE;Pantheon;'
```
