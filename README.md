# SQL Joins

### Part 1

Finish Regifter, if you haven't

### Part 2

Choose Your Own Learning

Rate your comfort and choose the matching activity

| Rating |              What it means               |                                                                                                               What you should work on                                                                                                               |
| :----: | :--------------------------------------: | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
|   5    | I feel amazing! Give me more challenges! | [Football/Futball/Soccer Data](https://github.com/jokecamp/FootballData/tree/master/openFootballData) Download and join the many tables to create info on historical data, like which players are on what teams? Who scored what goal in what game? |
|   4    |               Feeling good               |                                                                                     Go back to the bonus challenges in the lecture markdowns and solve each one                                                                                     |
|   3    |             Hanging in there             |                                                                                                 [Work your way through SQL Zoo](https://sqlzoo.net)                                                                                                 |
|   2    |           I'm feeling stressed           |                                                                                                [Work your way through SQL Bolt](https://sqlbolt.com)                                                                                                |
|   1    |           What just happened?            |                                                                                          Take a break and then schedule a time to talk to your instructor                                                                                           |

### In Canvas, answer the following questions:

- Which resource did you choose to use?

   - I chose `SQL Zoo`

- What are three things you learned during this lab?

    - Learned pattern matching strings which can be used to find a value in the table using the like operator %.

    - Learned how to use SELECT command and WHERE filter.

    - Learned how to use SELECT statements within SELECT statements which allows to perform more complex queries.
           - Example: 
               SELECT name
               FROM world
               WHERE continent='Europe' AND
               gdp/population>(
                  SELECT gdp/population
                  FROM world
                  WHERE name= 'United Kingdom'
                )
         This will select the counties in Europe with higher per capita GDP than 'United Kingdom'

