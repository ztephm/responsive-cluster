## Create indexes
```sql
create index index_name on table_name(column_name);
```

## Create clusters
```sql
cluster index_name on table_name
```

## Reduce categories
```sql
update table_name
   set column_name = `other`
 where column_name not in ('category1','category2')
 ```

## Subsample and order
```sql
-- use a smaller sample of original dataset
-- order by numbers assigned to categories when normal ORDER BY ASC or DESC doesn't give the order you need
select t.* 
     from table_name t tablesample system(20)
left join (
            values 
              ('category2',1),('other',2),
              ('category1',3)
            ) as c(categories,ordering)
       on t.category_column_name = c.categories
 order by c.ordering
```