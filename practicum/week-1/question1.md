1. Download and install PostgreSQL database (it is available at https://www.postgresql.org)
2. Create a database and name it as ISTA495.practicum
3. Ctreat the following table:
  - table name: world
  - table columns: id, country, population, area, migrants,fertility,medianage,urbanpopulation(id is a number, everything else is a string). 
4. Populate the world table using the csv file included in this folder

Hint:

* [How to import CSV file into PostgreSQL table](https://www.postgresqltutorial.com/import-csv-file-into-posgresql-table/)

* [How to import a selected number of the columns of a csv file](https://stackoverflow.com/questions/12618232/copy-a-few-of-the-columns-of-a-csv-file-into-a-table/49906327)

CREATE TABLE public.world
(
    id integer,
    country text COLLATE pg_catalog."default",
    population text COLLATE pg_catalog."default",
    area text COLLATE pg_catalog."default",
    migrants text COLLATE pg_catalog."default",
    fertility text COLLATE pg_catalog."default",
    medianage text COLLATE pg_catalog."default",
    urbanpopulation text COLLATE pg_catalog."default"
)

TABLESPACE pg_default;

ALTER TABLE public.world
    OWNER to postgres;