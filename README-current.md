Instructions to build QGIS 3.0.0 on Slackware current. Not all plugins will work
due to missing Python 3 SlackBuilds for some modules.

Build packages in the following order:
```
freexl
geos
proj
libinput
postgresql
numpy3
pytz [PYTHON3=yes]
OWSLib
psycopg2
MarkupSafe [PYTHON3=yes]
python3-Jinja2
gdal [rebuild to ensure that it has Python 3 support]
postgis
libspatialindex
libspatialite
libxkbcommon
qt5
qt5-webkit
python3-PyQt5 [match qt5 version; if using alien's PyQt5 package, you should already have all the Python 3 files, so you won't need this, but you will need to rebuild PyQt5 using this change https://git.slackware.nl/ktown/commit/?id=338b3b02b7bb7e3f8bde1645c694c2b6c6d42b11]
qtkeychain [rebuild to ensure that it is built for Qt5]
qwt-qt5 [new]
qca-qt5 [new]
QScintilla-qt5 [new; change python3-sip to sip3 in SlackBuild]
qgis3 [new; change python3-sip to sip3 in SlackBuild]
```
