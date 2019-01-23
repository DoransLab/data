# Inting Sion and execute analysis data
------

These two datasets correspond to the [Inting Sion](www.doranslab.gg/articles/sion-winning-by-losing.html) article.

## Patch 8.20 Execute Analysis dataset

This dataset has the death and execute statistics for each champion in patch 8.20. Each row corresponds to a champion.
Column | Description 
 ---|----- 
`champion`| Champion name
`n_games`| Number of games champion appeared in
`executes`| Total times executed
`all_deaths`| Total number of deaths
`execute_rate_per_100`| Executes per 100 games
`total_death_rate`| Deaths per game
`class`| Class that champion belongs to, e.g."Fighter"


## Inting Sion dataset


This dataset has the data for the Inting Sion plot. Each row corresponds to a day between 9/15/18 and 11/23/18.
Column | Description 
 ---|----- 
`date`| The day, in M/D/Y format. Ranges from 9/15/18 to 11/23/18
`avg_deaths_all`| Overall average champion deaths per game
`avg_deaths_sion`| Average Sion deaths per game
`n_games_sion`| Number of games Sion appeared in