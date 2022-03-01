# Proje Sahibi: Patika.Dev 
# Proje Konusu: Veri Yapıları ve Algoritmalar
## Konu : SQL

#### 1. Sorunun cevabı için :
- country tablosunda bulunan country sütunundaki ülke isimlerinden 'A' karakteri ile başlayıp 'a' karakteri ile sonlananları sıralayınız.
```sql
SELECT country
FROM country
Where country LIKE ‘A%a’;
```

#### 2. Sorunun cevabı için :
- country tablosunda bulunan country sütunundaki ülke isimlerinden en az 6 karakterden oluşan ve sonu 'n' karakteri ile sonlananları sıralayınız.
```sql
SELECT country
FROM country
Where country LIKE ‘%_____n’;
```

#### 3. Sorunun cevabı için :
- film tablosunda bulunan title sütunundaki film isimlerinden en az 4 adet büyük ya da küçük harf farketmesizin 'T' karakteri içeren film isimlerini sıralayınız.
```sql
SELECT title
FROM film
WHERE title ILIKE ‘%t%t%t%t%’;
```

#### 4. Sorunun cevabı için :
- film tablosunda bulunan tüm sütunlardaki verilerden title 'C' karakteri ile başlayan ve uzunluğu (length) 90 dan büyük olan ve rental_rate 2.99 olan verileri sıralayınız.
```sql
SELECT *
FROM film
WHERE title LIKE ‘C%’ AND length > 90 AND rental_rate=2.99;
```
