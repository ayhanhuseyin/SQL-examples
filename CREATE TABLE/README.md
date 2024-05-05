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

## TASK 2
Oluşturduğumuz employee tablosuna 'Mockaroo' servisini kullanarak 50 adet veri ekleyelim.
```Sql
insert into employee (name, email, birthday) values ('Merla', 'mgaitley0@sina.com.cn', '1990-07-25');
insert into employee (name, email, birthday) values ('Helaina', 'hhathaway1@ovh.net', '1996-03-31');
insert into employee (name, email, birthday) values ('Aurthur', 'alune2@squarespace.com', '1991-02-08');
insert into employee (name, email, birthday) values ('Ric', 'rgeorges3@netscape.com', '1999-06-23');
insert into employee (name, email, birthday) values ('Zonnya', 'zpossell4@timesonline.co.uk', '2000-10-24');
insert into employee (name, email, birthday) values ('Matilda', 'mwinks5@symantec.com', '2008-05-05');
insert into employee (name, email, birthday) values ('Katharyn', 'kstutter6@goodreads.com', '2003-04-05');
insert into employee (name, email, birthday) values ('Jareb', 'jcristoforetti7@freewebs.com', '1997-10-29');
insert into employee (name, email, birthday) values ('Dante', 'ddeane8@admin.ch', '2006-08-29');
insert into employee (name, email, birthday) values ('Fleming', 'fgoggins9@ebay.co.uk', '2000-03-11');
insert into employee (name, email, birthday) values ('Pall', 'pmashroa@taobao.com', '1995-05-14');
insert into employee (name, email, birthday) values ('Cull', 'cmabeb@odnoklassniki.ru', '2003-05-17');
insert into employee (name, email, birthday) values ('Claire', 'ckobeltc@wikia.com', '2000-03-06');
insert into employee (name, email, birthday) values ('Germana', 'ggladwind@admin.ch', '1991-06-14');
insert into employee (name, email, birthday) values ('Jilli', 'jwethericke@reverbnation.com', '1994-06-08');
insert into employee (name, email, birthday) values ('Burch', 'bpalkf@people.com.cn', '1994-12-24');
insert into employee (name, email, birthday) values ('Way', 'wagerg@wikipedia.org', '2005-05-22');
insert into employee (name, email, birthday) values ('Sam', 'seastbyh@prlog.org', '2003-01-31');
insert into employee (name, email, birthday) values ('Danny', 'dcarlei@sitemeter.com', '2007-04-25');
insert into employee (name, email, birthday) values ('Lowrance', 'lcowitzj@weather.com', '2001-07-18');
insert into employee (name, email, birthday) values ('Merrel', 'mwendoverk@i2i.jp', '1990-05-28');
insert into employee (name, email, birthday) values ('Arri', 'abladgel@studiopress.com', '1992-07-01');
insert into employee (name, email, birthday) values ('Kesley', 'kaddym@naver.com', '2002-03-22');
insert into employee (name, email, birthday) values ('Dreddy', 'dcheneryn@naver.com', '1992-04-05');
insert into employee (name, email, birthday) values ('Celestyna', 'codriscollo@berkeley.edu', '2009-01-17');
insert into employee (name, email, birthday) values ('Casper', 'cclutep@wordpress.com', '1999-05-09');
insert into employee (name, email, birthday) values ('Guinna', 'gcondieq@elpais.com', '1997-08-20');
insert into employee (name, email, birthday) values ('Arlene', 'aattawayr@cam.ac.uk', '1996-03-13');
insert into employee (name, email, birthday) values ('Cathee', 'cimisons@dailymotion.com', '2007-02-06');
insert into employee (name, email, birthday) values ('Wendel', 'wrubiet@cnbc.com', '2000-03-31');
insert into employee (name, email, birthday) values ('Michale', 'mbearsmoreu@yandex.ru', '1999-07-12');
insert into employee (name, email, birthday) values ('Valeda', 'vcoyettv@parallels.com', '1999-11-26');
insert into employee (name, email, birthday) values ('Chere', 'cvolagew@apple.com', '1990-06-15');
insert into employee (name, email, birthday) values ('Drucill', 'dmyriex@hibu.com', '1992-09-23');
insert into employee (name, email, birthday) values ('Mead', 'mgarmstony@rakuten.co.jp', '2004-12-13');
insert into employee (name, email, birthday) values ('Eyde', 'ebackez@ning.com', '1997-01-04');
insert into employee (name, email, birthday) values ('Franky', 'fsings10@t-online.de', '1992-05-29');
insert into employee (name, email, birthday) values ('Aveline', 'asmyth11@bloglines.com', '2008-12-20');
insert into employee (name, email, birthday) values ('Mace', 'mforkan12@hugedomains.com', '2008-03-04');
insert into employee (name, email, birthday) values ('Chere', 'csilberschatz13@answers.com', '1997-10-31');
insert into employee (name, email, birthday) values ('Leone', 'ldavidai14@usnews.com', '2001-04-16');
insert into employee (name, email, birthday) values ('Vance', 'vgouny15@pagesperso-orange.fr', '2004-11-09');
insert into employee (name, email, birthday) values ('Claudius', 'cpiggrem16@virginia.edu', '1990-08-12');
insert into employee (name, email, birthday) values ('Sigismundo', 'svinton17@istockphoto.com', '1990-11-04');
insert into employee (name, email, birthday) values ('Leonardo', 'lpetrakov18@homestead.com', '2009-03-02');
insert into employee (name, email, birthday) values ('Bartholemy', 'bphaup19@newsvine.com', '1996-04-02');
insert into employee (name, email, birthday) values ('Cody', 'ctrusdale1a@time.com', '2008-01-19');
insert into employee (name, email, birthday) values ('Kristen', 'kbrendish1b@istockphoto.com', '2002-03-13');
insert into employee (name, email, birthday) values ('Corey', 'ckynsey1c@nydailynews.com', '2006-09-25');
insert into employee (name, email, birthday) values ('Roxanna', 'radamovsky1d@wikipedia.org', '1992-10-05');
```

## TASK 3
Sütunların her birine göre diğer sütunları güncelleyecek 3 adet UPDATE işlemi yapalım.
```Sql
UPDATE employee
SET name = 'Jonh'
WHERE id = 5
```

```Sql
 UPDATE employee
 SET name = 'Billie'
 WHERE id = 47
```

```Sql
UPDATE employee
SET name = 'Carter'
WHERE id>40
```

