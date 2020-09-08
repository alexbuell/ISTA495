Wich countries send the most migrants? List the top 10.

SELECT country FROM world WHERE migrants IS NOT NULL ORDER BY REPLACE(migrants, ',', '')::integer DESC LIMIT 10 ;

"country"
"United States"
"Germany"
"Turkey"
"United Kingdom"
"Canada"
"Colombia"
"Russia"
"Uganda"
"Australia"
"Italy"