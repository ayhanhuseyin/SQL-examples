### Merhabalar, **dvdrental** örnek veri tabanını kullanarak **DICTINCT** ve **COUNT** operatorleri ile ilgili 3 adet örnek çalışma yapacağız. 
**Dvdrental** örnek verı tabanını **SQL-examples** dosyaları arasına ekledım, oradan elde ede bilirsiniz. Ve ya [Buradan](https://www.postgresqltutorial.com/postgresql-getting-started/postgresql-sample-database/) Internet aracılığıyla kendiniz indire bilirsiniz.
## TASK 1 
Film tablosunda bulunan replacement_cost sütununda bulunan birbirinden farklı değerleri sıralayınız.
```Sql
SELECT DISTINCT replacement_cost FROM film;
```

## TASK 2
Film tablosunda bulunan replacement_cost sütununda birbirinden farklı kaç tane veri vardır?
```Sql
SELECT COUNT (DISTINCT replacement_cost) FROM film;
```

## TASK 3
Film tablosunda bulunan film isimlerinde (title) kaç tanesini T karakteri ile başlar ve aynı zamanda rating 'G' ye eşittir?
```Sql
SELECT COUNT (DISTINCT title LIKE 'T%' AND rating = 'G') FROM film;
```

## TASK 4
City tablosundaki şehir isimlerinin kaç tanesi 'R' veya r karakteri ile biter?
```Sql
SELECT COUNT (*) FROM city
WHERE city LIKE 'R%r';
```
