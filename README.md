1#SORU - film tablosunda bulunan filmleri rating değerlerine göre gruplayınız.

1#CEVAP - SELECT title, rating FROM film
GROUP BY title, rating
ORDER BY rating;

1#<img width="960" alt="1" src="https://user-images.githubusercontent.com/129968939/230917798-ec5f6e06-a541-42cd-8696-30add3448ec4.png">

2#SORU - film tablosunda bulunan filmleri replacement_cost sütununa göre grupladığımızda film sayısı 50 den fazla olan replacement_cost değerini ve karşılık gelen film sayısını sıralayınız.

2#CEVAP - SELECT replacement_cost, COUNT (*) FROM film
GROUP BY replacement_cost
HAVING COUNT (*) > 50;

2#<img width="960" alt="2" src="https://user-images.githubusercontent.com/129968939/230918660-ddd74595-714f-4fbb-925a-39d41a192670.png">

3#SORU - customer tablosunda bulunan store_id değerlerine karşılık gelen müşteri sayılarını nelerdir?

3#CEVAP - SELECT store_id, COUNT (*) FROM customer
GROUP BY store_id;

3#<img width="960" alt="3" src="https://user-images.githubusercontent.com/129968939/230920038-c0612e3c-7b23-4786-8325-7f5de6e81f09.png">

4#SORU - city tablosunda bulunan şehir verilerini country_id sütununa göre gruplandırdıktan sonra en fazla şehir sayısı barındıran country_id bilgisini ve şehir sayısını paylaşınız.

4#CEVAP - SELECT country_id, COUNT (*) FROM city
GROUP BY country_id
ORDER BY COUNT (*) DESC
LIMIT 1;

4#<img width="960" alt="4" src="https://user-images.githubusercontent.com/129968939/230920906-ba44f0ae-3f65-4214-8688-2c3bcb21b5be.png">
