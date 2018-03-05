Instructions to build QGIS 3.0.0 on Slackware 14.2. Not all plugins will work
due to missing Python 3 SlackBuilds for some modules.

Build packages in the following order:
```
freexl
geos
proj
libinput
postgresql
python3
python3-sip
python3-six
python3-PyYAML
numpy3
gdal [rebuild to ensure that it has Python 3 support]
postgis
libspatialindex
libspatialite
libxkbcommon
qt5
qt5-webkit
python3-PyQt5 [downgrade the current SlackBuild to version 5.7.1]
qtkeychain [rebuild to ensure that it is built for Qt5]
qwt-qt5 [new]
qca-qt5 [new]
QScintilla-qt5 [new]
qgis3 [new]
```
