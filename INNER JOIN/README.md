### Merhabalar, **dvdrental** örnek veri tabanını kullanarak INNER JOIN ile ilgili 3 adet örnek çalışma yapacağız. 
**Dvdrental** örnek verı tabanını **SQL-examples** dosyaları arasına ekledım, oradan elde ede bilirsiniz. Ve ya [Buradan](https://www.postgresqltutorial.com/postgresql-getting-started/postgresql-sample-database/) Internet aracılığıyla kendiniz indire bilirsiniz.
## TASK 1 
City tablosu ile country tablosunda bulunan şehir (city) ve ülke (country) isimlerini birlikte görebileceğimiz INNER JOIN sorgusunu yazınız.
``` Sql
SELECT country, city FROM city
INNER JOIN country ON city.country.id = country.country_id;
```

## TASK 2
Customer tablosu ile payment tablosunda bulunan payment_id ile customer tablosundaki first_name ve last_name isimlerini birlikte görebileceğimiz INNER JOIN sorgusunu yazınız.
```Sql
SELECT payment.payment_id, customer.first_name, customer.last_name FROM payment
INNER JOIN customer ON payment.customer_id = customer.customer_id;
```

## TASK 3
Customer tablosu ile rental tablosunda bulunan rental_id ile customer tablosundaki first_name ve last_name isimlerini birlikte görebileceğimiz INNER JOIN sorgusunu yazınız.
```Sql
SELECT rental.rental_id, customer.first_name, customer.last_name FROM customer
INNER JOIN rental ON rental.customer_id = customer.customer_id;
```

#### Kodlarin SQL veri tabanı üzerinde yazılmış şekline INNER JOIN klasörü içerisindeki fotograflardan göz ata bilirsiniz.

