## Project Name: Summer Olympics Analysis
- Analysis using SQL and data available in MySql database.
- Sports goes into entertainment category as far as viewers are concerned.
- Olympic athletes are considered as benchmarks in regards with their Strength, Agility and Intelligence.

### Project goal:
- To explore a dataset available in MySql database on the modern Summer Olympic Games - Athens data from 1896 to Rio 2016.
- In this project, I investigate on the results and understand trends of Olympics results using SQL.
- I will use SQL and MySql connector to fetch data from database and perform analysis and answer some common questions on the Summer Olympics.

### Dataset:
- Dataset have records at an individual Athlete competing in an individual Olympic events. 
- Columns as Name, Age, Medal_Won, Game, Year, and so on.

### Using summer olympics dataset we try to find out following questions answer:

- Find the oldest year of Olympics and and find out count of sports played in that year ?
- Find the latest year of olympics and and find count of countries played in that year ?
- Which year saw the highest and lowest no of countries participating in olympics?
- Which nation has participated in all of the olympic games?
- Identify the sport which was played in all summer olympics? 
- Which Sports were just played only once in the olympics?
- Fetch oldest athletes olympic year to win a gold medal?
- Fetch the top 5 athletes who have won the most medals (gold/silver/bronze)?
- Fetch the top 5 most successful countries in olympics. Success is defined by no of medals won?
- In which Sport/event, India has won highest medal?
- List top 15 down total gold, silver and bronze medals won by each country corresponding to each olympic games?

 ### Phase 1: Data Collection
- ##### We are using two tables which are available at MySQL database:
 - **olympics_history** table where each row corresponds to an individual athlete competing in an individual Olympic event.
 - **olympics_history_noc_regions** contains NOC(National Olympic Committee  a 3-letter code) which helps us to add country information and its corresponding region from its NOC code.

 ### Phase 2: Data Understanding
 - #### olympics_history table

1. Id:
    - Represents unique number for each athlete.
2. Name:
    - Represents name of the athlete.
3. Sex:
    - Represents sex of athlete.
    - M for Male ,F for female
4. Age:
    - Represents age of an athlete 
5. Height:
    - Represents height of an athlete in cm.
    - It has 51402 null values.
6. Weight:
    - Represents Weight of an athlete in kg.
    - It has 54074 null values.
7. Team:
    - Represents for which team an athelete was playing.
8. NOC:
    - Represents National Olympic Committee which is 3-letter code.
9. Games:
    - Represents year and season olympic games was hosted.
10. Year:
    - Represnts for which year olympic games was hosted.
11. Season:
    - reprsents for which season olympic games was hosted.
12. City:
    - Represents host city for respective olympic games.
13. Sport:
    - Represents Sport played by each athlete in olympic games.
14. Event:
    - Represents event name with respect to each game.
15. Medal:
    - Represents  type of medal won by each athlete.
    - It contains gold, silver,bronze medals.
    - NA represents no medal won by the athlete.
    - There are 222153 null values.
   
#### olympics_history_noc_regions table
1. NOC:
 - Represents National Olympic Committee which is 3-letter code.
2. region:
  - Represents in which region olympic games was hosted.
3. notes:
 - Represents some additional notes with respect to every region.

### Phase 3: Data Analysis
#### Q.1 Find the oldest year of Olympics and and find out count of sports played in that year?
- Found that oldest year of olympics is is **1896**.
- Gymnastics has highest number of participation i.e **73** in the year 1896.
  <img width="1000" alt="Screenshot 2023-08-21 at 15 32 49" src="https://github.com/kirandhasade/Olympics_Sql_Project/assets/127043120/bb7bc354-c0f4-49a1-8271-b3c6454be553">

#### Q.2 Find the latest year of olympics and and find count of countries played in that year?
- Found that latest year of Olympics is 2016.
- Athletics has highest number of participation i.e. **2507** in the year 2016.
<img width="997" alt="Screenshot 2023-08-21 at 15 34 36" src="https://github.com/kirandhasade/Olympics_Sql_Project/assets/127043120/d99cd12c-4937-49ac-9f21-f9bdaebceb9a">

#### Q.3 Which year saw the highest and lowest no of countries participating in olympics?
- **1896 Summer olympics** games has lowest count of **11** nations participating in an Olympic games.
- **2016 Summer olympics** games has highest count of **204** nations participating in an Olympic games.
  <img width="437" alt="Screenshot 2023-08-21 at 15 39 28" src="https://github.com/kirandhasade/Olympics_Sql_Project/assets/127043120/ab61ddda-b0ca-43ac-9a61-df9ec7b3c554">

#### Q.4 Which nation has participated in all of the olympic games?
- There are total 51 games played in all olympic games.
- Switzerland and UK are the only countries which participated in all olympic games.
 <img width="519" alt="Screenshot 2023-08-21 at 15 41 46" src="https://github.com/kirandhasade/Olympics_Sql_Project/assets/127043120/62a48cc8-acf9-4ad7-94f4-9156167065c4">

#### Q.5 Identify the sport which was played in all summer Olympics.
- Gymnastics, Weightlifting, Speed skating and weightlifting games had played in most of the summer Olympic games.
<img width="1015" alt="Screenshot 2023-08-21 at 15 43 13" src="https://github.com/kirandhasade/Olympics_Sql_Project/assets/127043120/7174d005-7994-435c-a130-34bf9e463162">

#### Q.6. Which Sports were just played only once in the Olympics.
- Aeronautics, Basque Pelota, Cricket, Croquet, Jeu De Paume, Military Ski Patrol, Motorboating, Racquets, Roque and Rugby Sevens are the games which are only played once in the Olympics.
- The number of athletes who participated in mentioned games was in less count. Hence sports count was 1 in the dataset.
  <img width="1015" alt="Screenshot 2023-08-21 at 15 46 05" src="https://github.com/kirandhasade/Olympics_Sql_Project/assets/127043120/329d7fb6-1522-4df4-8e9d-44a97f5f78f3">

#### Q.7  Fetch the oldest athletes Olympic year to win a gold medal.
- Oscar Gomer Swahn won the oldest Gold medal in 1912 Summer olympics games for shooting.
- Charles Jacobus won the oldest Gold medal in 1904 Summer olympics games for Roque.
  <img width="931" alt="Screenshot 2023-08-21 at 15 49 28" src="https://github.com/kirandhasade/Olympics_Sql_Project/assets/127043120/fe40bd8e-85a9-4fca-b8fe-467ba9c9708f">

#### Q.8 Fetch the top 5 athletes who have won the most medals (gold/silver/bronze). 
- **Robert Tait** have won most of the medals with the count of **58** while **Alferd and Jean** have won least medals with the count of **32**.
  <img width="1000" alt="Screenshot 2023-08-21 at 15 50 33" src="https://github.com/kirandhasade/Olympics_Sql_Project/assets/127043120/05986859-85a1-43c3-8584-815322517264">

#### Q.9 Fetch the top 5 most successful countries in the Olympics. Success is defined by no of medals won.
- **USA** has highest number of medals i.e. **5392** and **France** has least number of medals i.e. **1681**.
<img width="1006" alt="Screenshot 2023-08-21 at 15 51 45" src="https://github.com/kirandhasade/Olympics_Sql_Project/assets/127043120/538d9802-7577-44d8-8ee4-9b0197ee9e98">
<img width="582" alt="Screenshot 2023-08-21 at 15 52 11" src="https://github.com/kirandhasade/Olympics_Sql_Project/assets/127043120/81bc1af5-22a9-4e96-8afc-8ea2e268f651">

#### Q.10 In which Sport/event, India has won the highest medals?
- India has won most of medals in **Hockey** Sport with the count of **161**.
<img width="152" alt="Screenshot 2023-08-21 at 15 54 40" src="https://github.com/kirandhasade/Olympics_Sql_Project/assets/127043120/6ccb5f06-a114-403b-8042-3173d69a1c76">

#### Q.11 Break down all Olympic games where India won a medal for Hockey and how many medals in each Olympic game.
- India has won most of the medals i.e. **18** in 1936 Summer Olympics games  while least i.e. **11** in 1932 Summer Olympics games for Hockey.
  <img width="1003" alt="Screenshot 2023-08-21 at 15 56 27" src="https://github.com/kirandhasade/Olympics_Sql_Project/assets/127043120/f1543d12-bfc7-4ecf-b99c-1270ec11f0ab">

  #### Q.12 List top 15 down total gold, silver and bronze medals won by each country corresponding to each Olympic games.
  - Russia has won most of the gold medals i.e. **187** in 1984 Summer Olympic games,while USA won least number of medals in 1904 Summer i.e. **115**.
  



