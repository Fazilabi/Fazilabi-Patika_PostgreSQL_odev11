# Fazilabi-Patika_PostgreSQL_odev11
## [Patika.dev](https://academy.patika.dev/)
### Aşağıdaki sorgu senaryolarını dvdrental örnek veri tabanı üzerinden gerçekleştiriniz.

### 1.actor ve customer tablolarında bulunan first_name sütunları için tüm verileri sıralayalım.
`(SELECT first_name FROM actor)`<br>
`UNION`<br>
`(SELECT first_name FROM customer);`

### 2.actor ve customer tablolarında bulunan first_name sütunları için kesişen verileri sıralayalım.
`(SELECT first_name FROM ACTOR)`<br>
`INTERSECT`<br>
`(SELECT first_name FROM CUSTOMER);`

### 3.actor ve customer tablolarında bulunan first_name sütunları için ilk tabloda bulunan ancak ikinci tabloda bulunmayan verileri sıralayalım.
`(SELECT first_name FROM ACTOR)`<br>
`EXCEPT`<br>
`(SELECT first_name FROM CUSTOMER);`

### 4.İlk 3 sorguyu tekrar eden veriler için de yapalım.
`(SELECT first_name FROM ACTOR)`<br>
`UNION ALL`<br>
`(SELECT first_name FROM CUSTOMER);`
