# History and accesslog

History of changes is logging all changes and actions caused by user. 

## Database
_fjord_history_
- PK id
- FK user_id
- VFK table
- VFK row_id
- changes (JSON)
- time DATETIME

### Changes JSON structure
```
{
    "changed_columns": ["col1", "val1"],
    "data": {
        "col1": "val1",
        "col2": "val2",
    }
}
```