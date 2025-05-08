This project aims to speed up python by replacing native types with tables in an in-memory sqlite database.

This should improve speed by improving data locality and let the query planner make better decisions about data traversal.
