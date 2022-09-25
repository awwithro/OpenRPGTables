# DungeonWorld

``` follower
HP: {{ lookup "./followers/hp" }}
Damage: {{ lookup "./followers/damage" }}
Armor:

Quality: {{ lookup "./followers/quality" }}
Background: {{ lookup "./followers/background" }}
Loyalty: +1
Instinct: {{ lookup "./followers/instinct" }}
Cost: {{ lookup "./followers/cost" }}

Moves:
Tags:

```

## followers

|_Quality_|1d12|
|---|---|
|-1, A liability|1-3|
|+0, Reasonably competent. +1 tags|4-9|
|+1, Fully Capable. +2 tags|10-11|
|+2, An exceptional individual. +4 tags|12|

|_Background_|1d12|
|---|---|
|Has lived a life of servitude and opression: +Meek|1-2|
|Past their prime. -1 Quality. +1 _-wise|3|
|Has lived a life of danger. +2 tags|4-5|
|Unremarkable.|6-9|
|Has lived a life of privlege. +1 tag| 10|
|Specialist. +1 Quality. -2 tags|11|
|{{ fudge "./background" "1d11" 2}}|12|

|_Instinct_|1d12|
|---|---|
|Loot, pillage, and burn| 1|
|Hold a grudge and seek payback|2|
|Question Leadership and authority|3|
|Lord over others|4-5|
|Act impulsively|6-7|
|Give in to temptation|8-9|
|Slack off|10-11|
|Avoid danger or punishment|12|

|_Cost_|1d12|
|---|---|
|Debauchery - food, drink, gambling, sex, and mischief. The higher their Loyalty, the more extreme the cost.|1|
|Vengeance - payback against theose that have wronged them or their loved ones. The higher their Quality, the more direct and tangible the payback they require|2|
|Lucre - coin appropriate to their steading's Prosperity; highly skilled followers might demand more coin|3-5|
|Renown -  public recognition for their deeds and skills. The higher their Quality, the larger the audience reqcquired|6-7|
|Glory - defeating a worthy foe in battle. The higher their Quality, the more worthy the fow must be. Possibly limited to certain enemy types.|8-9|
|Affection - kind words and deeds, quality time and attention. The more extreme their Loyalty, the more affection they require.|10|
|Knowledge - secrets, mysteries, and wonders only found by exploring the wider world|11|
|Good - suffering alleviated, innocents defended, wrongs righted. The higher their Quality, the greater the good required.|12|

|_HP_|1d12|
|---|---|
|3 HP, Weak/frail/soft| 1-3|
|6 HP, Able-bodied| 4-9|
|9 HP, Tough/strong/hard|10-12|

|_damage_|1d12|
|---|---|
|d4, Not very dangerous|1-4|
|d6, Can defend themselves|5-10|
|d8, Veteran fighter|11-12|