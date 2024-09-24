```sql
create table products (pro_id int(3), pro_name varchar(50), pro_price float, pro_code int (2));
```

```sql
insert into products values (101, "Mother Board", 3200.00, 15);
insert into products values (102, "Key Board", 450.00, 16);
insert into products values (103, "Zip Drive", 250.00, 14);
insert into products values (104, "Speaker", 550.00, 16);
insert into products values (105, "Monitor", 5000.00, 11);
insert into products values (106, "DVD Drive", 900.00, 12);
insert into products values (107, "CD Drive", 800.00, 12);
insert into products values (108, "Printer", 2600.00, 13);
insert into products values (109, "Refill Cartridge", 350.00, 13);
insert into products values (110, "Mouse", 250.00, 12);
```

```sql
select pro_name , pro_price from products where pro_price>=250.00 order by pro_name asc, pro_price desc;
```


```sql
select pro_name, pro_price from products order by pro_price asc limit 2;
```


```sql
select avg(pro_price) as Average_Price from products;  
```


```sql
select sum(pro_price) as Total_Price from products;
```