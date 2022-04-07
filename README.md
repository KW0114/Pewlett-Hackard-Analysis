# Employee Database Analysis

## Overview and Purpose

This analysis was performed on a database of multiple tables outlining the employees of Pewlett
Hackard. The goal was to gain more insight into how many employees from each department would be 
retiring soon, so that the company can put together a game plan for covering the absences.

## Results

### Database Design

I started out by creating an ERD to get a clearer picture of what I would be working with regarding
the tables I was provided with. I identified the primary and foreign keys from each table and 
used QuickDBD to map out the database for later use.

![screenshot]()


### Retirement Tables

The company was interested in the employees who were born between 1952 and 1955, who also are currently
active as employees. These are the employees who are most likely going to retire soon, and will need
to be replaced. 

* The original table included many duplicates of the same employee, since some of them were promoted
to new job titles during the course of their employment.

![duplicates screenshot](https://github.com/KW0114/Pewlett-Hackard-Analysis/blob/08d9bfdbac8300ab2b19de6347f3fdf43db62af8/Analysis%20screenshots/duplicate%20titles.png)

* As you scroll the file, you can see there is a shockingly large amount of employees
in this category, so we needed to group the employees by job title to get a better idea of the data.

![unique_titles](https://github.com/KW0114/Pewlett-Hackard-Analysis/blob/08d9bfdbac8300ab2b19de6347f3fdf43db62af8/Analysis%20screenshots/unique_titles_tail.png)

Here is the grouped table:

![retiring_titles](https://github.com/KW0114/Pewlett-Hackard-Analysis/blob/08d9bfdbac8300ab2b19de6347f3fdf43db62af8/Analysis%20screenshots/retiring_titles.png)

* From the table, it looks like there will be quite a lot of senior staff retiring (Senior Engineer
or Senior Staff). The company will most likely not be able to hire enough employees from the outside
to fill these roles, since they will need extensive knowledge about procedures at the company. They
will need to make lots of promotions, and hire for the lower level positions. I'm sure employees would
be much happier this way, since they have been working there for years!
Luckily not many managers will be retiring, so they will have lots of help hiring and training
the new employees!


### Mentorhsip Eligibility

On the other side of the spectrum, we took a look at the employees who were born in 1965. The company
deemed these employees eligible for the mentorship program. I made a new table of those employees
along with their birth dates, employment dates, and job titles.

![mentorship_eligibility](https://github.com/KW0114/Pewlett-Hackard-Analysis/blob/77f759dc85fa122ebda3148404472babe38b5ed7/Analysis%20screenshots/mentorship%20screenshot.png) 

* There seem to be a lot of senior level staff in this mentorship group, so I think these would be
great mentors for the new employees.


## Summary

The following tables show a count of reitirng employees from 1952 and 1953:


![born in 1952 only](https://github.com/KW0114/Pewlett-Hackard-Analysis/blob/f24ee62870f5c0fca72fceef81ba9355dd3b9302/Analysis%20screenshots/born_in_1952.png)


![born in 1952 AND 1953](https://github.com/KW0114/Pewlett-Hackard-Analysis/blob/f24ee62870f5c0fca72fceef81ba9355dd3b9302/Analysis%20screenshots/born_1952_to_1953.png)



* Looking at the two queries above, the number of employees born in 1952 alone is more comparable
to the available amount of employees needed to become mentors. So if the company focuses mainly on 
the most pressing vacancies, they will be alright for a little while. 

* Once I include those born in 1953 though, that's when the number starts to skyrocket. So they will
not have much time before the vacancies start to pile up.






