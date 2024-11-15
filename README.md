# SQL-TABLEAU_FOOD_PRODUCTION_IN_WOLRD
Proyek ini bertujuan untuk melakukan operasi CRUD (Create, Read, Update, Delete) pada dataset produksi bahan pangan global yang mencakup 226 negara menggunakan data dari tahun 1961 hingga 2023 dengan 22 jenis bahan pangan. SQL digunakan untuk mengelola dan memanipulasi data agar dapat menghasilkan analisis yang lebih akurat. Selain itu, Tableau digunakan untuk menciptakan visualisasi analitis yang memberikan wawasan lebih mendalam mengenai tren dan pola produksi pangan di berbagai negara sepanjang periode tersebut.
## Dataset
https://www.kaggle.com/datasets/rafsunahmad/world-food-production

## Mengganti tipe data
```sql
ALTER TABLE food_production
ALTER COLUMN [Maize Production (tonnes)] FLOAT;

ALTER TABLE food_production
ALTER COLUMN [Year] DATE;

ALTER TABLE food_production
ALTER COLUMN [Rice Production ( tonnes)] FLOAT;

ALTER TABLE food_production
ALTER COLUMN [Yams Production (tonnes)] FLOAT;

ALTER TABLE food_production
ALTER COLUMN [Wheat Production (tonnes)] FLOAT;

ALTER TABLE food_production
ALTER COLUMN [Tomatoes Production (tonnes)] FLOAT;

ALTER TABLE food_production
ALTER COLUMN [Tea  Production ( tonnes )] FLOAT;

ALTER TABLE food_production
ALTER COLUMN [Sweet potatoes Production (tonnes)] FLOAT;

ALTER TABLE food_production
ALTER COLUMN [Yams Production (tonnes)] FLOAT;

ALTER TABLE food_production
ALTER COLUMN [Sunflower seed Production (tonnes)] FLOAT;

ALTER TABLE food_production
ALTER COLUMN [Sugar cane Production (tonnes)] FLOAT;

ALTER TABLE food_production
ALTER COLUMN [Soybeans Production (tonnes)] FLOAT;

ALTER TABLE food_production
ALTER COLUMN [Rye Production (tonnes)] FLOAT;

ALTER TABLE food_production
ALTER COLUMN [Potatoes Production (tonnes)] FLOAT;

ALTER TABLE food_production
ALTER COLUMN [Oranges Production (tonnes)] FLOAT;

ALTER TABLE food_production
ALTER COLUMN [Peas dry Production ( tonnes)] FLOAT;

ALTER TABLE food_production
ALTER COLUMN [Grapes Production (tonnes)] FLOAT;

ALTER TABLE food_production
ALTER COLUMN [Coffee green Production ( tonnes)] FLOAT;

ALTER TABLE food_production
ALTER COLUMN [Cocoa beans Production (tonnes)] FLOAT;

ALTER TABLE food_production
ALTER COLUMN [Meat chicken Production (tonnes)"] FLOAT;

ALTER TABLE food_production
ALTER COLUMN [Bananas Production ( tonnes)] FLOAT;

ALTER TABLE food_production
ALTER COLUMN [Avocados Production (tonnes)] FLOAT;

ALTER TABLE food_production
ALTER COLUMN [Apples Production (tonnes)] FLOAT;
```
