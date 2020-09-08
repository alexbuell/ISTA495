Write a SQL solution to output the land share value of the wold (that is, the sum of the land area divided by the sum of the population).

SELECT (SUM(CAST(REPLACE(area, ',','')::integer AS float))/SUM(CAST(REPLACE(population, ',', '')::integer AS float)))AS land_share FROM world;

"land_share"
0.01668985785984384