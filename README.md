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

- ### Phase 1: Data Collection
- ##### We are using two tables which are available at MySQL database:
 - **olympics_history** table where each row corresponds to an individual athlete competing in an individual Olympic event.
 - **olympics_history_noc_regions** contains NOC(National Olympic Committee  a 3-letter code) which helps us to add country information and its corresponding region from its NOC code.

 - ### Phase 2: Data Understanding
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
