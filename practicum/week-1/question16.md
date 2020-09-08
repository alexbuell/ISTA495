Which country has the highest medium age and lowest fertility rate?

SELECT country, fertility from world WHERE fertility = (SELECT MIN(fertility) FROM world)

"country","fertility"
"South Korea","1.1"

SELECT country, medianage from world WHERE medianage = (SELECT MAX(medianage) FROM world WHERE NOT medianage = 'N.A.')

"country","medianage"
"Japan","48"