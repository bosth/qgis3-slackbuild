Instructions to build QGIS 3.0.0 on Slackware 14.2. Not all plugins will work
due to missing Python 3 SlackBuilds for some modules.

Build instructions:
freexl
geos
proj
libinput
postgresql
python3
python3-sip
python3-six
numpy3
gdal [rebuild to ensure that it has Python 3 support]
postgis
libspatialindex
libspatialite
libxkbcommon
qt5
qt5-webkit
PyQt5 [only needed because QScintilla-qt5 is built with Python 2 and 3 support]
python3-PyQt5 [downgrade the current SlackBuild to version 5.7.1]
qtkeychain [rebuild to ensure that it is built for Qt5]
qwt-qt5 [new]
qca-qt5 [new]
QScintilla2-qt5 [new]
qgis3 [new]
