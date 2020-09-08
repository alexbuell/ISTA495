Write a SQL solution to output the population of the world.

SELECT SUM(REPLACE(population, ',', '')::integer) as total_population
FROM world;


total_population
7794798739
