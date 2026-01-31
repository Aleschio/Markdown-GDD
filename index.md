# Project *Gamename*

## Pinboard 
This is place for suggestions about this document
> porada ohladom mapy a core loop\
> MVP - co tam podla vas parti a co vynechat\
> pravidla pohybu, co vy na to? treba vymysliet a zapisat

## Gameinfo
1. Title: unknown
2. Genre: co-op tower defense
3. Target audience: web browser users

## MVP [minimum viable product]
### setup 
- [x]  game lobby - screen for player matching and starting gameplay
- [ ]  the map - simple map that conatains:
> player base - the city, slots for farms, slots for towers, paths, basic enviroment
- [ ]  UI - buttons and resources information
> food amount bar, gold count, mask button, book button
- [ ]  avatar movement

### mechanics
- [ ]  creeps movement mechanic
> pest spawn, movement path, wave timing, spawn amount
- [ ]  building farms and towers
> interact range, popup menu, upgrade/downgrade buttons, crop type/weapon type buttons, resource cost
- [ ]  avatar interaction mechanic
> collisions with buildings/walls/pests/second avatar; collect resource  tile upon collision
- [ ]  using mask mechanic
> collecting 5 pieces of mask, gradual mask button highliting; mask mode duration and cooldown; tower interaction; 
- [ ]  cooperation mode - how its played, how it ends
> players stop fighting one another and build some crops fo pests so they can achieve full food amount bars

### level design
- [ ]  first playable level

**required tiles**

1x1 (animated)
- grass
- gold nugget
- mask piece
- book
- redberry
- blueberry
- apple
- mushroom
- pest

2x2
- masked avatar
- unmasked avatar
- pest distraction field
- empty pest distraction field
- empty tower place
- basic tower
- spray tower

3x3
- empty farm field
- farm field

4x4
- the city - players base

### sound
- [ ] menu music
- [ ] game music
- [ ] win music
- [ ] game over music

- [ ] tower sound
- [ ] mask mode sound
- [ ] resource collect sound
- [ ] pest sound
- [ ] pest death sound

### polish 
  - [ ] menu
  - [ ] working exit button
  - [ ] music volume
  - [ ] sound volume
  - [ ] score

## Game lore

### story
> how did we get here...
### setting
> what is this place...
## Development

## Game design
### screen parameters
display resolution
> 1280x720

tile grid
> 32x18 tiles

Game UI size
> ?

### controls

**click on tile** - avatar moves to clicked tile and collect resource if there\
**click on empty building tile with avatar neraby*" - popup building upgrade/downgrade menu\
*bug button* (optional)- this will send wave of pest to both players\
**foreign mask button** - wear second player's mask - this allows you to go to their territory and do actions with buildings\
**book button** - this will unmask player and allow him to go to restricted area

**ingame menu button**

1. new game
2. music volume
3. sounds volume
4. hiscore
5. exit game

### core loop
this must be:
1. fun
2. repeatable
3. partially random
4. click on tile
**collecting resources**
- resources:
- are randomly appearing on map
- appear for limited time and disappear afterwards
- can be colleted by any avatar

- gold nugget - add 2-5 gold 
- mask piece - player has to collect 5 mask pieces to be able to use second player's mask
- book - player has to collect 7 books to be able to use "book button" - wich will unmask player upon activation
- food piece - add 3-10 to players food supply (increase over time)


### movement rules
this needs to be talked and decided:\
movement speed\
movement direction\
movement restrictions

### game progression
**START**

each player start game with gold (100) food supply (50), one active farm field\
farm field generate 1 food/5s
basic pest control tower
"the city" is providing building resources (metal, polymer, ceramics, power) and consume 2 food/5s - food consumption rises over time

**gameplay**

player has to upgrade food production ,build pest controll towers and collect appearing resources

after 1 minute, first wave of pests appear
waves are equally distributed to both players
when one player have all fields completely infected, pests will divide 80:20 with more pests attacking player with healthlier food production

food consumption and pests count increase over time
using pesticides is more effective than normal towers but using pesticides diminishes farms food production

**special actions**

when player obtain 5 mask pieces, upon activating mask button will be teleported to random location in second players territory and can perform actions 
- collect random appearig resources
- upgrade or downgrade farm field
- turn towers power on/off
- steal resources upon clicking on city tile

- mask activation last for max 10 seconds
- mask activation has 30 second cooldown
- player need to go home manualy
- player can deactivate mask mode earlier by clicking mask button again


when player obtain 7 books, upon activating book button will take off mask
 - without mask player is not targeted with any towers
 - player can acces "the pest fields" location
 - there you are able to build farmfields, that will attract pests and feed them, to stop infesting human lands
 - there are also farmfields slots for other player to build upon
 - when you max your fields, second player will have option to improve this field (with his knowledge) to double the pest attraction rate,
 - you will also have option to improve second player maxed pest fields to double its production and stop pests from infesting your lands.


### objective

**if both players starves** - "game over" => final score will be shown and saved to hiscores

**if one player starves:**
- his food runs out, he can't build farmfields, or towers, 
- his avatar speed is reduced, but he is able to collect resources and use mask features
- his resource production will rapidly
- his food consumption rate will slowly decrease
- 
**if both players fill their food supply to max** - "win win" => final score will be shown and saved to hiscores

**score formula:** 
((total generated food amount)*(10[only if both players win]))/((number of seconds from start)/100)


## Sounds

## Soundtrack

 > - [*Flute.0.0.1*](https://is.gd/0MXuq4)
 >> first commit
 > - [*Flute.0.0.2*](https://is.gd/SmaKw0)
 >> add strings
 > - [*Flute.0.0.3*](https://is.gd/iGGhSf)
 >> inverted strings
 > - [*Flute.0.0.4*](https://is.gd/Ecft50)
 >> bass + drums
 > - [*Flute.1.1.4*](https://is.gd/YT3iVb)
 >> loop structure
 > - [*in Game 0.0.1*](https://is.gd/rZSloC)
 >> first commit for in Game track 1
 > - [*in Game 0.1.2*](https://is.gd/YklHx0)
 >> add bass + drums
 > - [*in Game 0.1.3*](https://is.gd/PhFDch)
 >> add several bars should lower the bass
