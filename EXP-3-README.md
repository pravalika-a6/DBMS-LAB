# DBMS-LAB
DROP DATABASE IF EXISTS 19WH1A12A6;

CREATE SCHEMA 19WH1A12A6;

USE 19WH1A12A6;

CREATE TABLE Busb(bus_no VARCHAR(20),Sourc VARCHAR(20),destination VARCHAR(20),bcolour VARCHAR(20));

INSERT INTO Busb VALUES('TS123','hyderabad','banglore','blue');

INSERT INTO Busb VALUES('TS124','hyderabad','vizag','red');

INSERT INTO Busb VALUES('TS125','banglore','rajahmandry','blue');

INSERT INTO Busb VALUES('TS126','vizag','guntur','blue');

INSERT INTO Busb VALUES('TS127','vijayawada','tirupati','green');

SELECT * FROM Busb;

DELETE FROM Busb B WHERE B.Sourc='hyderabad';

SELECT * FROM Busb;

CREATE TABLE Passenger(p_name VARCHAR(20),p_id INT,gender VARCHAR(20),age INT,p_destination VARCHAR(20));

INSERT INTO Passenger VALUES('Raju',1234,'male',28,'hyderabad');

INSERT INTO Passenger VALUES('Ravi',1235,'male',50,'tirupati');

INSERT INTO Passenger VALUES('Rani',1238,'female',20,'hyderabad');

INSERT INTO Passenger VALUES('Ravali',1267,'female',48,'varanasi');

INSERT INTO Passenger VALUES('soumya',1294,'female',24,'hyderabad');

INSERT INTO Passenger VALUES('sanju',1204,'female',28,'banglore');

INSERT INTO Passenger VALUES('Raghu',1284,'male',47,'guntur');

SELECT * FROM Passenger;

DELETE FROM Passenger P WHERE p.age=50;

SELECT * FROM Passenger;

CREATE TABLE ticket(t_id INT,t_cost INT,destination VARCHAR(20),seatno VARCHAR(20));

INSERT INTO ticket VALUES(1234,234,'vizag','L12');

INSERT INTO ticket VALUES(1237,568,'hyderabad','R19');

INSERT INTO ticket VALUES(1294,894,'banglore','L21');

INSERT INTO ticket VALUES(1256,765,'karnataka','L17');

INSERT INTO ticket VALUES(1284,567,'varanasi','R12');

SELECT * FROM ticket;

DELETE FROM ticket T WHERE t_id=1234;

SELECT * FROM ticket;

ALTER TABLE ticket ADD COLUMN seats INT;

SELECT * FROM ticket;
