Write a SQL solution to output the 10 least dense countries.

CREATE TABLE temp_table_density (country text,
population_density FLOAT)

INSERT INTO temp_table_density(country,population_density)
SELECT country,(CAST(REPLACE(population, ',', '')::integer AS FLOAT)/CAST(REPLACE(area, ',', '')::integer AS FLOAT)) FROM world WHERE REPLACE(area, ',', '')::integer >0;

SELECT country FROM temp_table_density ORDER BY population_density ASC LIMIT 10



"country"
"Greenland"
"Falkland Islands"
"Mongolia"
"Western Sahara"
"Namibia"
"Australia"
"Iceland"
"French Guiana"
"Suriname"
"Libya"