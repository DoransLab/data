## Individual Game Statistics

This directory contains individual game data collected from patch 8.14 for [Champion Clustering](http://www.doranslab.gg/articles/understanding-champ-similarity-i.html) article. Each .csv file contains information for only the position mentioned in its name.  Each row contains all of the summary statistics calculated or retrieved for an individual player’s game.

Column | Description
--|----
`true_role` | The position which we assigned a champion, these all match the file's name.
`champion_name` | The name of the champion.
`participant_id` | The player's participant ID in the game, a value of 1-5 represents a blue side player and a value of 6-10 represents a red side player.
`match_id` | The match ID which a row concerns.
`match_rank_score` | The average rank of a match where 1 is Bronze, 2 is Silver, 3 is Gold, 4 is Platinum, 5 is Diamond, 6 is Masters, and 7 is Challenger.
`account_id` | The account ID of the player.
`champion_id` | The champion ID that goes with the champion name
`win` | a 1 means the player won the match, a 0 means the player lost the match.
`companion_score` | The average Euclidean distance of a player to the nearest allied champion between minutes five and 20.
`split_score` | The average Euclidean distance of a player to all allied champions between minutes 15 and 30.
`rotation_score` | The average minute-to-minute change in arc length relative to the players angle to their fountain between minutes five and 20.
`gold_earned` | The total gold earned by a player in a game.
`kills` | A player's kills in a game
`deaths` | A player's kills in a game.
`assists` | A player's kills in a game
`total_minions_killed` | The number of minions a player killed.
`neutral_minions_killed` | The number of neutral minions a player killed.
`neutral_minions_killed_team_jungle` | The number junlge minions a player killed in their jungle.
`neutral_minions_killed_enemy_jungle` | The number of jungle minions a player killed in their enemy's jungle.
`wards_placed`| The number of wards a player placed in a game.
`wards_killed` | The number of wards a player killed in a game.
`damage_self_mitigated` | The amount of damage a player received that was prevented due to shields, armor, and damage reductions skills/abilities.
`total_damage_taken` | The total amount of damage a player received after mitigation.
`damage_dealt_to_objectives` | The amount of damage dealt by a player to structures and epic minions.
`damage_dealt_to_turrets` | The amount of damage dealt by a player to turrets.
`magic_damage_dealt_to_champions` | The amount magic damage dealt by a player to other champions in a game.
`physical_damage_dealt_to_champions`| The amount of physical damage a player dealt to other champions in a game.
`true_damage_dealt_to_champions` | The amount of true damage dealt by a player to other champions in a game.
`total_heal` | The total amount a player healed in a game.
`time_ccing_others`| The total time a player crowd controlled (CC'd) other players in seconds. Slows are weighted by 1/6 their time, soft CC's are weighted by 1/2, and hard CC's are weighted by 1.
`percent_taken` | The percentage of total damage received which was not mitigated by armor, shields, and damage reduction skills/abilities.
`total_damage_dealt_to_champions` | The total amount of all types of damage dealt to other champions in a game.
`percent_magic` | The percentage of the total amount of damage a champion dealt which was magic damage.
`max_time` | The length of the game in seconds.