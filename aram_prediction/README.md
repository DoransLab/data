## ARAM prediction data

This dataset has 585,363 rows and 143 columns and corresponds to the [ARAM Prediction tool](https://doranslab.gg/tools/aram-win-predictor.html). Each row represents one game. The first 141 columns correspond to champions, indicating the presence of each champion in the game. 

Column | Description
---|-----
`Aatrox` | The presence of Aatrox in game (1: red team, -1: blue team, 0: not in game)
... | Each other champion has its own column (1: red team, -1: blue team, 0: not in game)
`win` | The outcome of the game. 1 indicates the victory of red team, 0 indicates the victory of blue team
`matchId` | The ID number for the game provided by Riot's API