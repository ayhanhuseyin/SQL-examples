### Merhabalar, **dvdrental** örnek veri tabanını kullanarak SUBQUERIES ile ilgili 3 adet örnek çalışma yapacağız. 
**Dvdrental** örnek verı tabanını **SQL-examples** dosyaları arasına ekledım, oradan elde ede bilirsiniz. Ve ya [Buradan](https://www.postgresqltutorial.com/postgresql-getting-started/postgresql-sample-database/) Internet aracılığıyla kendiniz indire bilirsiniz.
## TASK 1 
Film tablosunda film uzunluğu length sütununda gösterilmektedir. Uzunluğu ortalama film uzunluğundan fazla kaç tane film vardır?
``` Sql
SELECT COUNT()* FROM film
WHERE length > (SELECT AVG(length) FROM film);
```

## TASK 2
Film tablosunda en yüksek rental_rate değerine sahip kaç tane film vardır?
```Sql
SELECT COUNT(*) FROM film
WHERE rental_rate = SELECT (MAX(rental_rate) FROM film);
```

## TASK 3
Film tablosunda en düşük rental_rate ve en düşün replacement_cost değerlerine sahip filmleri sıralayınız.
```Sql
SELECT * FROM film
WHERE rental_rate = (SELECT MIN(rental_rate) FROM film)
AND replacement_cost = (SELECT MIN(replacement_cost) FROM film); 
```

#### Kodlarin SQL veri tabanı üzerinde yazılmış şekline SUBQUERIES klasörü içerisindeki fotograflardan göz ata bilirsiniz.



