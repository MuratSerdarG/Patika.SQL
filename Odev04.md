# Proje Sahibi: Patika.Dev 
# Proje Konusu: Veri Yapıları ve Algoritmalar
## Konu : SQL

#### 1. Sorunun cevabı için :
- film tablosunda bulunan replacement_cost sütununda bulunan birbirinden farklı değerleri sıralayınız.
```sql
SELECT DISTINCT replacement_cost
FROM film;
```

#### 2. Sorunun cevabı için :
- film tablosunda bulunan replacement_cost sütununda birbirinden farklı kaç tane veri vardır?
```sql
SELECT COUNT (DISTINCT replacement_cost)
FROM film;
```

#### 3. Sorunun cevabı için :
- film tablosunda bulunan film isimlerinde (title) kaç tanesini T karakteri ile başlar ve aynı zamanda rating 'G' ye eşittir?
```sql
SELECT COUNT (title)
FROM film
WHERE title LIKE ‘T%’ AND rating=’G’;
```

#### 4. Sorunun cevabı için :
- country tablosunda bulunan ülke isimlerinden (country) kaç tanesi 5 karakterden oluşmaktadır?
```sql
SELECT COUNT(country)
FROM country
WHERE country LIKE ‘_____’;
```

#### 5. Sorunun cevabı için :
- city tablosundaki şehir isimlerinin kaç tanesi 'R' veya r karakteri ile biter?
```sql
SELECT city
FROM city
WHERE city LIKE ‘%R’  OR city LIKE’%r’;
```
