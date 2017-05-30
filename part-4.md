Find the author with the name 'Kara Melton' and then select all the articles she has written.

SELECT id from authors where name = 'Kara Melton';
SELECT title FROM articles where author_id=8;

Find Ontario in the provinces table and then find all the cities in that province.
SELECT * from cities where province_id = 14;

Who wrote the article called 'Coding Bootcamps and Emotional Labor'?
SELECT * from articles where title = 'Coding Bootcamps and Emotional Labor';

Who wrote the article called 'Coding Bootcamps and Emotional Labor'?

SELECT author_id FROM articles WHERE title=‘Coding Bootcamps and Emtional Labor’;
SELECT name FROM authors WHERE id=4;


Write a series of SQL queries to find out how many provinces are in Canada.
SELECT * FROM countries WHERE name = 'Canada';
SELECT * FROM provinces where country_id=1;
SELECT COUNT(name) FROM provinces WHERE country_id=1;

How many people live at 4740 McDermott Street?
select * from residences where address ='4740 McDermott Street';
SELECT * from persons where residence_id=9;
SELECT COUNT(name) from persons where residence_id=9;

What city is 4740 McDermott Street in?
select * from residences where address ='4740 McDermott Street'
Select * from cities where id=11;
or
Select * from cities where id in(Select city_id from residences where address='4740 McDermott Street');

What province is 4740 McDermott Street in?
select * from residences where address ='4740 McDermott Street'
Select * from provinces where id=14;

What country is 4740 McDermott Street in?
SELECT * from cities where id=11;
SELECT * from provinces where id=14;
select * from countries where id=1;

Find the person named 'Destini Davis' and then use a series of SQL queries to find what country they live in.
Select * from persons where name='Destini Davis'
Select * from residences where id=2;
Select * from cities where id=8;
Select * from provinces where id=14;
Select * from countries where id=1;


How many articles has Aditya Mukerjee written?
