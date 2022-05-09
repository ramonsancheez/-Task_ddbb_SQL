# -Task_ddbb_SQL

### TASK 1
The flight with number 222 has suffered a delay.
Change its Dia to 15/10/2009:
```mysql
UPDATE vol SET dia = "2009/10/15" WHERE NumVol = 222;
```
<img width="764" alt="image" src="https://user-images.githubusercontent.com/91556453/167422999-96b0ffb5-992b-4550-9135-ccff041f6ed9.png">


### TASK 2
The plane for flight 999 has been changed, the new one has 128 seats and is from the company Air France.
Set its new values:
```mysql
UPDATE vol SET Capacitat = 128, NomCo = "Air France" WHERE NumVol = 999;
```
<img width="753" alt="image" src="https://user-images.githubusercontent.com/91556453/167423519-f49667b0-9808-4159-b5c4-7fb275137def.png">


### TASK 3
Flight 666 has been canceled.
Remove it from the database:
```mysql
DELETE FROM vol WHERE NumVol = 666;
```
<img width="746" alt="image" src="https://user-images.githubusercontent.com/91556453/167423906-39a77e04-f211-43f6-9f96-a85f6cc5e2f1.png">

### TASK 4
The user with ID Z23456K has asked us to remove all of it's data.
Remove the user from the database:
```mysql
DELETE FROM passatger WHERE ID = "Z23456K";
```
<img width="501" alt="image" src="https://user-images.githubusercontent.com/91556453/167424394-bbfc02f2-a69c-43c7-907a-e5b60a8ff8ba.png">

### TASK 5
Using a subquery.
Find all cities with flight departures from the company Iberia:
```myqsl
SELECT Ciutat FROM Aeroport WHERE NomAeroport IN (SELECT NomAerOrigen FROM Vol WHERE NomCo = "Iberia");
```
<img width="281" alt="image" src="https://user-images.githubusercontent.com/91556453/167425118-756620be-0b97-4345-a343-086da31a77a3.png">



### TASK 6
Using a subquery.
Find the maximum amount of arrivals in a single airport.
```mysql

```
