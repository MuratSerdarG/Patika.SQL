# Proje Sahibi: Patika.Dev 
# Proje Konusu: Veri Yapıları ve Algoritmalar
## Konu : SQL

#### 1. Sorunun cevabı için :
- film tablosunda bulunan ve film ismi (title) 'n' karakteri ile biten en uzun (length) 5 filmi sıralayınız.
```sql
SELECT * FROM film
WHERE title LIKE ‘%n’
ORDER BY length DESC
LIMIT 5
```

#### 2. Sorunun cevabı için :
- film tablosunda bulunan ve film ismi (title) 'n' karakteri ile biten en kısa (length) ikinci(6,7,8,9,10) 5 filmi(6,7,8,9,10) sıralayınız.
```sql
SELECT * FROM film
WHERE title LIKE ‘%n’
ORDER BY length ASC
OFFSET 5
LIMIT 5
```

#### 3. Sorunun cevabı için :
- customer tablosunda bulunan last_name sütununa göre azalan yapılan sıralamada store_id 1 olmak koşuluyla ilk 4 veriyi sıralayınız.
```sql
SELECT * FROM customer
WHERE store_id=1
ORDER BY last_name DESC
LIMIT 4
```
