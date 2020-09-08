Which countries have a low population density, low fertility rate and hig migrants? List the top 10. 

CREATE TABLE temp_table_prob17 (country text, population_density FLOAT, fertility FLOAT, migrants integer);

INSERT INTO temp_table_prob17(country,population_density, fertility, migrants)
SELECT country,(CAST(REPLACE(population, ',', '')::integer AS FLOAT)/CAST(REPLACE(area, ',', '')::integer AS FLOAT)), fertility::float, REPLACE(migrants, ',', '')::integer FROM world WHERE REPLACE(area, ',', '')::integer >0 AND NOT fertility = 'N.A.';