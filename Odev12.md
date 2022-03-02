# Proje Sahibi: Patika.Dev 
# Proje Konusu: Veri Yapıları ve Algoritmalar
## Konu : SQL

#### 1. Sorunun cevabı için :
- film tablosunda film uzunluğu length sütununda gösterilmektedir. Uzunluğu ortalama film uzunluğundan fazla kaç tane film vardır?
```sql
SELECT COUNT(*)
FROM film
WHERE length>(SELECT AVG(length) FROM film);
```

#### 2. Sorunun cevabı için :
- film tablosunda en yüksek rental_rate değerine sahip kaç tane film vardır?
```sql
SELECT COUNT(*)
FROM film
WHERE rental_rate =(SELECT MAX(rental_rate) FROM film);
```

#### 3. Sorunun cevabı için :
- film tablosunda en düşük rental_rate ve en düşün replacement_cost değerlerine sahip filmleri sıralayınız.
```sql
SELECT *
FROM film
WHERE rental_rate =(SELECT MIN(rental_rate) FROM film) AND replacement_cost=( SELECT MIN(replacement_cost) FROM film);
```

#### 4. Sorunun cevabı için :
- payment tablosunda en fazla sayıda alışveriş yapan müşterileri(customer) sıralayınız.
```sql
SELECT customer.first_name, customer.last_name
FROM payment
INNER JOIN customer 
ON payment.customer_id = customer.customer_id
WHERE payment.amount =( SELECT MAX(amount) FROM payment);
```
