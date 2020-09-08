Write a SQL solution to output the 10 countries who have the highest land share.

#COMMENT: I get duplicate values and couldn't figure out why!!

CREATE TABLE temp_1 (country text,
land_area FLOAT)

INSERT INTO temp_1(country,land_area)
SELECT country,(CAST(REPLACE(area, ',', '')::integer AS FLOAT)/CAST(REPLACE(population, ',', '')::integer AS FLOAT)) FROM world

SELECT country FROM temp_1 ORDER BY land_area DESC LIMIT 10