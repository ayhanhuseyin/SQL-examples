### Merhabalar, **dvdrental** örnek veri tabanını kullanarak **ORDER BY**,  **LIMIT** ve **OFFSET** operatörleri ile ilgili 3 adet örnek çalışma yapacağız. 
**Dvdrental** örnek veri tabanını **SQL-examples** dosyaları arasına ekledım, oradan elde ede bilirsiniz. Ve ya [Buradan](https://www.postgresqltutorial.com/postgresql-getting-started/postgresql-sample-database/) Internet aracılığıyla kendiniz indire bilirsiniz.
## TASK 1 
Film tablosunda bulunan ve film ismi (title) 'n' karakteri ile biten en uzun (length) 5 filmi sıralayınız.
```Sql
SELECT * FROM film
WHERE title LIKE '%n'
ORDER BY length DESC
LIMIT 5;
```

## TASK 2
Film tablosunda bulunan ve film ismi (title) 'n' karakteri ile biten en kısa (length) ikinci(6,7,8,9,10) 5 filmi(6,7,8,9,10) sıralayınız.
```Sql
SELECT * FROM film
WHERE title LIKE '%n'
ORDER BY length DESC
OFFSET 5
LIMIT 5;
```

## TASK 3
Customer tablosunda bulunan last_name sütununa göre azalan yapılan sıralamada store_id 1 olmak koşuluyla ilk 4 veriyi sıralayınız.
```Sql
SELECT * FROM customer
WHERE store_id = 1
ORDER BY last_name DESC
LIMIT 4;
```


#### Kodlarin SQL veri tabanı üzerinde yazılmış şekline **ORDER BY, LİMİT, OFFSET** klasörü içerisindeki fotograflardan göz ata bilirsiniz.

