# Question 1

You are given a table named **OCCUPATIONS**, which includes names of people and their respective occupations. You 
need to write **two SQL queries** to process and display the data in specific formats.

---

## 🔹 Query 1: Names with Occupation Initial

- Return a list of all **names**, sorted in **alphabetical order**.
- After each name, append the **first letter** of their occupation (in **uppercase**), enclosed in 
**parentheses**.

#### ✅ Expected Format:
> Alice(A)
> Bob(D)
> Charlie(P)
> Diana(S)

### 2. Second Query:

Count how many people have each occupation. Then print that information in this format:

> There are a total of [number] [occupation]s.

Use **lowercase** for the occupation name, add **"s"** at the end (plural), and **sort** the results by number 
(smallest first). If two jobs have the same number of people, **sort alphabetically by the job title**.


#### ✅ Expected Format:

>There are a total of 2 doctors.
>There are a total of 2 singers.
>There are a total of 3 actors.
>There are a total of 3 professors.`



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
