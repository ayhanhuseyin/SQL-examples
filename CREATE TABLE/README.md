### Tablo oluşturmak
Bu projemizde artık örnek veri tabanı yerine kendi veribatanımızı oluşturup üzerinde bazı çalışmalar yapacağız. Örnek veri tabanı olustururken zaman kaybetmemek açısından verileri Mockaroo sitesini kullanarak olusturacağız. Siteye [Buradan](https://www.mockaroo.com/) ulaşabilirsiniz.


## TASK 1
Test veritabanınızda employee isimli sütun bilgileri id(INTEGER), name VARCHAR(50), birthday DATE, email VARCHAR(100) olan bir tablo oluşturalım.
```Sql
CREATE TABLE employee (
	id SERIAL PRIMARY KEY,
	name VARCHAR(50),
	birthday DATE,
	email VARCHAR(100)
);
```
