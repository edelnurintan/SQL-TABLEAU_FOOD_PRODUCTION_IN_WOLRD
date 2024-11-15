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
ALTER COLUMN [Meat chicken Production (tonnes)] FLOAT;

ALTER TABLE food_production
ALTER COLUMN [Bananas Production ( tonnes)] FLOAT;

ALTER TABLE food_production
ALTER COLUMN [Avocados Production (tonnes)] FLOAT;

ALTER TABLE food_production
ALTER COLUMN [Apples Production (tonnes)] FLOAT;

ALTER TABLE food_production
ALTER COLUMN [Palm oil Production (tonnes)] FLOAT;
```
## MENGHITUNG RATA-RATA PRODUKSI PER KOMODITAS SESUAI NEGARA
``` sql
SELECT 
    Entity,
    AVG([Maize Production (tonnes)]) AS Avg_Maize,
    AVG([Rice Production ( tonnes)]) AS Avg_Rice,
    AVG([Yams Production (tonnes)]) AS Avg_Yams,
    AVG([Wheat Production (tonnes)]) AS Avg_Wheat,
    AVG([Tomatoes Production (tonnes)]) AS Avg_Tomatoes,
    AVG([Tea  Production ( tonnes )]) AS Avg_Tea,
    AVG([Sweet potatoes Production (tonnes)]) AS Avg_SweetPotatoes,
    AVG([Sunflower seed Production (tonnes)]) AS Avg_SunflowerSeed,
    AVG([Sugar cane Production (tonnes)]) AS Avg_SugarCane,
    AVG([Soybeans Production (tonnes)]) AS Avg_Soybeans,
    AVG([Rye Production (tonnes)]) AS Avg_Rye,
    AVG([Potatoes Production (tonnes)]) AS Avg_Potatoes,
    AVG([Oranges Production (tonnes)]) AS Avg_Oranges,
    AVG([Peas dry Production ( tonnes)]) AS Avg_PeasDry,
    AVG([Palm oil Production (tonnes)]) AS Avg_PalmOil,
    AVG([Grapes Production (tonnes)]) AS Avg_Grapes,
    AVG([Coffee green Production ( tonnes)]) AS Avg_CoffeeGreen,
    AVG([Cocoa beans Production (tonnes)]) AS Avg_CocoaBeans,
    AVG([Meat chicken Production (tonnes)]) AS Avg_MeatChicken,
    AVG([Bananas Production ( tonnes)]) AS Avg_Bananas,
    AVG([Avocados Production (tonnes)]) AS Avg_Avocados,
    AVG([Apples Production (tonnes)]) AS Avg_Apples
FROM food_production
GROUP BY Entity;
```
Hasil tersebut dapat divisualisasikan dengan Tableau

