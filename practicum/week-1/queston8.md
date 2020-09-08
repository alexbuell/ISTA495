Write a SQL solution to output the population density of the world. That is, the sum of the population 
of all the countries divided by the sum of the land area of all the countries. 

SELECT (SUM(CAST(REPLACE(population, ',','')::integer AS float))/SUM(CAST(REPLACE(area, ',', '')::integer AS float)))AS world_population_density FROM world;

"world_population_density"
59.91662771472858