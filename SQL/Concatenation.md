```
SELECT CONCAT('afreen', ' poly');
```

gives output `afreen poly`


Hackerrank - Advanced Select - The PADS
---

Generate the following two result sets:
Query an alphabetically ordered list of all names in OCCUPATIONS, immediately followed by the first letter of each profession as a parenthetical (i.e.: enclosed in parentheses). For example: AnActorName(A), ADoctorName(D), AProfessorName(P), and ASingerName(S).
Query the number of ocurrences of each occupation in OCCUPATIONS. Sort the occurrences in ascending order, and output them in the following format:

There are a total of {occupation_count} {occupation}s.


```
SELECT CONCAT(name,'(',left(occupation,1),')') FROM occupations
ORDER BY name;


SELECT CONCAT('There are a total of ',COUNT(occupation),' ',LOWER(occupation),'s.') FROM occupations
GROUP BY occupation
ORDER BY COUNT(occupation);
```
