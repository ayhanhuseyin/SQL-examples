### Merhabalar, **dvdrental** örnek veri tabanını kullanarak **AND** ve **OR** operatorleri ile ilgili 5 adet örnek çalışma yapacağız. 
**Dvdrental** örnek verı tabanını **SQL-examples** dosyaları arasına ekledım, oradan elde ede bilirsiniz. Ve ya [Buradan](https://www.postgresqltutorial.com/postgresql-getting-started/postgresql-sample-database/) Internet aracılığıyla kendiniz indire bilirsiniz.
## TASK 1 
Film tablosunda bulunan title ve description sütunlarındaki verileri sıralayınız.
```Sql
SELECT title, desription FROM film;
```

## TASK 2
Film tablosunda bulunan tüm sütunlardaki verileri film uzunluğu (length) 60 dan büyük VE 75 ten küçük olma koşullarıyla sıralayınız.
```Sql
SELECT * FROM film
WHERE length>60 AND length<75;
```

## TASK 3
Film tablosunda bulunan tüm sütunlardaki verileri rental_rate 0.99 VE replacement_cost 12.99 VEYA 28.99 olma koşullarıyla sıralayınız.
```Sql
SELECT * FROM film
WHERE rental_rate = 0.99 AND replacement_cost = 12.99 OR replacement_cost = 28.99
```

## TASK 4
Customer tablosunda bulunan first_name sütunundaki değeri 'Mary' olan müşterinin last_name sütunundaki değeri nedir?
```Sql
SELECT * FROM customer
WHERE first_name = 'Mary'
```
**Not :** First_name'i 'Mary' olan müşteriyi veri tabanından çekdiğimizde Mary ile ilgili tüm bilgiler karşımıza çıkıyor, ve buradan da last_name'i görüntüleye biliyoruz. TASK 4 isimli fotografa tiklayarak daha detayli baka bilirisiniz.


## TASK 5
Film tablosundaki uzunluğu(length) 50 ten büyük OLMAYIP aynı zamanda rental_rate değeri 2.99 veya 4.99 OLMAYAN verileri sıralayınız.
```Sql
SELECT * FROM film
WHERE length<50 AND NOT (rental_rate = 2.99 OR rental_rate = 4.99);
```
