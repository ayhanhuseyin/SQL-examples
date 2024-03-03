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
