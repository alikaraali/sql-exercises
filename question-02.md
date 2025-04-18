# Question 2

Transform the **OCCUPATIONS** table by pivoting the Occupation column, so that each occupation becomes its own 
column. 
The final output should have four columns in this exact order: Doctor, Professor, Singer, and Actor.

Each column should list the names of individuals with that occupation, sorted in alphabetical order. Align the 
names row by row so that the first row shows the first name for each occupation, the second row shows the second 
name for each occupation, and so on.

If a particular row has no name for a given occupation, display **NULL** in that cell.


## 🔹 OCCUPATIONS table
The following table can be used to solve the problem. 

``` sql
-- Create the OCCUPATIONS table
CREATE TABLE OCCUPATIONS (
    Name VARCHAR(100),
    Occupation VARCHAR(100)
);

-- Insert data into OCCUPATIONS
INSERT INTO OCCUPATIONS (Name, Occupation) VALUES
('Ashley', 'Professor'),
('Samantha', 'Actor'),
('Julia', 'Doctor'),
('Britney', 'Professor'),
('Maria', 'Professor'),
('Meera', 'Professor'),
('Priya', 'Doctor'),
('Priyanka', 'Professor'),
('Jennifer', 'Actor'),
('Ketty', 'Actor'),
('Belvet', 'Professor'),
('Naomi', 'Professor'),
('Jane', 'Singer'),
('Jenny', 'Singer'),
('Kristeen', 'Singer'),
('Christeen', 'Singer'),
('Eve', 'Actor'),
('Aamina', 'Doctor');
``` 


## ✅ OCCUPATIONS table

The solution should be as follows:

``` sql
Aamina Ashley Christeen Eve
Julia Belvet Jane Jennifer
Priya Britney Jenny Ketty
NULL Maria Kristeen Samantha
NULL Meera NULL NULL
NULL Naomi NULL NULL
NULL Priyanka NULL NULL
```

