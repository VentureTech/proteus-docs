# Proteus Documents

Content in the gh-pages branch is public through GitHub Pages.  Pages are processed using Jekyll, with Redcarpet as the markdown engine.
Each markdown `.md` file must contain the "front matter":
```
---
title: Some title
layout: A file from the _layouts directory, e.g. default or guide
---
```

## Directory structure
 * The highest level directory is a number indicating the major release of Proteus.  Each version directory contains:
   * `changes.md` Change log for the release (developer-oriented)
   * `features.md` Notable features added or major interface changes for the release
   * `guides/` Developer guides in markdown
   * `api/` Javadoc reference
