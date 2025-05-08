This project aims to speed up python by replacing native types with tables in an in-memory sqlite database.

This should improve speed by improving data locality and let the query planner make better decisions about data traversal.

```python
from py_record import record

@record
class ProgramArgs:
    args: list[str]

args = ProgramArgs(...)

args.select(...).filter(...)...
```

TODO:
 - [ ] parse class without annotations
 - [ ] create an `__init__` method
 - [ ] add data to our tables
 - [ ] query data from our tables
