# hackerrankhw2
11.	select DISTINCT(city) from station where REGEXP_LIKE(city,'[aeiou]$', 'i');
12.	select DISTINCT(city) from station where CITY RLIKE '^[aeiouAEIOU].*[aeiouAEIOU]$';
13.	select distinct city from station  
where city Not like 'A%' and city Not like 'E%' and city Not like 'I%' and
 city Not like 'o%' and city not like 'U%';
14.	select distinct city from station where city not like '%a'and city not like '%e'and city not like '%i'and city not like '%o'and city not like '%u';
15.	select distinct city from station where (city not like'a%' and city not like'e%' and city not like'i%' and city not like'o%' and city not like'u%') or (city not like'%a' and city not like'%e' and city not like'%i' and city not like'%o' and city not like'%u' );
16.	SELECT DISTINCT CITY FROM STATION WHERE CITY REGEXP '^[^aeiou].*[^aeiou]$';
17.	select name from students where marks>75 order by right(name,3), id asc;
18.	select name from employee order by name;
19.	select name from employee where months<10 and salary>2000 order by employee_id;
20.	select s.name, g.grade, s.marks from students s, grades g where g.grade>=8 and s.marks between g.min_mark and g.max_mark order by g.grade desc, s.name;
select 'NULL', g.grade, s.marks from students s, grades g where g.grade<8 and s.marks between g.min_mark and g.max_mark order by g.grade desc, s.marks;
