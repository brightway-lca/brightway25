Brightway2.5
============

Brightway 2.5 is the next generation of the [Brightway2](https://brightway.dev/) framework for life cycle assessment. It provides new capabilities for cloud computing and model interaction, with the use of a new [processed data library](https://github.com/brightway-lca/bw_processing) and a separation between the calculation library and a library for [matrix construction and manipulation](https://github.com/brightway-lca/matrix_utils).

Note that this library does not import anything, so running `from brightway25 import *` won't do anything useful. Instead, import each constituent library separately. A good default is:

```python

import bw2analyzer as ba
import bw2data as bd
import bw2calc as bc
import bw2io as bi
import matrix_utils as mu
import bw_processing as bp

```

# Upgrading

Brightway 2.5 can be use in parallel with Brightway 2, but each project must be either version 2 or 2.5. Brightway 2.5 projects have a different processed data format, and no longer use the `mapping` object.

To upgrade an existing project to version 2.5, use the function `bw2data.projects.migrate_project_25()`.

To maintain a clean separation between these two sets of projects, you can use some type of naming convention, or use an [environment variable](https://2.docs.brightway.dev/faq.html?#how-do-i-find-where-my-data-is-saved) for a new data directory.


Official site:

* https://brightway.dev

Online documentation:

* https://25.docs.brightway.dev/

Development blog:

* http://chris.mutel.org
