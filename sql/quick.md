#### 查看数据库表大小
```sql
select * from INFORMATION_SCHEMA.INNODB_SYS_TABLESPACES order by ALLOCATED_SIZE desc;
```
