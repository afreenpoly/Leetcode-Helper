```
SELECT LEFT('SQL DATA', 1)
```
This gives the output `'S'`

This can be used to select the STARTING character of a string

```
SELECT LEFT('SQL DATA', 3)
```
This gives the output `'SQL'`

```
SELECT RIGHT('SQL DATA', 1)
```
This gives the output `'A'`

This can be used to select the LAST character of a string



Hackerrank - Basic Select - Weather Observation Station 9
---



Query the list of CITY names from STATION that do not start with vowels. Your result cannot contain duplicates.  
```
select distinct city from station
where left(city,1) not in('a','e','i','o','u');
```
