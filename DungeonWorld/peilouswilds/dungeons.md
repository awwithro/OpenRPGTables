# DungeonWorld

``` dungeon
{{$size := lookup "./dungeons/size" -}}
Function: {{lookup "./dungeons/function" }}
Builder: {{lookup "./dungeons/builder" }}
Ruination: {{lookup "./dungeons/ruination" }}
Size: {{$size}}
{{$themes := lookup (print "./dungeons/sizes/" $size "/themes") |atoi -}}
Themes:
{{ range $x := until $themes -}}
      * {{lookup "./dungeons/theme" | print "\t" }}
{{end -}}
{{$areas := lookup (print "./dungeons/sizes/" $size "/areas") |atoi -}}
Areas:
{{ range $x := until $areas -}}
      * {{lookup "./dungeons/area" | print "\t" }}
{{end -}}
```

## Dungeons

| _Size_ | 1d12  |
| ------ | ----- |
| small  | 1-3   |
| medium | 4-9   |
| large  | 10-11 |
| huge   | 12    |

| _Ruination_                | 1d12 |
| -------------------------- | ---- |
| arcane disaster            | 1    |
| damnation/curse            | 2    |
| earthquake/fire/flood      | 3-4  |
| plague/famine/drought      | 5-6  |
| overrun by monsters        | 7-8  |
| war/invasion               | 9-10 |
| depleted resources         | 11   |
| better prospects elsewhere | 12   |

| _Builder_                                    | 1d12 |
| -------------------------------------------- | ---- |
| aliens/precursors                            | 1    |
| demigod/demon                                | 2    |
| natural (caves, etc.)                        | 3-4  |
| religious order/cult                         | 5    |
| {{lookup "dungeonworld/creatures/humanoid"}} | 6-7  |
| dwarves/gnomes                               | 8-9  |
| elves                                        | 10   |
| wizard/madman                                | 11   |
| monarch/warlord                              | 12   |

| _function_           | 1d12 |
| -------------------- | ---- |
| source/portal        | 1    |
| mine                 | 2    |
| tomb/crypt           | 3-4  |
| prison               | 5    |
| lair/den/hideout     | 6-7  |
| stronghold/sanctuary | 8-9  |
| shrine/temple/oracle | 10   |
| archive/library      | 11   |
| unknown/mystery      | 12   |

| _theme_                                             | 1d12  |
| --------------------------------------------------- | ----- |
| Mundane: {{lookup "./themes/mundane" }}             | 1-5   |
| Unusual: {{lookup "./themes/unusual"}}              | 6-9   |
| Extraordinary: {{lookup "./themes/extraordinary" }} | 10-12 |

| _discovery_                          | 1d12  |
| ------------------------------------ | ----- |
| {{lookup "./discoveries/dressing" }} | 1-3   |
| {{lookup "./discoveries/feature"}}   | 4-9   |
| {{lookup "./discoveries/find" }}     | 10-12 |

| _danger_                                                                      | 1d12 |
| ----------------------------------------------------------------------------- | ---- |
| Trap: {{lookup "./dangers/trap" }}                                            | 1-4  |
| Creature: {{lookup "./dangers/creature"}}: {{lookup "dungeonworld/creature"}} | 5-11 |
| Entity: {{lookup "./dangers/entity" }}                                        | 12   |

| _area_                                                                                    | 1d12 |
| ----------------------------------------------------------------------------------------- | ---- |
| Unthemed, Common: empty                                                                   | 1    |
| Unthemed, Common: Danger: {{lookup "./danger"}}                                           | 2    |
| Unthemed, Common: Discovery: {{ lookup "./discovery"}} and Danger: {{ lookup "./danger"}} | 3-4  |
| Unthemed, Common: Discovery: {{ lookup "./discovery"}}                                    | 5-6  |
| Themed, Common: Danger: {{lookup "./danger"}}                                             | 7    |
| Themed, Common: Discovery: {{ lookup "./discovery"}} and Danger: {{ lookup "./danger"}}   | 8    |
| Themed, Common: Discovery: {{ lookup "./discovery"}}                                      | 9    |
| Themed, Unique: Danger: {{lookup "./danger"}}                                             | 10   |
| Themed, Unique: Discovery: {{ lookup "./discovery"}} and Danger: {{ lookup "./danger"}}   | 11   |
| Themed, Unique: Discovery: {{lookup "./discovery"}}                                       | 12   |

### Sizes

#### Small

| _themes_       |
| -------------- |
| {{roll "1d2"}} |

| _areas_        |
| -------------- |
| {{roll "2d3"}} |

#### Medium

| _themes_       |
| -------------- |
| {{roll "1d3"}} |

| _areas_        |
| -------------- |
| {{roll "4d3"}} |

#### Large

| _themes_       |
| -------------- |
| {{roll "2d2"}} |

| _areas_                    |
| -------------------------- |
| {{min 16 (roll "3d6+6") }} |

#### Huge

| _themes_                  |
| ------------------------- |
| {{min 5 (roll "1d6+2") }} |

| _areas_                     |
| --------------------------- |
| {{min 24 (roll "4d6+10") }} |

### Dangers

| _trap_                                    |
| ----------------------------------------- |
| alarm                                     |
| ensnaring/paralyzing                      |
| pit                                       |
| crushing                                  |
| piercing/puncturing                       |
| chopping/slashing                         |
| confusing (maze, etc.)                    |
| gas (poison, etc.)                        |
| {{lookup "dungeonworld/details/element"}} |
| ambush                                    |
| magical                                   |
| {{lookup "./trap" 2}}                     |

| _creature_           |
| -------------------- |
| waiting in ambush    |
| fighting/squabbling  |
| prowling/on patrol   |
| looking for food     |
| eating/resting       |
| guarding             |
| on the move          |
| searching/scavenging |
| returning to den     |
| making plans         |
| sleeping             |
| dying                |

| _entity_                                                  |
| --------------------------------------------------------- |
| alien interloper                                          |
| vermin lord                                               |
| criminal mastermind                                       |
| warlord                                                   |
| high priest                                               |
| oracle                                                    |
| wizard/witch/alchemist                                    |
| Monster lord: {{lookup "dungeonworld/creatures/monster"}} |
| evil spirit/ghost                                         |
| undead lord (lich, etc.)                                  |
| demon                                                     |
| dark god                                                  |

### Discoveries

| _dressing_                                |
| ----------------------------------------- |
| junk/debris                               |
| tracks/marks                              |
| signs of battle                           |
| writing/carving                           |
| warning                                   |
| dead: {{ lookup "dungeonworld/creature"}} |
| bones/remains                             |
| book/scroll/map                           |
| broken door/wall                          |
| breeze/wind/smell                         |
| lichen/moss/fungus                        |
| {{lookup "dungeonworld/details/oddity"}}  |

| _feature_                     |
| ----------------------------- |
| cave-in/collapse              |
| pit/shaft/chasm               |
| pillars/columns               |
| locked door/gate              |
| alcoves/niches                |
| bridge/stairs/ramp            |
| fountain/well/pool            |
| puzzle                        |
| altar/dais/platform           |
| statue/idol                   |
| magic pool/statue/idol        |
| connection to another dungeon |

| _find_                |
| --------------------- |
| trinkets              |
| tools                 |
| weapons/armor         |
| supplies/trade goods  |
| coins/gems/jewelry    |
| poisons/potions       |
| adventurer/captive    |
| magic item            |
| scroll/book           |
| magic weapon/armor    |
| artifact              |
| {{lookup "./find" 2}} |

### Themes

| _mundane_            |
| -------------------- |
| rot/decay            |
| torture/agony        |
| madness              |
| all is lost          |
| noble sacrifice      |
| savage fury          |
| survival             |
| criminal activity    |
| secrets/treachery    |
| tricks and traps     |
| invasion/infestation |
| factions at war      |

| _unusual_                                 |
| ----------------------------------------- |
| creation/invention                        |
| {{lookup "dungeonworld/details/element"}} |
| knowledge/learning                        |
| growth/expansion                          |
| deepening mystery                         |
| transformation/change                     |
| chaos and destruction                     |
| shadowy forces                            |
| forbidden knowledge                       |
| poison/disease                            |
| corruption/blight                         |
| impending disaster                        |

| _extraordinary_     |
| ------------------- |
| scheming evil       |
| divination/scrying  |
| blasphemy           |
| arcane research     |
| occult forces       |
| an ancient curse    |
| mutation            |
| the unquiet dead    |
| bottomless hunger   |
| incredible power    |
| unspeakable horrors |
| holy war            |