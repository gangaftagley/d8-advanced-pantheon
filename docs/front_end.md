# Front End

## Theming Commands

To compile theme(s):
```
$ fin theme-compile
```
This will compile all themes in `src/themes`
To compile specific theme(s) use parameters to specify which themes to compile
```
$ fin theme-compile theme1 theme2
```
To compile for production (no map file and css compressed)
```
$ fin theme-compile -p
or
$ fin theme-compile -p theme1 theme2
```

To watch themes:
```
$ fin theme-watch
```
If there are multiple theme this command will watch the first theme in `src/themes`
To watch a specific theme:
```
$ fin watch-theme theme1
```
To create a bootstrap subtheme:
```
$ fin theme-bootstrap-subtheme
```
It will prompt for theme machine name and title.
This command is called from `fin init` so doesn't need to be called when creating a new site, but can be useful for creating multiple themes. The new theme will be automatically enabled.
