# Group-2-MIST-4610-Project-1
# Team Name 
21482 Group 2
# Team Members 
Rohan Patel [@rohpat](https://github.com/rohpat)  <br>
Grace Okpurukre  [@graceokpurukre](https://github.com/graceokpurukre) <br>
Lindsey Isenberg [@lindseyisenberg](https://github.com/lindseyisenberg)  <br>
Catherine Repke  [@catherinerepke](https://github.com/catherinerepke) <br> 
Ore Pratt [@nathanp2020](https://github.com/nathanp2020) <br> 
# Problem Description:
Our aim is to build a database for a soccer club through multiple entities with relationships such as many-to-many, recursive, and one to many. The club entity is the heart of our operations as it holds many of the relationships between players, coaches, teams, equipment, etc. Our project displays the relationships between the different entities along with a database that holds information about our operations. Finally, we have written queries that are useful in finding important information about the club.

# Data Model 
Our model displays a database for a Soccer Club. The heart of the operations is the club, which holds information about the name, 
coaches, email, and location. Connected to the club through a one to many relationship is the players table, 
which holds the playerID as the primary key and attributes such as their name and team. 

Next, parents are connected to the players entity through a one to many relationship since parents can have many players 
but a player only belongs to one parent. The soccer club needs information about parents such as their name and 
contact information. Parents also pay the club for their students to participate, which is shown by the one to many 
relationship between parents and financial transactions. Information about transactions needs to be stored such as the fees and amount.

The club also takes donations, so it needs to keep track of the amount and sponsorID. A sponsor can make many donations, 
but a donation can only belong to one sponsor. Also connected to the players table is the Age Division table where one 
age division can have multiple players, and a player can belong to one age division. This entity includes the divisionID, team type,
and location. Also connected to the club entity is the coaches entity, which holds information about coachID, name, and the team they manage.

Coaches can also offer training sessions, which is depicted through a one to many relationship since one coach can have many training sessions 
and a training session is led by one coach. Information about the training sessions is documented such as sessionID, location, the coach that 
leads the session, and the division. Coaches are also connected to players, as a coach can coach many players at one time. 
The next offshoot of our club entity is the executives entity, which is also connected through a many to many relationship. It contains information such 
as their names and contact information. However, this entity also contains a 1:1 recursive relationship. There are club executives that 
manage the entire organization, but also league administrators for each division. Executives can also be league administrators, 
which is shown by the non-identifying 1:1 recursive relationship labeled as “league administrators.”

Next is the equipment table, which houses information such as the equipmentID, type, date of rental, and date returned.
A one to many relationship is formed because one club has many pieces of equipment, and equipment belongs to one club. 
The last entity directly connected to the club is the tournaments entity, which stores information about the tournament name and location. 
Tournaments are housed in facilities, which is shown through a 1:1 relationship since a tournament can be in one facility and a facility can 
only house one tournament at a time as per the club’s rules. This data model allows the soccer club to effectively store all of its information, 
providing a seamless experience for coaches, teams, and players.


<img width="838" alt="image" src="https://github.com/nathanp2020/SP24-MIST4610-Group-2-Project-1/assets/163202597/6ec17357-d417-485b-91fc-1edb1aa46bad">



# Data Dictionary 
<h2> Age Division Table </h2>

<img width="499" alt="image" src="https://github.com/nathanp2020/SP24-MIST4610-Group-2-Project-1/assets/163202597/c8f0af48-5c0a-4a91-84fd-ffe4f66610ea">

<h2> Club Table </h2>

<img width="455" alt="image" src="https://github.com/nathanp2020/SP24-MIST4610-Group-2-Project-1/assets/163202597/ec2987ad-2d46-4442-9525-b4773ddc4474">

<h2> Coaches Table </h2>

<img width="499" alt="image" src="https://github.com/nathanp2020/SP24-MIST4610-Group-2-Project-1/assets/163202597/f7dd3664-879f-4b91-a6a5-5b6a11406b56">

<h2> Executives Table </h2>

<img width="498" alt="image" src="https://github.com/nathanp2020/SP24-MIST4610-Group-2-Project-1/assets/163202597/4543b83d-3aa5-4206-9ad9-caf9e5d9dff4">

<h2> Equipment Table </h2>

<img width="499" alt="image" src="https://github.com/nathanp2020/SP24-MIST4610-Group-2-Project-1/assets/163202597/2f8f5041-18d1-4004-ac76-9873edff6284">

<h2> Facilities Table </h2>

<img width="500" alt="image" src="https://github.com/nathanp2020/SP24-MIST4610-Group-2-Project-1/assets/163202597/8f7d1a0f-8c98-43ea-bfc9-9722318e1550">

<h2> Financial Transactions Table </h2>

<img width="503" alt="image" src="https://github.com/nathanp2020/SP24-MIST4610-Group-2-Project-1/assets/163202597/d67440d6-2756-49ab-b808-0f08fecdfe9c">

<h2> Parents Table </h2>

<img width="502" alt="image" src="https://github.com/nathanp2020/SP24-MIST4610-Group-2-Project-1/assets/163202597/2350d81a-2d4b-494b-a85a-5d748095a3a3">

<h2> Players Table </h2>

<img width="498" alt="image" src="https://github.com/nathanp2020/SP24-MIST4610-Group-2-Project-1/assets/163202597/4db31ca9-4528-4754-aea6-79a5c5aa548d">

<h2> Sponsors/Donors Table </h2>

<img width="503" alt="image" src="https://github.com/nathanp2020/SP24-MIST4610-Group-2-Project-1/assets/163202597/30d5aac5-668f-4401-8e39-9b390af57d4b">

<h2> Tournaments Table </h2>

<img width="501" alt="image" src="https://github.com/nathanp2020/SP24-MIST4610-Group-2-Project-1/assets/163202597/9b699ff5-944a-4e1c-ae4a-f0c3f9ad1659">

<h2> Training Sessions Table </h2>

<img width="500" alt="image" src="https://github.com/nathanp2020/SP24-MIST4610-Group-2-Project-1/assets/163202597/08410e7b-7a35-436c-b5d1-16895b503437">










# Queries 


![Screenshot (269)](https://github.com/nathanp2020/SP24-MIST4610-Group-2-Project-1/assets/148779254/5c7b27ca-f66f-4a9d-b7d2-13492e0257bc)


<h2>Query 1</h2>
1. List the coach’s name and the names of the players they coach. Order by name (descending).

![image](https://github.com/nathanp2020/SP24-MIST4610-Group-2-Project-1/assets/148779254/78b0ab4c-aef9-4570-91e8-92fc92708ae7)


The SQL query to list the coach's name and the names of the players they coach is useful for various reasons, especially in the context of sports management or team organization. It provides valuable insights into the coaching relationships within a sports team or organization. Listing by descending employee name allows a manager to quickly view coaches in alphabetical order and the players under them.


<h2>Query 2</h2>
2. List the maximum transaction amount and the parent who made the transaction.

![image](https://github.com/nathanp2020/SP24-MIST4610-Group-2-Project-1/assets/148779254/63d742a1-89a9-44d2-b5aa-b828aebbb022)


This SQL query finds the parent who made the largest transaction and provides their name. A manager can use this information to identify their highest-spending parent donors.


<h2>Query 3</h2>
3. Find the capacity of each facility for where the tournaments are being held. Order the results by capacity in descending order.

![image](https://github.com/nathanp2020/SP24-MIST4610-Group-2-Project-1/assets/148779254/3a5f7189-3615-4449-aaf4-2cbb21b1e588)



This SQL query retrieves information about tournaments along with the corresponding facility information and its capacity. This information is valuable for tournament managers who need to know the capacity of their facilities and the city in which the tournament is being held.

<h2>Query 4</h2>
4. List the coaches for each club and their contact information

![image](https://github.com/nathanp2020/SP24-MIST4610-Group-2-Project-1/assets/148779254/e8bd7be4-431c-43ab-a272-734f2e83149e)



This SQL query retrieves a list of the coaches and their email. This query is useful for anyone interested in the leadership of the clubs in the league, and gives them contact information should they want to reach out.

<h2>Query 5</h2>
5. List the parents who have players in both the college and professional age divisions by alphabetical order.

![image](https://github.com/nathanp2020/SP24-MIST4610-Group-2-Project-1/assets/148779254/ee40d066-55df-4d9f-bacc-b6181b1979f0)



This SQL query retrieves a list of parents who have players in both the college and professional age divisions. It provides a clear view of which players have players in both. This information is valuable for recognizing what parents identify with which kids.

<h2>Query 6</h2>
6. List the sponsors who have made donations over $5000 and the teams they are sponsors for, sort by descending amount.

![image](https://github.com/nathanp2020/SP24-MIST4610-Group-2-Project-1/assets/148779254/59daf8b7-b80d-43bc-b5db-9908bb4bb23f)


This SQL query retrieves a list of sponsors, their associated teams, and the sponsorship payment amounts. It provides a clear view of sponsors contributing significant amounts (exceeding $1000) to specific teams. This information is valuable for recognizing and nurturing key sponsor relationships, evaluating the financial impact of sponsorships, and determining which teams have attracted substantial sponsor support. Managers can use these insights to develop targeted strategies for engaging and retaining high-value sponsors, contributing to the financial health and success of their teams or organization.

<h2>Query 7</h2>
7. List all coaches who are associated with clubs that have a specific type of equipment, such as 'shoes’.

![image](https://github.com/nathanp2020/SP24-MIST4610-Group-2-Project-1/assets/148779254/0b867aa0-8131-4dc2-8d8a-49877ca15410)


This query retrieves a list of financial transactions as well as the player name associated with each transaction record. It also provides transparency regarding financial transactions involving players, aiding in financial management and accountability.

<h2>Query 8</h2>
8. Find all jerseys rented in 2024 and group them by club name.

![image](https://github.com/nathanp2020/SP24-MIST4610-Group-2-Project-1/assets/148779254/25c652d2-3107-4116-b823-f20b33465b82)

This query finds all jerseys rented out in 2024, and groups them by the club name. This query will be useful for league managers in terms of keeping track of equipment and seeing when their highest equipment usage times are.


<h2>Query 9</h2>
9. List the parents names of players who are sponsored by Adidas and also pay fees over $8000.

![image](https://github.com/nathanp2020/SP24-MIST4610-Group-2-Project-1/assets/148779254/89427330-778e-4bb6-a057-13fbe3fb4585)


This query generates a list of players' parents who pay over 8000 dollars in fees and whose child is also sponsored by Adidas.  This query is useful for knowing which players' families pay higher fees and can help the club forecast and manage its finances more effectively and which companies are sponsoring these players. 

<h2>Query 10</h2>
10. List the players and coaches whose training sessions are located in the AL East. 

![image](https://github.com/nathanp2020/SP24-MIST4610-Group-2-Project-1/assets/148779254/f7b71cd2-300d-47d1-96bb-f5018d7af4df)


This query would generate a list of teams that have training sessions located on the East Coast. This information would allow teams and players to stay up to date on team training schedules and where each team hosts their training sessions.

# Database Information

The name of the database on the mySQL server is: al_Group_21482_G2

Each query listed above is marked in the database using stored procedures which can be called using the following format: "CALL TP_Q1();", "CALL TP_Q2();", "CALL TP_Q3();"
and so forth.













