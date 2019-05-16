## Choose Your Path jungle tool data

This directory contains the data used in the creation of the [Choose Your Path ](https://doranslab.gg/tools/jungle-tool.html) tool and the [Hacking the Jungle with Data Science](https://doranslab.gg/articles/hacking-the-jungle.html) article. This data contains jungler positions from minute 1 to minute 6 for nearly 100,000 matches in each file where each row represents the position data for a jungler from one match at a particular time point. All data came from patches 9.1 and 9.2 from matches that were diamond average or better on the North American server

The "blue_side_jungler_data.csv" file contains blue-side jungler data, and the "jungle_positions_red_side.csv" file contains red-side jungler data.

Column | Description
---|-----
`matchId` | Number that uniquely identifies each match (from Riot API)
`participantId` | Number that identifies a player in a particular match (From Riot API)
`win` | Value of 1 if jungler went on to win, and 0 if they went on to lose
`position1` | The jungler's position at 1:00 as a coordinate: [x-position, y-position]
`position2` | Same as above, for 2:00
`position3` | Same as above, for 3:00
`position4` | Same as above, for 4:00
`position5` | Same as above, for 5:00
`position6` | Same as above, for 6:00
