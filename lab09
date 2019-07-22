-- 1 create table for pple in department 80
create table L09SalesRep AS(
    select  employee_id as RepID,
            first_name as FName,
            last_name as LName,
            phone_number as Phone#,
            salary as Salary,
            commission_pct as Comission
    from employees
    where department_id = 80
);

-- 2.
create table L09Cust (
    CUST#       NUMBER(6),
    CUSTNAME    VARCHAR2(30),
    CITY        VARCHAR2(20),
    RATING      CHAR(1),
    COMMENTS    VARCHAR2(200),
    SALESREP#   NUMBER(7)
);

insert into L09Cust (CUST#, CUSTNAME, CITY, RATING, SALESREP#) VALUES (501, 'ABC LTD.', 'Montreal', 'C', 201);
insert into L09Cust (CUST#, CUSTNAME, CITY, RATING, SALESREP#) VALUES (502, 'Black Giant', 'Ottawa', 'B', 202);
insert into L09Cust (CUST#, CUSTNAME, CITY, RATING, SALESREP#) VALUES (503, 'Mother Goose', 'London', 'B', 202);
insert into L09Cust (CUST#, CUSTNAME, CITY, RATING, SALESREP#) VALUES (701, 'BLUE SKY LTD', 'Vancouver', 'B', 102);
insert into L09Cust (CUST#, CUSTNAME, CITY, RATING, SALESREP#) VALUES (702, 'MIKE and SAM Inc.', 'Kingston', 'A', 107);
insert into L09Cust (CUST#, CUSTNAME, CITY, RATING, SALESREP#) VALUES (703, 'RED PLANET', 'Mississauga', 'C', 107);
insert into L09Cust (CUST#, CUSTNAME, CITY, RATING, SALESREP#) VALUES (717, 'BLUE SKY LTD', 'Regina', 'D', 102);

-- 3
create table L09GoodCust as(
    select cust# as CustID,
            CUSTNAME as Name,
            CITY as Location,
            SALESREP# as RepId
            from L09Cust
            where rating in ('A', 'B')
);

-- 4
alter table L09SalesRep add JobCode VARCHAR2(12);
