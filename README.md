# PlantUML QEditor 2.x

Copyright (c) 2012 Ionutz Borcoman
Copyright (c) 2016 J. Albers

At a glance:
* simple PlantUML editor, with preview
* update the diagram while editing
* code assistant to insert ready-made code snipets
* written in Qt5, so it should run on all platforms supported by Qt5 and PlantUML
* license: GPLv3

PlantUML QEditor is a simple editor written in Qt5 for [PlantUML](http://plantuml.sourceforge.net/index.html).

Based on Ionutz Borcoman's great [PlantUML QEditor v1.x](http://sourceforge.net/projects/plantumlqeditor/).

Beside Qt5, you will need your own copy of PlantUML, java and graphviz/dot. The
path to java and plantuml are configurable via the Preferences dialog. Graphviz
should be installed so that plantuml can find it (there is no configuration
provided for this in Preferences).

The editor is quite simple: it monitors the editor for changes, and, if any,
runs plantuml to regenerate the image.

Plantuml is run using pipes, to simplify the interprocess communication.

If you want to save a specific image, export it via the File menu or using the
CTRL+E/CTRL+SHIFT+E shortcuts. The image is exported using the current selected
image format (SVG or PNG).

The editor also supports an assistant that allows easy insertion of code
snippets into the editor. The assistant is defined by a simple XML and a bunch
of icons, one for each snippet.
