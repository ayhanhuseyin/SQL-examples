### Merhabalar, **dvdrental** örnek veri tabanını kullanarak **LIKE** ve **ILIKE** operatorleri ile ilgili 4 adet örnek çalışma yapacağız. 
**Dvdrental** örnek verı tabanını **SQL-examples** dosyaları arasına ekledım, oradan elde ede bilirsiniz. Ve ya [Buradan](https://www.postgresqltutorial.com/postgresql-getting-started/postgresql-sample-database/) Internet aracılığıyla kendiniz indire bilirsiniz.
## TASK 1 
Country tablosunda bulunan country sütunundaki ülke isimlerinden 'A' karakteri ile başlayıp 'a' karakteri ile sonlananları sıralayınız.
```Sql
SELECT * FROM country
WHERE country LIKE 'A%a';
```

## TASK 2
Country tablosunda bulunan country sütunundaki ülke isimlerinden en az 6 karakterden oluşan ve sonu 'n' karakteri ile sonlananları sıralayınız.
```Sql
SELECT * FROM country
WHERE country LIKE '_____n';
```

## TASK 3
Film tablosunda bulunan title sütunundaki film isimlerinden en az 4 adet büyük ya da küçük harf farketmesizin 'T' karakteri içeren film isimlerini sıralayınız.
```Sql
SELECT * FROM film
WHERE title ILIKE 'T%';
```

## TASK 4
Film tablosunda bulunan tüm sütunlardaki verilerden title 'C' karakteri ile başlayan ve uzunluğu (length) 90 dan büyük olan ve rental_rate 2.99 olan verileri sıralayınız.
```Sql
SELECT * FROM film
WHERE title LIKE 'C%' AND length>90 AND rental_rate = 2.99;
```

#### Kodlarin SQL veri tabanı üzerinde yazılmış şekline **LIKE, ILIKE** klasörü içerisindeki fotograflardan göz ata bilirsiniz.
