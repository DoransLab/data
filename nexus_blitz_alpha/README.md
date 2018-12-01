# Nexus Blitz alpha data
These three datasets correspond to the [Nexus Blitz Numbers](https://doranslab.gg/articles/nexus-blitz.html) article. 

## Jungle pair data

This dataset has 9867 rows, each corresponding to a pair of junglers played in the Nexus Blitz alpha in North America.

Column | Description
---|-----
`champ1` | The first champion in the pair, e.g. "Anivia"
`champ2` | The second champion in the pair
`winrate` | The % of games won by this jungle duo
`ngames` | The number of Nexus Blitz games played with this jungle duo

## Champion stats by queue

This dataset has 564 rows and 12 columns. Each row corresponds to a champion in a game mode (e.g. Aatrox in ARAM). The columns correspond to different statistics calculated for these champions during the time the Nexus Blitz alpha was live. 

Column | Description
---|-----
`champion` | The champion, e.g. "Aatrox"
`queueid` | The game mode: 420 (Ranked Solo), 450 (ARAM), 470 (TT), or 1200 (Nexus Blitz)
`ngames` | Games played on the champion in that game mode
`nwins` | Games won on that champion in that game mode
... | (other end-of-game stats)
`subclass` | The champion subclass as [defined by  Riot](https://na.leagueoflegends.com/en/news/game-updates/gameplay/taking-another-look-subclasses)
`class` | The champion class as [defined by  Riot](https://na.leagueoflegends.com/en/news/game-updates/gameplay/taking-another-look-subclasses)

## Daily play counts

This dataset has 83 rows, each corresponding to a day. The columns correspond to the number of games played in Nexus Blitz, Ranked, and ARAM in North America each day.

Column | Description
---|-----
`date` | A day between 2018-07-20 and 2018-10-10. 
`nexus_blitz` | Nexus Blitz games played that day
`ranked` | Ranked games played that day
`aram` | ARAM games played that day
`nexus_blitz_smooth` |  Nexus Blitz games played, smoothed using a 7-day rolling mean**.
`ranked_smooth` | Ranked games played, smoothed using a 7-day rolling mean. 
`aram_smooth` | ARAM games played, smoothed using a 7-day rolling mean. 

** Note: In order to be able to show the play counts on the first few days of nexus blitz (which would normally be excluded by a 7-day rolling average), we allowed the average to be calculated as long as there were at least 2 games in the rolling window. So, on the first day of Nexus Blitz there was no smoothed value, but on the second day, there was one--- the average of the previous two days.
