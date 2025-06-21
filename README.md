# draw.io

Provides packaging for the [draw.io](https://www.draw.io) diagramming library. The generated packages are used by the [Diagram Application](https://github.com/xwiki-contrib/application-diagram/).

Recent versions of the upstream [draw.io](https://github.com/jgraph/drawio) repository moved the editor sources from `js/grapheditor` to `src/main/webapp/js`. The WebJar build from this packaging project already bundles the required editor files, so you don't need to fetch them from the old location. To build the WebJar use this packaging project (forked at [seclution/draw.io](https://github.com/seclution/draw.io)):

```bash
mvn clean install
```

The produced WebJar can then be used by the XWiki Diagram Application.

* Project Lead: [Marius Dumitru Florea](http://www.xwiki.org/xwiki/bin/view/XWiki/mflorea)
* License: **Apache 2.0** license. Note that the packaged code (the draw.io library developed by JGraph Ltd) and some classes we modified (also developed by JGraph Ltd)  are licensed under Apache 2.0.
* Continuous Integration Status: [![Build Status](http://ci.xwiki.org/job/XWiki%20Contrib/job/draw.io/job/master/badge/icon)](http://ci.xwiki.org/view/Contrib/job/XWiki%20Contrib/job/draw.io/job/master/)
