# draw.io

Provides packaging for the [draw.io](https://www.draw.io) diagramming library. The generated packages are used by the [Diagram Application](https://github.com/xwiki-contrib/application-diagram/).

* Project Lead: [Marius Dumitru Florea](http://www.xwiki.org/xwiki/bin/view/XWiki/mflorea)
* License: **Apache 2.0** license. Note that the packaged code (the draw.io library developed by JGraph Ltd) and some classes we modified (also developed by JGraph Ltd)  are licensed under Apache 2.0.
* Continuous Integration Status: [![Build Status](http://ci.xwiki.org/job/XWiki%20Contrib/job/draw.io/job/master/badge/icon)](http://ci.xwiki.org/view/Contrib/job/XWiki%20Contrib/job/draw.io/job/master/)

## GitHub Workflows

This repository uses several GitHub Actions for automation:

* **release.yml** builds and uploads the packaged artifacts when a release is published.
* **sync-drawio-sources.yml** regularly pulls the upstream sources from [jgraph/drawio](https://github.com/jgraph/drawio) and opens a pull request with the updates.
* **sync-package-builder.yml** keeps the packaging helper scripts in sync with [seclution/draw.io](https://github.com/seclution/draw.io).

Both sync workflows run weekly and can also be triggered manually through the GitHub interface.
