Polytopia Deconstruction

Tribes
- name
- properties
  - theme
    - tiles
    - units
  - language
  - special troops
  - technology

Game
- number of opponents 1 - 9
- Difficulty levels 1,2,3,4
- map-size scales w/ number of opponents

World
- procedurally generated
  1. place cities, have to spread at least 2 tiles apart
     1. begin with cities placed evenly every 5 tiles
     2. randomly shift each city -1,0,1 X-unit
     3. randomly shift each city -1,0,1 Y-unit
     4. land-based tribes have a city on land
     5. sea-based tribes have a city in the sea
  2. starting a city, calculate the random probably of land/water
  3. for each tile, calculate the probably of it being mountain/sea-trench
  4. % of tiles that have a resource
- cities
  - at least 2 tiles apart
- resources
  - sea: fish
  - plains: gatherable plants
  - forest: huntable animals
  - ?mountain: mine
- tiles
  - plain
  - forest
  - mountains
  - coastal water
  - deep water
  - sea-trench

UI
- colored border outline around territories


Play
- turn-based
- start w/ 1 unit
- other tribes 
  - unknown until discovered
  - shows their size in number of cities
- stats
  - speed skill ~ how quickly you conquer others
  - battle ~ wins / total
  - tribes destroyed
  - weighted by difficulty
- building
  - building on empty plain or in the sea is a basic ability
  - building in forest, mountain, coast, or sea-trench requires advanced technology

Technology
- 5 branches, each w/ 2 sub-branches
  - transportation
    - roads
      - trade
    - free spirit
      - chivalry
  - hunting
    - conservation
      - mathematics
    - archery
      - spiritualism
  - seaman
    - whaling
      - advanced travel
    - sea construction
      - sea warfare
  - mountain
    - mining
      - smithing
    - meditation
      - philosophy
  - gathering
    - land construction
      - land warfare
    - agriculture
      - infrastructure

Units
- explorer
- fighting
- builder

Cities
- only the home-cities are occupied to begin with
- have levels, 1+
  - level is number of claimed resources in the cities area of control
  - number of live units that a city can sustain = level
    - i.e. lvl-5 city can sustain 5 units
- size
  - starts 1x1
  - when first occupied it goes up-to 3x3
    - depends on whether nearby cities have expanded into this one's territory
  - sequence
    -  1 | 3
    -  5 | 5
    - 14 | 7
    - 35 | 8
  - if the expansion territory covers another city the tribe automatically gains that city
    - tyrrant-mode: expansion co-opts resources in expanding city's zone
    - republic-mode: expansion occupies that city but grants adjacent to the new city
    - 