# SQL-Practise

1. This below Query to retrieve the city,(min & max) length of city from the station table.

    select * from (select city,length(city) as citylen from station order by citylen, city) where rownum =1;
    select * from (select city,length(city) as citylen from station order by citylen desc, city) where rownum =1;
    
2. Query the list of CITY names starting with vowels (i.e., a, e, i, o, or u) from STATION. Your result cannot contain duplicates.

    select DISTINCT  city from station where city like 'A%' OR city like 'E%' OR  city like 'I%' OR city like 'O%' OR city like 'U%';
