# Proje Sahibi: Patika.Dev 
# Proje Konusu: Veri Yapıları ve Algoritmalar
## Konu : SQL

#### 1. Sorunun cevabı için :
- city tablosu ile country tablosunda bulunan şehir (city) ve ülke (country) isimlerini birlikte görebileceğimiz LEFT JOIN sorgusunu yazınız.
```sql
SELECT city, country 
FROM city
LEFT JOIN country 
ON city.country_id=country.country_id;
```

#### 2. Sorunun cevabı için :
- customer tablosu ile payment tablosunda bulunan payment_id ile customer tablosundaki first_name ve last_name isimlerini birlikte görebileceğimiz RIGHT JOIN sorgusunu yazınız.
```sql
SELECT payment_id, first_name, last_name
FROM customer
RIGHT JOIN payment
ON customer.customer_id=payment.customer.id;
```

#### 3. Sorunun cevabı için :
- customer tablosu ile rental tablosunda bulunan rental_id ile customer tablosundaki first_name ve last_name isimlerini birlikte görebileceğimiz FULL JOIN sorgusunu yazınız.
```sql
SELECT rental_id, first_name, last_name
FROM customer
FULL JOIN rental
ON customer.customer_id=rental.customer.id;
```

