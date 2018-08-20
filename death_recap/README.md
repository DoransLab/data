## Death Recap data

This directory contains the data for the [Death Recap](http://www.doranslab.gg/articles/rabadons-death-recap.html) article. The data consists of information from six fights that resulted in a player being killed, with each row corresponding to an event that contributed to the player's death.

Column | Description
---|-----
`fight_id` | ID of the fight.  There are six total fights, therefore six fight IDs (1-6).
`time` | Time at which an event took place (in seconds, game time).
`source` | Source of the damage.  Usually a champion, sometimes a turret.
`ability` | Ability used to do damage/CC. Can be ability, passive, auto, or item.
`damage` | Amount of damage  done with the ability.
`type` | Type of damage dealt from ability. Can be either `Magical`, `Physical`, `True`, or `None`.
`cc` | Type of CC applied during event, if any.  Left as `None` if not applicable.
`cc_duration` | Duration of CC applied during event. Left as 0 if no CC applied or if instant CC.
`fight_gif` | Corresponding GIF of fight to the event.  GIFs hosted on GFYCAT. Column contains URLs for GIF.
