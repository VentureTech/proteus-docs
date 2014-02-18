# Proteus Documents

Content in the gh-pages branch is [public] (http://docs.proteusframework.com) through GitHub Pages.  Pages are processed using Jekyll, with Redcarpet as the markdown engine.  For debugging or testing you might want to [install and run Jekyll locally] (https://help.github.com/articles/using-jekyll-with-pages#installing-jekyll).


Each markdown `.md` file must contain the "front matter":
```
---
title: Some title
layout: A file from the _layouts directory, e.g. default or guide
---
```

**Files that do not contain the above "front matter" are passed through to the site unchanged.** For example, if you include an HTML file without the section above, it will appear on the site without going through the template engine.

## Directory structure
 * `version/` Contains a subdirectory named with a number, indicating the major release of Proteus, e.g.,
`version/0/`. Each version directory contains:
   * `changes.md` Change log for the release
   * `guides/` Developer guides in markdown
   * `api/` Javadoc reference
 * Other contents in the root directory:
   * `index.md` Home page
   * `CNAME` Tells GitHub Pages to use a special (sub)domain name
   * `Gemfile` Helps with running Jekyll locally
   * `_config.yml` Global Jekyll config file
   * `_layouts/` Jekyll templates for the documentation
   * `style/` Stylesheets for layouts
