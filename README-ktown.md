Instructions to build QGIS 3.x on Slackware current with AlienBob's ktown.
Not all plugins will work due to missing Python 3 SlackBuilds for some modules.

Build packages in the following order:
```
freexl
geos
proj
postgresql
numpy3
pytz [PYTHON3=yes]
OWSLib
psycopg2
MarkupSafe [PYTHON3=yes]
python3-Jinja2
gdal [rebuild to ensure that it has Python 3 support; change to --with-poppler=no]
postgis
libspatialindex
libspatialite
qtkeychain [rebuild to ensure that it is built for Qt5]
qwt-qt5 [new]
qgis3 [new]
```
