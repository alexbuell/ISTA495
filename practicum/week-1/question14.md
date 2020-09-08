Which countries receive the most migrants? List the name and the migrants number of the top 10.

SELECT country, migrants FROM world WHERE migrants IS NOT NULL ORDER BY REPLACE(migrants, ',', '')::integer DESC LIMIT 10 ;


"country","migrants"
"United States","954,806"
"Germany","543,822"
"Turkey","283,922"
"United Kingdom","260,650"
"Canada","242,032"
"Colombia","204,796"
"Russia","182,456"
"Uganda","168,694"
"Australia","158,246"
"Italy","148,943"
