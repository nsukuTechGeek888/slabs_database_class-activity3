#Author : Nsuku Shikhibana


1.  Vertical Software

Vertical Software:
Vertical software is designed for a specific industry or business.

Example: Uber is vertical software because it focuses on the transportation industry. It allows customers to book rides, drivers to accept trips, and passengers to make payments.

Horizontal Software:
Horizontal software is designed to be used in different industries.

Example: Microsoft Excel is horizontal software because it can be used by schools, banks, hospitals, and other businesses to organise information and perform calculations.

Difference:
Vertical software focuses on one specific industry, while horizontal software can be used across many industries.


2. Batch Processing vs Real-Time Processing

Batch Processing:
Batch processing is when data is collected and processed together at a scheduled time.

Example: A company processes employee salaries at the end of every month.

Real-Time Processing:
Real-time processing is when data is processed immediately or within a required time limit.

Example: An ATM processes a withdrawal when a customer requests money.

Difference:
Batch processing handles data in groups, while real-time processing handles data as events happen.


3. company_db=# INSERT INTO employees (name, position, salary)
company_db-# VALUES
company_db-# ('Nsuku', 'Manager', 25000),
company_db-# ('Lemart', 'Developer', 18000),
company_db-# ('Kwando', 'Technician', 12000);
INSERT 0 3
company_db=# SELECT * FROM employees;
 id |  name  |  position  |  salary
----+--------+------------+----------
  1 | Nsuku  | Manager    | 25000.00
  2 | Lemart | Developer  | 18000.00
  3 | Kwando | Technician | 12000.00
(3 rows)


company_db=# SELECT * FROM employees
company_db-# WHERE salary > 15000;
 id |  name  | position  |  salary
----+--------+-----------+----------
  1 | Nsuku  | Manager   | 25000.00
  2 | Lemart | Developer | 18000.00
(2 rows)


company_db=# UPDATE employees
company_db-# SET salary = 20000
company_db-# WHERE id = 2;
UPDATE 1
company_db=# SELECT * FROM employees;
 id |  name  |  position  |  salary
----+--------+------------+----------
  1 | Nsuku  | Manager    | 25000.00
  3 | Kwando | Technician | 12000.00
  2 | Lemart | Developer  | 20000.00
(3 rows)


company_db=# DELETE FROM employees
company_db-# WHERE id = 3;
DELETE 1
company_db=# SELECT * FROM employees;
 id |  name  | position  |  salary
----+--------+-----------+----------
  1 | Nsuku  | Manager   | 25000.00
  2 | Lemart | Developer | 20000.00
(2 rows)

