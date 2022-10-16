# DungeonWorld

| Region                                                                                               | 1d12 |
| ---------------------------------------------------------------------------------------------------- | ---- |
| {{lookup "./regions/adjective"}} {{lookup "./regions/terrain"}}                                      | 1-4  |
| {{lookup "./regions/terrain"}} of (the) {{lookup "./regions/noun"}}                                  | 5-6  |
| The {{lookup "./regions/terrain"}} {{lookup "./regions/adjective"}}                                  | 7-8  |
| {{lookup "./regions/noun"}} {{lookup "./regions/terrain"}}                                           | 9-10 |
| {{lookup "./regions/noun"}}'s {{lookup "./regions/adjective"}} {{lookup "./regions/terrain"}}        | 11   |
| {{lookup "./regions/adjective"}} {{lookup "./regions/terrain"}} of (the) {{lookup "./regions/noun"}} | 12   |

| Place                                                                                         | 1d12  |
| --------------------------------------------------------------------------------------------- | ----- |
| The {{lookup "./places/place"}}                                                               | 1-2   |
| The {{lookup "./places/adjective"}} {{lookup "./places/place"}}                               | 3-4   |
| The {{lookup "./places/place"}} of (the) {{lookup "./places/noun"}}                           | 5-6   |
| (The) {{lookup "./places/noun"}}'s {{lookup "./places/place"}}                                | 7-8   |
| {{lookup "./places/place"}} of the {{lookup "./places/adjective"}} {{lookup "./places/noun"}} | 9-10  |
| The {{lookup "./places/adjective"}} {{lookup "./places/noun"}}                                | 11-12 |

| Discovery                                   | 1d12 |
| ------------------------------------------- | ---- |
| {{lookup "./discoveries/unnaturalfeature"}} | 1    |
| {{lookup "./discoveries/naturalfeature"}}   | 2-4  |
| {{lookup "./discoveries/evidence"}}         | 5-6  |
| {{lookup "./npc"}}                          | 7-8  |
| {{lookup "./discoveries/structure"}}        | 9-12 |

| Danger                                  | 1d12 |
| --------------------------------------- | ---- |
| {{lookup "./dangers/unnaturalentity" }} | 1    |
| {{lookup "./dangers/hazard"}}           | 2-6  |
| {{lookup "dungeonworld/creature"}}      | 7-12 |

| Steading                                  | 1d12 |
| ----------------------------------------- | ---- |
| Village: {{lookup "./steadings/village" }} | 1-5  |
| Town: {{lookup "./steadings/town" }}       | 6-8  |
| Keep: {{lookup "./steadings/keep" }}       | 9-11 |
| City: {{lookup "./steadings/city"}}        | 12   |

| Creature                              | 1d12 |
| ------------------------------------- | ---- |
| {{lookup "./creatures/beasttext"}}    | 1-4  |
| {{lookup "dungeonworld/npc"}}         | 5-6  |
| {{lookup "./creatures/humanoidtext"}} | 7-8  |
| {{lookup "./creatures/monstertext"}}  | 9-12 |

``` npc
Context: {{lookup "./npcs/context"}}
Occupation: {{lookup "./npcs/occupation"}}
Appearance: {{lookup "./npcs/traits/physicalappearance"}}
Personality: {{lookup "./npcs/traits/personality"}}
Quirk: {{lookup "./npcs/traits/quirk"}}

HP: {{lookup "./npcs/traits/hp"}}
Damage Die: {{lookup "./npcs/traits/damagedie"}}
```

## Steadings

| _Built By_                                   |
| -------------------------------------------- |
| Humans                                       |
| {{lookup "dungeonworld/creatures/humanoid"}} |

``` village
{{lookup "dungeonworld/place"}}
Built By: {{lookup "./builtby"}}
Tags: Poor, Steady, Militia, Resource (add table), Oath (other steading)
Characteristics: {{lookup "./villages/characteristics"}}
Problem: {{lookup "./villages/problems"}}
```

``` town
{{lookup "dungeonworld/place"}}
Built By: {{lookup "./builtby"}}
Tags: Moderate, Steady, Watch, Trade (2 locations)
Characteristics: {{lookup "./town/characteristics"}}
Problem: {{lookup "./town/problems"}}
```

``` keep
{{lookup "dungeonworld/place"}}
Built By: {{lookup "./builtby"}}
Tags: Poor, Guard, Need (supplies), Trade, Oath
Characteristics: {{lookup "./keep/characteristics"}}
Problem: {{lookup "./keep/problems"}}
```

``` city

{{lookup "dungeonworld/place"}}
Built By: {{lookup "./builtby"}}
Tags: Moderate, Steady, Guard, Market, Guild, 2+ Oaths
Characteristics: {{lookup "./city/characteristics"}}
Problem: {{lookup "./city/problems"}}
```

### City

| _Characteristics_                                                      | 1d12 |
| ---------------------------------------------------------------------- | ---- |
| Permanent defenses, such as walls: +Defenses, Oath (GM’s choice)      | 1-3  |
| Ruled by a single individual: Personage (the ruler), Power (political) | 4-6  |
| Diverse: Dwarven or Elven or both                                      | 7    |
| Trade hub: Trade (every nearby steading), +Prosperity                  | 8-10 |
| Ancient, built on top of its own ruins: History (your choice), Divine  | 11   |
| Center of learning: Arcane, Craft (your choice), Power (arcane)        | 12   |

| _Problems_                                                                                                  | 1d12 |
| ----------------------------------------------------------------------------------------------------------- | ---- |
| Outgrown its resources: +Population, Need (food)                                                            | 1-3  |
| Designs on nearby territory: Enmity (nearby steadings), +Defenses                                           | 4-6  |
| Ruled by a theocracy: -Defenses, Power (divine)                                                             | 7-8  |
| Ruled by the people: -Defenses, +Population                                                                 | 9-10 |
| Supernatural defenses: +Defenses, Blight (related supernatural creatures)                                   | 11   |
| Occupies a place of power: Arcane, Personage (whoever watches the place of power ,Blight (arcane creatures) | 12   |

### Keep

| _Characteristics_                                                                |
| -------------------------------------------------------------------------------- |
| Belongs to a noble family: +Prosperity, Power (political)                        |
| Run by a skilled commander: Personage (the commander), +Defenses                 |
| Stands watch over a trade road: +Prosperity, Guild (trade)                       |
| Used to train special troops: Arcane, -Population                                |
| Surrounded by fertile land: remove Need (Supplies)                               |
| Stands on a border: +Defenses, Enmity (steading on the other side of the border) |

| _Problems_                                                                | 1d12  |
| ------------------------------------------------------------------------- | ----- |
| Built on a naturally defensible position: Safe, -Population               | 1-3   |
| Formerly occupied by another power: Enmity (steadings of that power)      | 4     |
| Safe haven for brigands: Lawless                                          | 5     |
| Built to defend from a specific threat: Blight (that threat)              | 6     |
| Has seen horrible bloody war: History (battle), Blight (restless spirits) | 7     |
| Is given the worst of the worst: Need (skilled recruits)                  | 8     |
| Suffers from disease: -Population                                         | 9-10  |
| Popular meeting place: +Population, -Law                                  | 11-12 |

### Town

| _Characteristics_                                                                       | 1d12  |
| --------------------------------------------------------------------------------------- | ----- |
| Booming: Booming, Lawless                                                               | 1     |
| At a crossroads: Market, +Prosperity                                                    | 2-3   |
| Defended by another steading: Oath (that steading), +Defenses                           | 4-5   |
| Built around a church: Power (divine)                                                   | 6-7   |
| Built around a craft: Craft (your choice), Resource (something required for that craft) | 8-10  |
| Built around a military post: +Defenses                                                 | 11-12 |

| _Problems_                                                                               |
| ---------------------------------------------------------------------------------------- |
| Outgrowing a vital resource: Need (that resource), Trade (a steading with that resource) |
| Offers defense to others: Oath (GM choice), -Defenses                                    |
| Outlaw rumored to live there: Personage (the outlaw), Enmity (steading preyed upon)      |
| Controls a good/service: Exotic (that good/service), Enmity (steading with ambition)     |
| Suffers from disease: -Population                                                        |
| Popular meeting place: +Population, Lawless                                              |

### Villages

| _Characteristics_                                                                 | 1d12 |
| --------------------------------------------------------------------------------- | ---- |
| Natural defenses: Safe, -Defenses                                                 | 1-3  |
| Abundant resources: +Prosperity, Resource (GM choice), Enmity (GM choice)         | 4-6  |
| Protected by another steading: Oath (that steading), +Defenses                    | 7-8  |
| On a major road: Trade (GM choice), +Prosperity                                   | 9-10 |
| Built around a wizard’s tower: Personage (the wizard), Blight (arcane creatures) | 11   |
| Built on a site of religious significance: Divine, History (GM choice)            | 12   |

| _Problems_                                                                                  |
| ------------------------------------------------------------------------------------------- |
| Surrounded by arid or uncultivable land: Need (food)                                        |
| Dedicated to a deity: Religious (that deity), Enmity (steading of opposing deity)           |
| Recently at war: -Population, -Prosperity if they fought to the end, -Defenses if they lost |
| Monster problem: Blight (that monster), Need (adventurers)                                  |
| Absorbed another village: +Population, Lawless                                              |
| Remote or unwelcoming: -Prosperity, Dwarven or Elven or other non-human                     |

## NPCs

| _Context_                          | 1d12  |
| ---------------------------------- | ----- |
| {{lookup "./contexts/wilderness"}} | 1-3   |
| {{lookup "./contexts/rural"}}      | 4-9   |
| {{lookup "./contexts/urban"}}      | 10-12 |

| _Occupation_                            | 1d12 |
| --------------------------------------- | ---- |
| {{lookup "./occupations/criminal"}}     | 1    |
| {{lookup "./occupations/commoner"}}     | 2-6  |
| {{lookup "./occupations/tradesperson"}} | 7-8  |
| {{lookup "./occupations/merchant"}}     | 9-10 |
| {{lookup "./occupations/specialist"}}   | 11   |
| {{lookup "./occupations/official"}}     | 12   |

| _Trait_                                  | 1d12  |
| ---------------------------------------- | ----- |
| {{lookup "./traits/physicalappearance"}} | 1-6   |
| {{lookup "./traits/personality"}}        | 7-9   |
| {{lookup "./traits/quirk"}}              | 10-12 |


### Contexts

| _Wilderness_                                        | 1d12 |
| --------------------------------------------------- | ---- |
| {{lookup "dungeonworld/npcs/occupations/criminal"}} | 1-2  |
| adventurer/explorer                                 | 3-4  |
| hunter/gatherer                                     | 5-6  |
| {{lookup "dungeonworld/npcs/occupations/commoner"}} | 7-8  |
| ranger/scout                                        | 9-10 |
| soldier/mercenary                                   | 11   |
| {{lookup "dungeonworld/npcs/occupations/official"}} | 12   |

| _Rural_                                                 | 1d12 |
| ------------------------------------------------------- | ---- |
| beggar/urchin                                           | 1    |
| {{lookup "dungeonworld/npcs/occupations/criminal"}}     | 2    |
| adventurer/explorer                                     | 3    |
| hunter/gatherer                                         | 4    |
| {{lookup "dungeonworld/npcs/occupations/commoner"}}     | 5-8  |
| {{lookup "dungeonworld/npcs/occupations/tradesperson"}} | 9    |
| {{lookup "dungeonworld/npcs/occupations/merchant"}}     | 10   |
| militia/soldier/guard                                   | 11   |
| {{lookup "dungeonworld/npcs/occupations/official"}}     | 12   |

| _Urban_                                                 | 1d12 |
| ------------------------------------------------------- | ---- |
| beggar/urchin                                           | 1-2  |
| {{lookup "dungeonworld/npcs/occupations/criminal"}}     | 3    |
| {{lookup "dungeonworld/npcs/occupations/commoner"}}     | 4-7  |
| {{lookup "dungeonworld/npcs/occupations/tradesperson"}} | 8    |
| {{lookup "dungeonworld/npcs/occupations/merchant"}}     | 9    |
| {{lookup "dungeonworld/npcs/occupations/specialist"}}   | 10   |
| militia/soldier/guard                                   | 11   |
| {{lookup "dungeonworld/npcs/occupations/official"}}     | 12   |

### Occupations

| _Criminal_          | 1d12 |
| ------------------- | ---- |
| bandit/brigand/thug | 1-2  |
| theif               | 3-4  |
| bodyguard/tough     | 5-6  |
| burglar             | 7-8  |
| dealer/fence        | 9    |
| racketeer           | 10   |
| lieutenant          | 11   |
| boss                | 12   |

| _Commoner_            | 1d12 |
| --------------------- | ---- |
| housewife/husband     | 1    |
| hunter/gatherer       | 2-3  |
| farmer/herder         | 4-6  |
| laborer/servant       | 7-8  |
| driver/porter/guide   | 9    |
| sailor/solder/guard   | 10   |
| clergy/monk           | 11   |
| apprentice/adventurer | 12   |

| _Tradesperson_         |
| ---------------------- |
| cobbler/furrier/tailor |
| weaver/basketmaker     |
| potter/carpenter       |
| mason/baker/chandler   |
| cooper/wheelwright     |
| tanner/ropemaker       |
| smith/tinker           |
| stablekeeper/herbalist |
| vintner/jeweler        |
| inkeeper/tavernkeeper  |
| artist/actor/minstrel  |
| armorer/weaponsmith    |

| _Merchant_              | 1d12 |
| ----------------------- | ---- |
| general goods/outfitter | 1-3  |
| raw materials           | 4    |
| grain/livestock         | 5    |
| ale/wine/spirits        | 6    |
| clothing/jewelry        | 7    |
| weapons/armor           | 8    |
| spices/tobacco          | 9    |
| labor/slaves            | 10   |
| books/scrolls           | 11   |
| magic supplies/items    | 12   |

| _specialist_         | 1d12 |
| -------------------- | ---- |
| undertaker           | 1    |
| sage/scholar/wizard  | 2    |
| writer/illuminated   | 3    |
| perfumer             | 4    |
| architect/engineer   | 5    |
| locksmith/clockmaker | 6    |
| physician/apothecary | 7    |
| navigator/guide      | 8    |
| alchemist/astrologer | 9    |
| spy/diplomat         | 10   |
| cartographer         | 11   |
| inventor             | 12   |

| _official_              | 1d12 |
| ----------------------- | ---- |
| town crier              | 1    |
| tax collector           | 2    |
| armiger/gentry          | 3-4  |
| reeve/sheriff/constable | 5    |
| mayor/magistrate        | 6    |
| priest/bishop/abbot     | 7    |
| guildmaster             | 8    |
| knight/templar          | 9    |
| lelder/high priest      | 10   |
| noble (baron, etc)      | 11   |
| lord/lady/king/queen    | 12   |

### Traits

| _Physical Appearance_                                                                       |
| ------------------------------------------------------------------------------------------- |
| disfigured (missing teeth, eye, etc.)                                                       |
| lasting injury (bad leg, arm, etc.)                                                         |
| tattooed/pockmarked/scarred                                                                 |
| unkempt/shabby/grubby                                                                       |
| big/thick/brawny                                                                            |
| small/scrawny/emaciated                                                                     |
| notable hair (wild, long, none, etc.)                                                       |
| notable nose (big, hooked, etc.)                                                            |
| notable eyes (blue, bloodshot, etc.)                                                        |
| clean/well-dressed/well-groomed                                                             |
| attractive/handsome/stunning                                                                |
| they are {{lookup "./physicalappearance" }} despite [a contra-dictory detail of your choice |

| _Personality_                                                                       |
| ----------------------------------------------------------------------------------- |
| loner/alienated/antisocial                                                          |
| cruel/belligerent/bully                                                             |
| anxious/fearful/cowardly                                                            |
| envious/covetous/greedy                                                             |
| aloof/haughty/arrogant                                                              |
| awkward/shy/self-loathing                                                           |
| orderly/compulsive/controlling                                                      |
| confident/impulsive/reckless                                                        |
| kind/generous/compassionate                                                         |
| easygoing/relaxed/peaceful                                                          |
| cheerful/happy/optimistic                                                           |
| they are {{lookup "./personality"}} despite [a contradictory detail of your choice] |

| _Quirk_                                                                      |
| ---------------------------------------------------------------------------- |
| insecure/racist/xenophobic                                                   |
| addict (sweets, drugs, sex, etc.)                                            |
| phobia (spiders, fire, darkness, etc.)                                       |
| allergic/asthmatic/chronically ill                                           |
| skeptic/paranoid                                                             |
| superstitious/devout/fanatical                                               |
| miser/pack-rat                                                               |
| spendthrift/wastrel                                                          |
| smart aleck/know-it-all                                                      |
| artistic/dreamer/delusional                                                  |
| naive/idealistic                                                             |
| they are {{lookup "./quirk"}} despite [a contradictory detail of your choice |

| _Competence_                       | 1d12  |
| ---------------------------------- | ----- |
| A liability: Quality -1, +0 tags   | 1-3   |
| Competent: Quality +0, +1 tags     | 4-9   |
| Fully capable: Quality +1, +2 tags | 10-11 |
| Exceptional: Quality +2, +4 tags   | 12    |

| _Background_                             | 1d12 |
| ---------------------------------------- | ---- |
| Life of servitude/oppression: +Meek      | 1-2  |
| Past their prime: -1 to Quality, +1 Wise | 3    |
| Has lived a life of danger: +2 tags      | 4-5  |
| Unremarkable                             | 6-9  |
| Has lived a life of privilege: +1 tag    | 10   |
| Specialist: +1 to Quality, -2 tags       | 11   |
| {{lookup "./background"}}                | 12   |

| _Instinct_                       | 1d12  |
| -------------------------------- | ----- |
| Loot, pillage, and burn          | 1     |
| Hold a grudge and seek payback   | 2     |
| Question leadership or authority | 3     |
| Lord over others                 | 4-5   |
| Act impulsively                  | 6-7   |
| Give in to temptation            | 8-9   |
| Slack off                        | 10-11 |
| Avoid danger or punishment       | 12    |

| _Cost_     | 1d12 |
| ---------- | ---- |
| Debauchery | 1    |
| Vengeance  | 2    |
| Lucre      | 3-5  |
| Renown     | 6-7  |
| Glory      | 8-9  |
| Affection  | 10   |
| Knowledge  | 11   |
| Good       | 12   |

| _Loyalty_ | 1d12  |
| --------- | ----- |
| 0         | 1-2   |
| 1         | 3-10  |
| 2         | 11-12 |

| _HP_ | 1d12  |
| ---- | ----- |
| 3    | 1-3   |
| 6    | 4-9   |
| 9    | 10-12 |

| _Damage Die_ | 1d12  |
| ------------ | ----- |
| d4           | 1-3   |
| d6           | 4-9   |
| d8           | 10-12 |

## Creatures

``` _beasttext_
{{ lookup "./beast" }}
Activity: {{lookup "dungeonworld/details/activity" }}
Disposition: {{lookup "dungeonworld/details/disposition" }}
Number Appearing: {{lookup "dungeonworld/details/numberappearing" }}
Size: {{lookup "dungeonworld/details/size" }}
```

| _Beast_                          | 1d12  |
| -------------------------------- | ----- |
| {{lookup "./beasts/earthbound"}} | 1-7   |
| {{lookup "./beasts/airborne"}}   | 8-10  |
| {{lookup "./beasts/watergoing"}} | 11-12 |

``` _humanoidtext_
{{ lookup "./humanoid" }}
Activity: {{lookup "dungeonworld/details/activity" }}
Alignment: {{ lookup "dungeonworld/details/alignment"}}
Disposition: {{lookup "dungeonworld/details/disposition" }}
Number Appearing: {{lookup "dungeonworld/details/numberappearing" }}
```

| _humanoid_                        | 1d12  |
| --------------------------------- | ----- |
| {{lookup "./humanoids/common"}}   | 1-7   |
| {{lookup "./humanoids/uncommon"}} | 8-10  |
| {{lookup "./humanoids/hybrid"}}   | 11-12 |

``` _monstertext_
{{ lookup "./monster" }}
Activity: {{lookup "dungeonworld/details/activity" }}
Alignment: {{ lookup "dungeonworld/details/alignment"}}
Disposition: {{lookup "dungeonworld/details/disposition" }}
Number Appearing: {{lookup "dungeonworld/details/numberappearing" }}
Size: {{lookup "dungeonworld/details/size" }}
Optional:
Ability: {{lookup "dungeonworld/details/ability" }}
Adjective: {{lookup "dungeonworld/details/adjective" }}
Aspect: {{lookup "dungeonworld/details/aspect" }}
Condition: {{lookup "dungeonworld/details/condition" }}
Feature: {{lookup "dungeonworld/details/feature" }}
Tags: {{lookup "dungeonworld/details/tag" }}
```

| _monster_                         | 1d12  |
| --------------------------------- | ----- |
| {{lookup "./monsters/unusual"}}   | 1-7   |
| {{lookup "./monsters/rare"}}      | 8-10  |
| {{lookup "./monsters/legendary"}} | 11-12 |

### Beasts

| _Earthbound_           |
| ---------------------- |
| termite/tick/louse     |
| snail/slug/worm        |
| ant/centipede/scorpion |
| snake/lizard           |
| vole/rat/weasel        |
| boar/pig               |
| dog/fox/wolf           |
| cat/lion/panther       |
| deer/horse/camel       |
| ox/rhino               |
| bear/ape/gorilla       |
| mammoth/dinosaur       |

| _Airborne_            |
| --------------------- |
| mosquito/firefly      |
| locust/dragonfly/moth |
| bee/wasp              |
| chicken/duck/goose    |
| songbird/parrot       |
| gull/waterbird        |
| heron/crane/stork     |
| crow/raven            |
| hawk/falcon           |
| eagle/owl             |
| condor                |
| pteranodon            |

| _Water Going_      |
| ------------------ |
| insect             |
| jelly/anemone      |
| clam/oyster/snail  |
| eel/snake          |
| frog/toad          |
| fish               |
| crab/lobster       |
| turtle             |
| aligator/crocodile |
| dolphin/shark      |
| squid/octopus      |
| whale              |

### Humanoids

| _Common_               | 1d12  |
| ---------------------- | ----- |
| Halfling               | 1-3   |
| Goblin/Kobold          | 4-5   |
| Dwarf/Gnome            | 6-7   |
| Orc/Hobgoblin/Gnoll    | 8-9   |
| half-elf/half-orc, etc | 10-11 |
| elf                    | 12    |

 | _Uncommon_         | 1d12  |
 | ------------------ | ----- |
 | fey                | 1     |
 | catfol/dogfolk     | 2-3   |
 | lizardfolk/merfolk | 4-6   |
 | birdfolk           | 7     |
 | ogre/troll         | 8-10  |
 | cyclops/giant      | 11-12 |

| _Hybrid_                                                        | 1d12  |
| --------------------------------------------------------------- | ----- |
| centaur                                                         | 1-2   |
| werewold/werebear                                               | 3-5   |
| werecreature (human {{lookup "dungeonworld/creatures/beast" }}) | 6     |
| human/{{lookup "dungeonworld/creatures/beast" }}                | 7-10  |
| human/({{lookup "dungeonworld/creatures/beast" 2}})             | 11-12 |

### Monsters

| _Unusual_                                                                             | 1d12  |
| ------------------------------------------------------------------------------------- | ----- |
| plant/fungus                                                                          | 1-3   |
| Undead Human                                                                          | 4-5   |
| Undead {{lookup "dungeonworld/creatures/humanoid"}}                                   | 6     |
| {{lookup "dungeonworld/creatures/beast" 2 }}                                          | 7-8   |
| {{lookup "dungeonworld/creatures/beast" }} {{lookup "dungeonworld/details/ability" }} | 9-10  |
| {{lookup "dungeonworld/creatures/beast" }} {{lookup "dungeonworld/details/feature" }} | 11-12 |

| _Rare_                                                                                     | 1d12  |
| ------------------------------------------------------------------------------------------ | ----- |
| slime/ooze                                                                                 | 1-3   |
| creation (Constuct)                                                                        | 4-6   |
| {{lookup "dungeonworld/creatures/beast" }} With: {{lookup "dungeonworld/details/oddity" }} | 7-9   |
| {{lookup "dungeonworld/dangers/unnaturalentity" }}                                         | 10-12 |

| _Legendary_                                       | 1d12 |
| ------------------------------------------------- | ---- |
| dragon/colossus                                   | 1-3  |
| Huge: {{lookup "./unusual"}}                      | 4-6  |
| Huge: {{lookup "./rare"}}                         | 7-9  |
| {{lookup "dungeonworld/creatures/beast" }} Dragon | 10   |
| {{lookup "./unusual"}} Dragon                     | 11   |
| {{lookup "./rare"}} Dragon                        | 12   |

## Dangers

| _Unnatural Entity_                          | 1d12 |
| ------------------------------------------- | ---- |
| {{lookup "./unnaturalentities/undeadtext"}} | 1-8  |
| {{lookup "./unnaturalentities/planartext"}} | 9-11 |
| {{lookup "./unnaturalentities/divinetext"}} | 12   |

| _Hazard_                                                                                                                                     | 1d12  |
| -------------------------------------------------------------------------------------------------------------------------------------------- | ----- |
| Unnatural Hazard: {{lookup "./hazards/unnatural"}}. {{lookup "dungeonworld/details/aspect" }}, {{lookup "dungeonworld/details/visibility" }} | 1-2   |
| Natural Hazard: {{lookup "./hazards/natural"}}                                                                                               | 3-10  |
| Trap: {{lookup "./hazards/trap"}}. {{lookup "dungeonworld/details/aspect" }}, {{lookup "dungeonworld/details/visibility" }}                  | 11-12 |

### Unnatural Entities

``` _undeadtext_
{{lookup "./undead"}}  
Ability: {{lookup "dungeonworld/details/ability"}}
Activity: {{lookup "dungeonworld/details/activity"}}
Alignment: {{lookup "dungeonworld/details/alignment"}}
Disposition: {{lookup "dungeonworld/details/disposition"}}
```

| _Undead_           | 1d12  |
| ------------------ | ----- |
| haunt/wisp         | 1-4   |
| ghost/spectre      | 5-8   |
| banshee            | 9     |
| wraith/wight       | 10-11 |
| spirit lord/master | 12    |

``` _planartext_
{{lookup "./planar"}}  
Ability: {{lookup "dungeonworld/details/ability"}}
Activity: {{lookup "dungeonworld/details/activity"}}
Alignment: {{lookup "dungeonworld/details/alignment"}}
Disposition: {{lookup "dungeonworld/details/disposition"}}
Element: {{lookup "dungeonworld/details/element"}}
Feature: {{lookup "dungeonworld/details/feature"}}
Tag: {{lookup "dungeonworld/details/tag"}}
```

| _Planar_                                                     | 1d12 |
| ------------------------------------------------------------ | ---- |
| imp (small)                                                  | 1-3  |
| lesser elemental: {{lookup "dungeonworld/details/element"}}  | 4-6  |
| lesser demon/horror                                          | 7-9  |
| greater elemental: {{lookup "dungeonworld/details/element"}} | 10   |
| greater demon/horror                                         | 11   |
| devil/elemental lord                                         | 12   |

``` _divinetext_
{{lookup "./divine"}}  
Ability: {{lookup "dungeonworld/details/ability"}}
Activity: {{lookup "dungeonworld/details/activity"}}
Alignment: {{lookup "dungeonworld/details/alignment"}}
Aspect: {{lookup "dungeonworld/details/aspect"}}
Disposition: {{lookup "dungeonworld/details/disposition"}}
Element: {{lookup "dungeonworld/details/element"}}
Feature: {{lookup "dungeonworld/details/feature"}}
Tag: {{lookup "dungeonworld/details/tag"}}
```

| _Divine_     | 1d12  |
| ------------ | ----- |
| agent        | 1-5   |
| champion     | 6-9   |
| army (horde) | 10-11 |
| avatar       | 12    |

### Hazards

| _Unnatural_        | 1d12 |
| ------------------ | ---- |
| taint/bligh/curse  | 1-3  |
| arcane trap/effect | 4-8  |
| planar trap/effect | 9-11 |
| divine             | 12   |

| _Natural_                                | 1d12  |
| ---------------------------------------- | ----- |
| blinding mist/fog                        | 1-2   |
| bog/mire/quicksand                       | 3-4   |
| pitfall/sinkhole/chasm                   | 5-7   |
| poison/disease                           | 8-9   |
| flood/fire/tornado                       | 10-11 |
| {{lookup "dungeonworld/details/oddity"}} | 12    |

| _Trap_                | 1d12  |
| --------------------- | ----- |
| alarm                 | 1-2   |
| ensnaring/paralyzing  | 3-5   |
| injurious (pit, etc.) | 6-8   |
| gas/fire/poison       | 9     |
| ambush                | 10-12 |

## Discoveries

| _Unnatural Feature_                                                                                                                       | 1d12  |
| ----------------------------------------------------------------------------------------------------------------------------------------- | ----- |
| Arcane: {{lookup "./unnaturalfeatures/arcane"}}. {{lookup "dungeonworld/details/alignment"}}, {{lookup "dungeonworld/details/magictype"}} | 1-9   |
| Planar: {{lookup "./unnaturalfeatures/planar"}}. {{lookup "dungeonworld/details/alignment"}}, {{lookup "dungeonworld/details/element"}}   | 10-11 |
| Divine: {{lookup "./unnaturalfeatures/arcane"}}. {{lookup "dungeonworld/details/alignment"}}, {{lookup "dungeonworld/details/aspect"}}    | 12    |

| _Natural Feature_                                                                                                                             | 1d12  |
| --------------------------------------------------------------------------------------------------------------------------------------------- | ----- |
| Lair: {{lookup "./naturalfeatures/lair"}}. {{lookup "dungeonworld/creature"}} responsible, {{lookup "dungeonworld/details/visibility"}}       | 1-2   |
| Obstacle: {{lookup "./naturalfeatures/obstacle"}}                                                                                             | 3-4   |
| Terrain Change: {{lookup "./naturalfeatures/terrainchange"}}                                                                                  | 5-7   |
| Water Feature: {{lookup "./naturalfeatures/waterfeature"}}                                                                                    | 8-9   |
| Landmark: {{lookup "./naturalfeatures/landmark"}}                                                                                             | 10-11 |
| Resource: {{lookup "./naturalfeatures/resource"}}. Size: {{lookup "dungeonworld/details/size"}}, {{lookup "dungeonworld/details/visibility"}} | 12    |

| _Evidence_                                                                                                                               | 1d12  |
| ---------------------------------------------------------------------------------------------------------------------------------------- | ----- |
| Tracks/Spoor: {{lookup "./evidence/tracks"}}. Age: {{lookup "dungeonworld/details/age"}} Made By: {{lookup "dungeonworld/creature"}}     | 1-6   |
| Remains/Debris {{lookup "./evidence/remains"}}. Age: {{lookup "dungeonworld/details/age"}}, {{lookup "dungeonworld/details/visibility"}} | 7-10  |
| Stash/Cache {{lookup "./evidence/stash"}}                                                                                                | 11-12 |

| _Structure_                                                                                                                                                                                                                             | 1d12 |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---- |
| Enigmatic: {{lookup "./structures/enigmatic"}}. {{fudge "dungeonworld/details/age" "1d8+4"}}, {{fudge "dungeonworld/details/size" "1d8+4"}}, {{lookup "dungeonworld/details/visibility"}}                                               | 1    |
| Infrastructure: {{lookup "./structures/infrastructure"}}. {{lookup "dungeonworld/steadings/builtby"}} responsible                                                                                                                       | 2-3  |
| Dwelling: {{lookup "./structures/dwelling"}}. {{lookup "dungeonworld/steadings/builtby"}} responsible                                                                                                                                   | 4    |
| Burial/Religious: {{lookup "./structures/burial"}}.{{lookup "dungeonworld/steadings/builtby"}} responsible, {{lookup "dungeonworld/details/alignment"}}, {{lookup "dungeonworld/details/aspect"}}                                       | 5-6  |
| Steading: {{lookup "dungeonworld/steading"}}                                                                                                                                                                                            | 7-8  |
| Ruin: {{lookup "./structures/ruin" }}. {{lookup "dungeonworld/steadings/builtby"}} responsible, {{fudge "dungeonworld/details/age" "1d8+4"}}, {{lookup "dungeonworld/details/ruination"}}, {{lookup "dungeonworld/details/visibility"}} | 9-12 |

### Unnatural Features

| _arcane_            | 1d12  |
| ------------------- | ----- |
| residue             | 1-2   |
| blight              | 3-5   |
| alteration/mutation | 6-7   |
| enchantment         | 8-10  |
| source/repository   | 11-12 |

| _planar_        | 1d12  |
| --------------- | ----- |
| distortion/warp | 1-4   |
| portal/gate     | 5-8   |
| rift/tear       | 9-10  |
| outpost         | 11-12 |

| _divine_       | 1d12  |
| -------------- | ----- |
| mark/sign      | 1-3   |
| cursed place   | 4-6   |
| hallowed place | 7-9   |
| watched place  | 10-11 |
| presence       | 12    |

### Natural Features

| _lair_                                                 | 1d12  |
| ------------------------------------------------------ | ----- |
| burrow                                                 | 1-3   |
| cave/tunnels                                           | 4-7   |
| nest/aerie                                             | 8-9   |
| hive                                                   | 10    |
| Ruins: {{lookup "dungeonworld/discoveries/structure"}} | 11-12 |

| _obstacle_                               | 1d12  |
| ---------------------------------------- | ----- |
| difficult ground (specific to terrain)   | 1-5   |
| cliff/crevasse/chasm                     | 6-8   |
| ravine/gorge                             | 9-10  |
| {{lookup "dungeonworld/details/oddity"}} | 11-12 |

| _terrain change_                                          | 1d12  |
| --------------------------------------------------------- | ----- |
| limited area of {{lookup "dungeonworld/regions/terrain"}} | 1-4   |
| crevice/hole/pit/cave                                     | 5-6   |
| altitude change                                           | 7-8   |
| canyon/valley                                             | 9-10  |
| rise/peak in distance                                     | 11-12 |

| _water feature_    | 1d12  |
| ------------------ | ----- |
| spring             | 1     |
| waterfall/geyser   | 2     |
| creek/stream/brook | 3-6   |
| pond/lake          | 7-8   |
| river              | 9-10  |
| sea/ocean          | 11-12 |

| _landmark_                               | 1d12  |
| ---------------------------------------- | ----- |
| water-based                              | 1-3   |
| plant-based                              | 4-6   |
| earth-based                              | 7-10  |
| {{lookup "dungeonworld/details/oddity"}} | 11-12 |

| _resource_            | 1d12  |
| --------------------- | ----- |
| game/fruit/vegetable  | 1-4   |
| herb/spice/dye source | 5-6   |
| timber/stone          | 7-9   |
| ore                   | 10-11 |
| precious metal/gems   | 12    |

### Evidence

| _tracks_             | 1d12  |
| -------------------- | ----- |
| faint/unclear        | 1-3   |
| definite/clear       | 4-6   |
| multiple             | 7-8   |
| signs of violence    | 9-10  |
| trail of blood/other | 11-12 |

| _remains_           | 1d12 |
| ------------------- | ---- |
| bones               | 1-4  |
| corpse/carcass      | 5-7  |
| site of violence    | 8-9  |
| junk/refuse         | 10   |
| lost supplies/cargo | 11   |
| tools/weapons/armor | 12   |

| _stash_             | 1d12  |
| ------------------- | ----- |
| trinkets/coins      | 1-3   |
| tools/weapons/armor | 4-5   |
| map                 | 6-7   |
| food/supplies       | 8-9   |
| treasure            | 10-12 |

### Structures

| _enigmatic_                              | 1d12 |
| ---------------------------------------- | ---- |
| earthworks                               | 1-4  |
| megalith                                 | 5-8  |
| statue/idol/totem                        | 9-11 |
| {{lookup "dungeonworld/details/oddity"}} | 12   |

| _infrastructure_      | 1d12 |
| --------------------- | ---- |
| track/path            | 1-4  |
| road                  | 5-8  |
| bridge/ford           | 9-10 |
| mine/quarry           | 11   |
| aqueduct/canal/portal | 12   |

| _dwelling_        | 1d12  |
| ----------------- | ----- |
| campsite          | 1-3   |
| hovel/hut         | 4-6   |
| farm              | 7-8   |
| inn/roadhouse     | 9-10  |
| tower/keep/estate | 11-12 |

| _burial_             | 1d12  |
| -------------------- | ----- |
| grave marker/barrow  | 1-2   |
| graveyard/necropolis | 3-4   |
| tomb/crypt           | 5-6   |
| shrine               | 7-9   |
| temple/retreat       | 10-11 |
| great temple         | 12    |

| _ruin_                                            | 1d12 |
| ------------------------------------------------- | ---- |
| Ruined {{fudge "./infrastructure" "1d6+6" }}      | 1-2  |
| Ruined {{fudge "./dwelling" "1d8+4"}}             | 3-4  |
| Ruined {{fudge "./burial" "1d8+4" }}              | 5-6  |
| Ruined {{fudge "dungeonworld/steading" "1d10+2"}} | 7-8  |
| {{lookup "dungeonworld/dungeon"}}                 | 9-12 |

## Regions

| _Terrain_ |
| --------- |
| Bay       |
| Bluffs    |
| Bog       |
| Cliffs    |
| Desert    |
| Downs     |
| Dunes     |
| Expanse   |
| Fells     |
| Fen       |
| Flats     |
| Foothills |
| Forest    |
| Groves    |
| Heath     |
| Heights   |
| Hills     |
| Hollows   |
| Jungle    |
| Lake      |
| Lowland   |
| March     |
| Marsh     |
| Meadows   |
| Moor      |
| Morass    |
| Mounds    |
| Mountains |
| Peaks     |
| Plains    |
| Prairie   |
| Quagmire  |
| Range     |
| Reach     |
| Sands     |
| Savanna   |
| Scarps    |
| Sea       |
| Slough    |
| Sound     |
| Steppe    |
| Swamp     |
| Sweep     |
| Teeth     |
| Thicket   |
| Upland    |
| Wall      |
| Waste     |
| Wasteland |
| Woods     |

| _Adjective_ |
| ----------- |
| Ageless     |
| Ashen       |
| Black       |
| Blessed     |
| Blighted    |
| Blue        |
| Broken      |
| Burning     |
| Cold        |
| Cursed      |
| Dark        |
| Dead        |
| Deadly      |
| Deep        |
| Desolate    |
| Diamond     |
| Dim         |
| Dismal      |
| Dun         |
| Eerie       |
| Endless     |
| Fallen      |
| Far         |
| Fell        |
| Flaming     |
| Forgotten   |
| Forsaken    |
| Frozen      |
| Glittering  |
| Golden      |
| Green       |
| Grim        |
| Holy        |
| Impassable  |
| Jagged      |
| Light       |
| Long        |
| Misty       |
| Perilous    |
| Purple      |
| Red         |
| Savage      |
| Shadowy     |
| Shattered   |
| Shifting    |
| Shining     |
| Silver      |
| White       |
| Wicked      |
| Yellow      |

| _Noun_     |
| ---------- |
| Ash        |
| Bone       |
| Darkness   |
| Dead       |
| Death      |
| Desolation |
| Despair    |
| Devil      |
| Doom       |
| Dragon     |
| Fate       |
| Fear       |
| Fire       |
| Fury       |
| Ghost      |
| Giant      |
| God        |
| Gold       |
| Heaven     |
| Hell       |
| Honor      |
| Hope       |
| Horror     |
| King       |
| Life       |
| Light      |
| Lord       |
| Mist       |
| Peril      |
| Queen      |
| Rain       |
| Refuge     |
| Regret     |
| Savior     |
| Shadow     |
| Silver     |
| Skull      |
| Sky        |
| Smoke      |
| Snake      |
| Sorrow     |
| Storm      |
| Sun        |
| Thorn      |
| Thunder    |
| Traitor    |
| Troll      |
| Victory    |
| Witch      |

## Places

| _Place_  |
| -------- |
| Barrier  |
| Beach    |
| Bowl     |
| Camp     |
| Cave     |
| Circle   |
| City     |
| Cliff    |
| Crater   |
| Crossing |
| Crypt    |
| Den      |
| Ditch    |
| Falls    |
| Fence    |
| Field    |
| Fort     |
| Gate     |
| Grove    |
| Hill     |
| Hole     |
| Hut      |
| Keep     |
| Lake     |
| Marsh    |
| Meadow   |
| Mountain |
| Pit      |
| Post     |
| Ridge    |
| Ring     |
| Rise     |
| Road     |
| Rock     |
| Ruin     |
| Shrine   |
| Spire    |
| Spring   |
| Stone    |
| Tangle   |
| Temple   |
| Throne   |
| Tomb     |
| Tower    |
| Town     |
| Tree     |
| Vale     |
| Valley   |
| Village  |
| Wall     |

| _Adjective_ |
| ----------- |
| Ancient     |
| Ashen       |
| Black       |
| Bloody      |
| Blue        |
| Bright      |
| Broken      |
| Burning     |
| Clouded     |
| Copper      |
| Cracked     |
| Dark        |
| Dead        |
| Doomed      |
| Endless     |
| Fallen      |
| Far         |
| Fearsome    |
| Floating    |
| Forbidden   |
| Frozen      |
| Ghostly     |
| Gloomy      |
| Golden      |
| Grim        |
| Hidden      |
| High        |
| Iron        |
| Jagged      |
| Lonely      |
| Lost        |
| Low         |
| Near        |
| Petrified   |
| Red         |
| Screaming   |
| Sharp       |
| Shattered   |
| Shifting    |
| Shining     |
| Shivering   |
| Shrouded    |
| Silver      |
| Stalwart    |
| Stoney      |
| Sunken      |
| Thorny      |
| Thundering  |
| White       |
| Withered    |

| _Noun_  |
| ------- |
| Arm     |
| Ash     |
| Blood   |
| Child   |
| Cinder  |
| Corpse  |
| Crystal |
| Dagger  |
| Death   |
| Demon   |
| Devil   |
| Doom    |
| Eye     |
| Fear    |
| Finger  |
| Fire    |
| Foot    |
| Ghost   |
| Giant   |
| Goblin  |
| God     |
| Gold    |
| Hand    |
| Head    |
| Heart   |
| Hero    |
| Hope    |
| King    |
| Knave   |
| Knight  |
| Muck    |
| Mud     |
| Priest  |
| Queen   |
| Sailor  |
| Silver  |
| Skull   |
| Smoke   |
| Souls   |
| Spear   |
| Spirit  |
| Stone   |
| Sword   |
| Thief   |
| Troll   |
| Warrior |
| Water   |
| Witch   |
| Wizard  |

## Details

| Ability                           |
| --------------------------------- |
| bless/curse                       |
| entangle/trap/snare               |
| poison/disease                    |
| paralyze/petrify                  |
| mimic/camouflage                  |
| seduce/hypnotize                  |
| dissolve/disintegrate             |
| ability: {{lookup "./magictype"}} |
| drain life/magic                  |
| immunity: {{lookup "./element"}}  |
| read/control minds                |
| {{lookup "./ability" 2}}          |

| Activity             |
| -------------------- |
| laying trap/ambush   |
| fighting/at war      |
| prowling/on patrol   |
| hunting/foraging     |
| eating/resting       |
| crafting/praying     |
| traveling/relocating |
| exploring/lost       |
| returning home       |
| building/excavating  |
| sleeping             |

| Adjective         |
| ----------------- |
| slick/slimy       |
| rough/hard/sharp  |
| smooth/soft/dull  |
| corroded/rusty    |
| rotten/decaying   |
| broken/brittle    |
| stinking/smelly   |
| weak/thin/drained |
| strong/fat/full   |
| pale/poor/shallow |
| dark/rich/deep    |
| colorful          |

| Age              | 1d12  |
| ---------------- | ----- |
| being born/built | 1     |
| young/recent     | 2-4   |
| middle-aged      | 5-7   |
| old              | 8-9   |
| ancient          | 10-11 |
| pre-historic     | 12    |

| Alignment | 1d12  |
| --------- | ----- |
| Chaotic   | 1-2   |
| Evil      | 3-4   |
| Neutral   | 5-8   |
| Good      | 9-10  |
| Lawful    | 11-12 |

| Aspect                  |
| ----------------------- |
| power/strength          |
| trickery/dexterity      |
| time/constitution       |
| knowledge/intelligence  |
| nature/wisdom           |
| culture/charisma        |
| war/lies/discord        |
| peace/truth/balance     |
| hate/envy               |
| love/admiration         |
| {{lookup "./element"}}  |
| {{lookup "./aspect" 2}} |

| Condition             | 1d12 |
| --------------------- | ---- |
| being built/born      | 1    |
| intact/healthy/stable | 2-4  |
| occupied/active/alert | 5-7  |
| worn/tired/weak       | 8-9  |
| vacant/lost           | 10   |
| ruined/defiled/dying  | 11   |
| disappeared/dead      | 12   |

| Disposition        | 1d12 |
| ------------------ | ---- |
| attacking          | 1    |
| hostile/aggressive | 2-4  |
| cautious/doubtful  | 5-6  |
| fearful/fleeing    | 7    |
| neutral            | 8-10 |
| curious/hopeful    | 11   |
| friendly           | 12   |

| Element | 1d12  |
| ------- | ----- |
| air     | 1-2   |
| earth   | 3-4   |
| fire    | 5-6   |
| water   | 7-8   |
| life    | 9-10  |
| death   | 11-12 |

| Feature                            | 1d12 |
| ---------------------------------- | ---- |
| heavily armored                    | 1    |
| winged/flying                      | 2-3  |
| multiple heads/headless            | 4    |
| many eyes/one eye                  | 5    |
| many limbs/tails                   | 6    |
| tentacles/tendrils                 | 7    |
| feature: {{lookup "./aspect" }}    | 8    |
| feature: {{lookup "./element" }}   | 9    |
| feature: {{lookup "./magictype" }} | 10   |
| feature: {{lookup "./oddity" }}    | 11   |
| {{lookup "./feature" 2}}           | 12   |

| Magic Type  | 1d12  |
| ----------- | ----- |
| divination  | 1-2   |
| enchantment | 3-4   |
| evocation   | 5-6   |
| illusion    | 7-8   |
| necromancy  | 9-10  |
| summoning   | 11-12 |

| Number Appearing                | 1d12  |
| ------------------------------- | ----- |
| Solitary (1)                    | 1-4   |
| Group ({{roll "1d6+2"}})        | 5-9   |
| Horde ({{roll "4d6"}} per wave) | 10-12 |

| Oddity                  |
| ----------------------- |
| weird color/smell/sound |
| geometric               |
| web/network/system      |
| crystalline/glass-like  |
| fungal                  |
| gaseous/smokey          |
| mirage/illusion         |
| volcanic/explosive      |
| magnetic/repellant      |
| devoid of life          |
| unexpectedly alive      |
| {{lookup "./oddity" 2}} |

| Orientation    | 1d12  |
| -------------- | ----- |
| down/earthward | 1-2   |
| north          | 3     |
| northeast      | 4     |
| east           | 5     |
| southeast      | 6     |
| south          | 7     |
| southwest      | 8     |
| west           | 9     |
| northwest      | 10    |
| up/skyward     | 11-12 |

| Ruination                  | 1d12 |
| -------------------------- | ---- |
| arcane disaster            | 1    |
| damnation/curse            | 2    |
| earthquake/fire/flood      | 3-4  |
| plague/famine/drought      | 5-6  |
| overrun by monsters        | 7-8  |
| war/invasion               | 9-10 |
| depleted resources         | 11   |
| better prospects elsewhere | 12   |

| Size         | 1d12  |
| ------------ | ----- |
| Tiny         | 1     |
| Small        | 2-3   |
| Medium-sized | 4-9   |
| Large        | 10-11 |
| Huge         | 12    |

| Tag                   | 1d12 |
| --------------------- | ---- |
| Amorphous             | 1    |
| Cautious              | 2    |
| Construct             | 3    |
| Devious               | 4    |
| Intelligent           | 5    |
| Magical               | 6    |
| Organized             | 7-8  |
| Planar                | 9    |
| Stealthy              | 10   |
| Terrifying            | 11   |
| {{lookup "./tag" 2 }} | 12   |

| Terrain                | 1d12  |
| ---------------------- | ----- |
| wasteland/desert       | 1     |
| flatland/plain         | 2-3   |
| wetland/marsh/swamp    | 4     |
| woodland/forest/jungle | 5-7   |
| highland/hills         | 8-9   |
| mountains              | 10-11 |
| {{lookup "./oddity" }} | 12    |

| Visibility                            | 1d12  |
| ------------------------------------- | ----- |
| buried/camouflaged/nigh invisible     | 1-2   |
| partly covered/over-grown/hidden      | 3-6   |
| obvious/in plain sight                | 7-9   |
| visible at near distance              | 10-11 |
| visible at great distance/focal point | 12    |
