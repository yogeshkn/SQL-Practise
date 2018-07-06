# SQL-Practise

1. This below Query to retrieve the city,(min & max) length of city from the station table.

    select * from (select city,length(city) as citylen from station order by citylen, city) where rownum =1;
    select * from (select city,length(city) as citylen from station order by citylen desc, city) where rownum =1;
    
2. 
