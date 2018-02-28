<img src="https://i.imgur.com/Ldzc6ju.png">

## About me

I am [Norman Benet](https://es.linkedin.com/in/NormanBenet), student of the
[Bachelor’s Degree in Video Games by UPC at CITM](https://www.citm.upc.edu/ing/estudis/graus-videojocs/). This content is generated for the second year’s
subject Project 2, under supervision of lecturer [Ricard Pillosu](https://es.linkedin.com/in/ricardpillosu).

## To start, here it is a brief explanation of production plan on videogames:

It is a document created **collaborative among the team** (if it is a small team, it will be done with the whole team, if it is a big one, it will be done with the leads of each section), as it affects each member of the team directly. 
It serves as a comprehensive task list of everything that needs to be implemented in the game and all of the components thereof. Which is then given a man-month requirement individually to help to define a most likely rough timeline for the development engagement.
There are professional project management tools like Jira or MS Project that helps the production plan. But, the simple spreadsheet production plan is a decent solution that works in a snap.

<img src="https://i.imgur.com/fLrgxGX.jpg">
*Example in excel from a [Business Model Report](https://zoltanjakibcfe.weebly.com/career-development-for-the-computer-games-industry.html).*

## 5 Aspects to take in account for doing a production plan:

### First of all:

We have to know that the game production pipeline is divided into 3 branches:

1·**PRE-PRODUCTION:** is time to have just an idea of a game from where to start building (e.g. “Make a game about number matching”).Having this, it is time to define all the details and came out with a **solid** game concept. Documents like [Game Design Document "GDD"](https://en.wikipedia.org/wiki/Game_design_document), [Technical Design Document "TDD"](https://www.studytonight.com/3d-game-engineering-with-unity/tdd-and-gdd), [Paper Prototype](http://gamedevelopertips.com/paper-prototyping-game-development/) are done here.

2·**PRODUCTION:** here is where the designer, engineers, producers and basically all the members of the team will work together to bring the game to life. It is important to know that changes in this phase will cost a lot in terms of time and money to invest.

3·**POST-PRODUCTION:** is the time to get your game to an audience as large as possible and first, solve all the bugs possible with testers on a Beta. Then, the game is ready to buy. Developers can add new features to expand the game in order to increase the retention of the game.

<img src="http://1.bp.blogspot.com/-rneaL5NCyx8/VdzlLlCT_FI/AAAAAAAAARg/i2LjDE9nG7U/s640/six%2Bsigma.jpg">
*Image from [Oniralia Blogspot](http://oniralia.blogspot.com.es/)*

### Second:

Now, knowing the pipeline a question can come to us: **When is the Production Plan done?**

It is done at the earliest of the pipeline, on the pre-production, to have a schedule for the Concept creation and all the details defined. But, once the GDD and TDD are done, we have the enough information to determine the staff size. After the staffing plan* the planning will be mostly accurrate (Mostly? Yes, making games is "a bit" unpredictable). 

### Third:

The production plan estimates the expenditure of the total production of the game. A simple list of costs on making a game could be this one:

Organized by categories the costs are the following:

·**FIXED COST:** salaries, electricity, rent of the studio, etc.

·**VARIABLE COST:** software license fees, short-turn contractors, travels, etc.

The budget could be divided in 5 branches:

1·**SALARIES**.

2·**GENERAL & ADMINISTRATIVE**.

3·**RESEARCH & DEVELOPMENT**.

4·**LICENSES**.

5·**TRAVEL & ENTERTAINTMENT**.

### Fourth:

Momentarily, we basically comprehend how the costs are broken. The aim of the production plan is not leaving anything open and contemplate all the hypothetical problems and their solutions. I would like to mention a sentence that reflects what, probably, will happen if there are vulnerable parts of the plan:

-*Anything that can go wrong will go wrong* - Murphy's Law.

### Fifth:

Production schedules are by their nature imprecise, as it is entirely based on estimates and not actual development. This directly means that when you make a schedule, give a development time buffer. You will be glad you did. 

The buffer could be this: **_YOUR ESTIMATE + 20%_**. 

## What should Production Plan has to contain?

<img src="https://tops-secure-graphics.grocerywebsite.com/GraphicsShoppingList/ShoppingListIcon_221x221.png">

These are what a good Production plan **must** have: Initial planning, Feature list, Break down of tasks, assign tasks, dependencies, schedule, milestones.
HOW TO PUT A VIDEO: 

<iframe width="560" height="315" src="https://www.youtube.com/embed/GiHrWDm7B6M" frameborder="0" allowfullscreen></iframe>

### Game Controls
**A** - Move player to the left.

**D** - Move player to the right.

**SPACE** - jump/double jump (on air).

**MOUSE LEFT** - interact with UI elements that allows to click.

**ESC** - Close application/toggle pause (in mid-game).

#### Debug Keys
**F1** - Start from the very first level.

**F2** - Start from the beginning of the current level.

**F3** - Activate/Deactivate path drawing.

**F5** - Save the current state.

**F6** - Load the previous state.

**F8** - Activate/Deactivate collider GUI drawing.

**F9** - Activate/Deactivate collider drawing.

**F10** - Activate/Deactivate god mode.

**F11** - Activate/Deactivate Framecap.

### Main Core Subsytems
This game has 5 main modules:

**Entity System** that holds all entities such as: player, enemies, collectibles and deals with their physics.

It is connected with the **pathfinding** which is in charge of calculating the path that each enemy will do and send it to him.

The **map** which reads .tmx files that hold all information of the tile based level (done in [Tiled](http://www.mapeditor.org/))(position and texture of each tile, collisions and entity position).

The **UI** with a polymorphism system of UI elements that can be created and managed by the GUI module and stored in menu structs to deal with them in groups.

And finally but not less important, the **scene management**, which is in charge of deliverying to the renderer the current level, menu and entities on screen as well as managing the transitions between them.

### Innovation features
**1st Assignment**

Simple entity system for player, thought to hold more entity types.

**2nd Assignment**

· Logic for entities(animations, speed, jump force and collider size and position) is defined in tiled.

	Their position on the map is also defined in tiled.

· When god mode is activated and the player dies or falls out of the map, he will reappear in the further platform that he has reached.

· When an enemy does not found a path to the player, after 1.5 seconds it will start flying/walking around.

		Charger(Boar): Will walk along all the platform in each directions.

		Bat: Will fly randomly across air.

**3rd Assignment**

- In the main menu, there is a continue button that can be unabled (after losing all lives or completing the game),
or enabled (if saved game with f5 or by going back to main menu while in mid-game).

- The volume control is done by sliders, which also show the current percentage.

- There is a switch button to toggle fullscreen.

- The game can be paused at any time while in mid-game using the top-right button or 'ESC'.

- UI element progress bar that can be decreasing or increasing and have multiple marks that can be active or unactive with diferent textures.

		In mid-game, there is a bar that decreases overtime and shows the current trophy
		that would be obtained, each one turning dark after losing it.

		When the game is paused, it will open a menu with a progress bar
		that shows the current position of the player respect the level length.

- After completing the game, it will open a menu with the score , the trophy and the coins obtained.

### Developer Team

<img src="https://drive.google.com/uc?id=1vQUdU2pbTyUeGBdSpkp46poJoaWvpupi">

[Adrià Ferrer](https://github.com/Adria-F)

- Entity system.
- Half of individual entities creation.
- Half of pathfinding algorythm.
- Design of the UI.
- Half of UI elements implementation.



[Norman Benet](https://github.com/Normanbg)

- Half of individual entities creation.
- Half of pathfinding algorythm.
- Design of the levels and difficulty.
- Menu composition and behaviour.
- Half of UI elements implementation.

## Check Out the repository [here](https://github.com/Adria-F/Game-Development)

## Download the last version of N.A.T.P [here](https://github.com/Adria-F/Game-Development/releases/tag/3.0)


### License
This is free and unencumbered software released into the public domain.

Anyone is free to copy, modify, publish, use, compile, sell, or
distribute this software, either in source code form or as a compiled
binary, for any purpose, commercial or non-commercial, and by any
means.

In jurisdictions that recognize copyright laws, the author or authors
of this software dedicate any and all copyright interest in the
software to the public domain. We make this dedication for the benefit
of the public at large and to the detriment of our heirs and
successors. We intend this dedication to be an overt act of
relinquishment in perpetuity of all present and future rights to this
software under copyright law.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR
OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
OTHER DEALINGS IN THE SOFTWARE.