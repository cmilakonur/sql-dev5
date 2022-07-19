# sql-dev5
patika.dev linkim: https://app.patika.dev/cmilakonur <br />

1- film tablosunda bulunan ve film ismi (title) 'n' karakteri ile biten en uzun (length) 5 filmi sıralayınız. <br />
SELECT * FROM film WHERE title LIKE '%n' <br />
ORDER BY length DESC LIMIT 5; <br />

2- film tablosunda bulunan ve film ismi (title) 'n' karakteri ile biten en kısa (length) ikinci(6,7,8,9,10) 5 filmi(6,7,8,9,10) sıralayınız. <br />
SELECT * FROM film WHERE title LIKE '%n' <br />
ORDER BY length OFFSET 5 LIMIT 5; <br />

3- customer tablosunda bulunan last_name sütununa göre azalan yapılan sıralamada store_id 1 olmak koşuluyla ilk 4 veriyi sıralayınız. <br />
SELECT * FROM customer WHERE store_id=1 <br />
ORDER BY last_name DESC LIMIT 4; <br />
