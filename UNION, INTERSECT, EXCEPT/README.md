### Merhabalar, **dvdrental** örnek veri tabanını kullanarak UNION, INTERSECT, EXCEPT ile ilgili 3 adet örnek çalışma yapacağız. 
**Dvdrental** örnek verı tabanını **SQL-examples** dosyaları arasına ekledım, oradan elde ede bilirsiniz. Ve ya [Buradan](https://www.postgresqltutorial.com/postgresql-getting-started/postgresql-sample-database/) Internet aracılığıyla kendiniz indire bilirsiniz.
## TASK 1 
Actor ve customer tablolarında bulunan first_name sütunları için tüm verileri sıralayalım.
``` Sql
(
	SELECT first_name FROM actor
)
UNION ALL
(
	SELECT first_name FROM customer
);
```

## TASK 2
Actor ve customer tablolarında bulunan first_name sütunları için kesişen verileri sıralayalım.
```Sql
(
	SELECT first_name FROM actor
)
INTERSECT
(
	SELECT first_name FROM customer
);
```

## TASK 3
Actor ve customer tablolarında bulunan first_name sütunları için ilk tabloda bulunan ancak ikinci tabloda bulunmayan verileri sıralayalım.
```Sql
(
	SELECT first_name FROM actor
)
EXCEPT
(
	SELECT first_name FROM customer
);
```

#### Kodlarin SQL veri tabanı üzerinde yazılmış şekline UNION, INTERSECT, EXCEPT klasörü içerisindeki fotograflardan göz ata bilirsiniz.



