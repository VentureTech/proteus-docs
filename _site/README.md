Content in the gh-pages branch is public through GitHub Pages.
 * The master branch is empty and should be ignored
 * The gh-pages branch contains source (e.g. DocBook XML) in the "_docbook" directories (where the underscore causes GitHub Pages / Jekyll to ignore them), plus published documents, e.g. HTML

Directory structure:
 * The highest level directory is a number indicating the major release of Proteus.  The version directory contains:
   * _docbook: source files for DocBook (not published)
   * guides: DocBook developer guides published as HTML
   * api: Javadoc reference
