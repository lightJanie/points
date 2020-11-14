## mysql

```python
1.delete操作失败，需要修改变量
show variables like 'sql_safa_updates';
set sql_safe_updates=1;
```

## python

```python
1.list转str
  如果list中元素为数字，不能直接转str，需要map操作。
  ','.join(map(str,li))

2.字典列表按照某个键的值进行排序
 rows=[{'frame':'Brian','lname':'Jones','uid':1003},...]
 from operator import itemgetter
 rows_by_frame=sorted(rows,key=itemgetter('fname'))
```

## Django

```python
1. 	queryset.values(a).annotate(b=sum(num))  
    a为group by字段，b为聚合字段，最后显示a和b字段。
    
2.select_related()
作用：在对QuerySet使用select_related()函数后，Django会获取相应外键对应的对象，从而在之后需要的时候不必再查询数据库了。
```

