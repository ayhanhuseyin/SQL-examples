### Merhabalar, **dvdrental** örnek veri tabanını kullanarak **Aggragate fonksiyonlari** ile ilgili 4 adet örnek çalışma yapacağız. 
**Dvdrental** örnek verı tabanını **SQL-examples** dosyaları arasına ekledim, oradan elde ede bilirsiniz. Ve ya [Buradan](https://www.postgresqltutorial.com/postgresql-getting-started/postgresql-sample-database/) Internet aracılığıyla kendiniz indire bilirsiniz.
## TASK 1 
Film tablosunda bulunan rental_rate sütunundaki değerlerin ortalaması nedir?
```Sql
SELECT ROUND(AVG(rental_rate), 3) FROM film;
```

## TASK 2
Film tablosunda bulunan filmlerden kaç tanesi 'C' karakteri ile başlar?
```Sql
SELECT COUNT(*) FROM film
WHERE title LIKE 'C%';
```

## TASK 3
Film tablosunda bulunan filmlerden rental_rate değeri 0.99 a eşit olan en uzun (length) film kaç dakikadır?
```Sql
SELECT MAX(length) FROM film
WHERE rental_rate = 0.99;
```

## TASK 4
Film tablosunda bulunan filmlerin uzunluğu 150 dakikadan büyük olanlarına ait kaç farklı replacement_cost değeri vardır?
```Sql
SELECT COUNT(replacement_cost) FROM film
WHERE length>150;
```


#### Kodlarin SQL veri tabanı üzerinde yazılmış şekline **Aggragate Fonsksiyonlari** klasörü içerisindeki fotograflardan göz ata bilirsiniz.

