# core-practise
1. Write a SQL statement that displays all the information given in the table

         _id |    name    |   city   | commission 
-------------+------------+----------+------------
        5001 | James Hoog | New York |       0.15
        5002 | Nail Knite | Paris    |       0.13
        5005 | Pit Alex   | London   |       0.11
        5006 | Mc Lyon    | Paris    |       0.14
        5007 | Paul Adam  | Rome     |       0.13
        5003 | Lauson Hen | San Jose |       0.12

answer:
create  table EMPLOYEE( id int not null primary key,name text not null,city text not null,commission int not null);

  INSERT INTO EMPLOYEE VALUES(5001,"James Hoog","New York", 0.15);
  INSERT INTO EMPLOYEE VALUES(5002,"Nail Knite", "Paris", 0.13);
  INSERT INTO EMPLOYEE VALUES(5005,"Pit Alex","London",0.11);
  INSERT INTO EMPLOYEE VALUES(5006, "Mc Lyon","Paris",0.14);
  INSERT INTO EMPLOYEE VALUES(5007,"Paul Adam","Rome", 0.13);
  INSERT INTO EMPLOYEE VALUES(5003,"Lauson Hen","San Jose",0.12);
 
SELECT * FROM EMPLOYEE;
2.Write a SQL statement to display a string "This is SQL Exercise, Practice and Solution"
SELECT "This is SQL Exercise, Practice and Solution";

3.Write a SQL query to display three numbers in three columns.
select 5001,50002,5004;
4. Write a SQL statement to display specific columns such as names and commissions for all the id's

         _id |    name    |   city   | commission 
-------------+------------+----------+------------
        5001 | James Hoog | New York |       0.15
        5002 | Nail Knite | Paris    |       0.13
        5005 | Pit Alex   | London   |       0.11
        5006 | Mc Lyon    | Paris    |       0.14
        5007 | Paul Adam  | Rome     |       0.13
        5003 | Lauson Hen | San Jose |       0.12


SELECT name,commission FROM EMPLOYEE;
5.Write a query to display the columns in a specific order, such as order date, salesman ID, order number, and purchase amount for all orders.

ord_no      purch_amt   ord_date    customer_id  salesman_id
----------  ----------  ----------  -----------  -----------
70001       150.5       2012-10-05  3005         5002
70009       270.65      2012-09-10  3001         5005
70002       65.26       2012-10-05  3002         5001
70004       110.5       2012-08-17  3009         5003
70007       948.5       2012-09-10  3005         5002
70005       2400.6      2012-07-27  3007         5001
70008       5760        2012-09-10  3002         5001
70010       1983.43     2012-10-10  3004         5006
70003       2480.4      2012-10-10  3009         5003
70012       250.45      2012-06-27  3008         5002
70011       75.29       2012-08-17  3003         5007
70013       3045.6      2012-04-25  3002         5001


SELECT ord_date, salesman_id, ord_no, purch_amt FROM orders;
