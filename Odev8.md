# Proje Sahibi: Patika.Dev 
# Proje Konusu: Veri Yapıları ve Algoritmalar
## Konu : SQL

#### 1. Sorunun cevabı için :
- test veritabanınızda employee isimli sütun bilgileri id(INTEGER), name VARCHAR(50), birthday DATE, email VARCHAR(100) olan bir tablo oluşturalım.
```
CREATE TABLE employee (
  id INTEGER,
  name VARCHAR(50),
  birthday DATE,
  email VARCHAR(100));
```

#### 2. Sorunun cevabı için :
- Oluşturduğumuz employee tablosuna 'Mockaroo' servisini kullanarak 50 adet veri ekleyelim.

![mockaroo](https://user-images.githubusercontent.com/93589387/154493855-d29b1071-9f79-46ef-b5e1-04a5b9974a9f.jpg)


```
![mockaroo](https://user-images.githubusercontent.com/93589387/154493855-d29b1071-9f79-46ef-b5e1-04a5b9974a9f.jpg)

Örnekler;
insert into employee (id, name, birthday , email ) values (1, 'Judith', '1951-10-31', 'jskelbeck0@phpbb.com');
insert into employee (id, name, birthday , email ) values (2, 'Helaina', '1967-07-26', 'hmcdaid1@angelfire.com');
insert into employee (id, name, birthday , email ) values (3, 'Bertie', '1971-02-02', 'banespie2@army.mil');

```

#### 3. Sorunun cevabı için :
- Sütunların her birine göre diğer sütunları güncelleyecek 5 adet UPDATE işlemi yapalım.
```
update employee
set name='Warlock'
Where id=4
RETURNING *; 

update employee
set email='akettridgec@digger.com'
Where id=13
RETURNING *;

update employee
set email='sseyd@europe.eu'
Where id=14
RETURNING *;

update employee
set name='ShadowShaman'
Where id=22
RETURNING *;

update employee
set name='Scherlock'
Where id=39
RETURNING *;
```
#### 4. Sorunun cevabı için :
- Sütunların her birine göre ilgili satırı silecek 5 adet DELETE işlemi yapalım.
```
Tek tek yapmak istersek;
DELETE FROM employee
WHERE id=9;

5’i birden toplu yapmak istersek;
DELETE FROM employee
WHERE id IN(11,13,15,17,19);
```

