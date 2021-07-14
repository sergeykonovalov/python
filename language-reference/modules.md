# Modules

When trying to import modules, Python looks into several paths:

- directories listed in sys.path
- sys modules (baked into Python) , code in .py not available

To add new path: `sys.path.insert(0, new_path)`.

Once imported, all module functions and variables are available.

```python
import random  # single package
import os, sys  # several packages at once
from package_name import *  # import specific class or function
# ^^^ not recommended, as names might overlap
```
