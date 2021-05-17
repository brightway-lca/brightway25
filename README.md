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

Official site:

* https://brightway.dev

Online documentation:

* https://25.docs.brightway.dev/

Development blog:

* http://chris.mutel.org
