### Merhabalar, **dvdrental** örnek veri tabanını kullanarak GROUP BY, HAVING operatorleri ile ilgili 4 adet örnek çalışma yapacağız. 
**Dvdrental** örnek verı tabanını **SQL-examples** dosyaları arasına ekledım, oradan elde ede bilirsiniz. Ve ya [Buradan](https://www.postgresqltutorial.com/postgresql-getting-started/postgresql-sample-database/) Internet aracılığıyla kendiniz indire bilirsiniz.
## TASK 1 
Film tablosunda bulunan filmleri rating değerlerine göre gruplayınız.
```Sql
SELECT rating FROM film
GROUP BY rating
```

## TASK 2
Film tablosunda bulunan filmleri replacement_cost sütununa göre grupladığımızda film sayısı 50 den fazla olan replacement_cost değerini ve karşılık gelen film sayısını sıralayınız.
```Sql
SELECT replacement_cost, COUNT(*) FROM film
GROUP BY replacement_cost
HAVING COUNT(*)>50;
```

## TASK 3
Customer tablosunda bulunan store_id değerlerine karşılık gelen müşteri sayılarını nelerdir?
```Sql
SELECT store_id, COUNT(*) FROM customer
GROUP BY store_id;
```

## TASK 4
City tablosunda bulunan şehir verilerini country_id sütununa göre gruplandırdıktan sonra en fazla şehir sayısı barındıran country_id bilgisini ve şehir sayısını paylaşınız.
```Sql
SELECT country_id, COUNT(*) FROM city
GROUP BY country_id
ORDER BY country_id DESC
LIMIT 1;
```


#### Kodlarin SQL veri tabanı üzerinde yazılmış şekline GROUP BY, HAVING klasörü içerisindeki fotograflardan göz ata bilirsiniz.

