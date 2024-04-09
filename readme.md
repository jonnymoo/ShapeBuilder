# ShapeBuilder

This HTML page provides a tool to create shapes compatible with the PythonCalcs repository. By defining your data structure within the page, you can generate the necessary shape information for use in your Python calculations.

## How to Use

Open `index.html` in your web browser.

## SQL required to build table / column shapes

```sql
select lower(Table_name) as table_name, lower(COLUMN_NAME) as column_name
from INFORMATION_SCHEMA.COLUMNS
where TABLE_NAME like 'UPM%'
FOR JSON AUTO
```

Modify the `column` variable at the bottom of index.html 
