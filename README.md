## W1
### Activity 1
Start working on an assignment on the day that it is assigned. This reduces the likelihood of procrastination. 

### Activity 2
1. 10
2. 2
3. These lines of code call the PrintMessage function, which prints "hello world" to Unity's console. This happens every frame.
4. MonoBehavior
5. These lines of code prints "x = 10" to Unity's console when the object with this script first appears in a scene
6. The 10 is the argument given to PrintMessage(), and the argument is passed to x. x is the parameter passed to Debug.log. 
7. Transform is not an object, but a class in Unity. While Translate is a method of the transform class, it can only be called on an instance of the class, not on the class itself. 
8. Replace Transform with _playerTransform

### Activity 3
[MG1 breakdown Google doc](https://docs.google.com/document/d/1UQTlTMUv7OoSRXdfaYn3iWpCgYABL-kNvOKmFYxCaUk/edit?tab=t.0)

## W2
### Activity 1
![image](https://github.com/user-attachments/assets/7a710b95-d8c0-4314-9372-2d74fd0be0fe)


### Activity 2
[Github commit link](https://github.com/UCI-GDIM32-W25/mg2-oop-review-Nedajist/commit/0d3b613a97bc3b1dd6d6453499c9e188191cf88b)
I believe I have met every element of the rubric. I added a player character who jumps but cannot double jump, and who collects moving coins upon colliding with them.
Collecting a coin updates the score text, and coins spawn in randomly.

## W3
### Activities 0-2
Partner's name: Marcelo Thomas Esposo Tolosa

### Activity 3
![image](https://github.com/user-attachments/assets/ed8352a5-04ef-446e-b46f-8cab00bf7ff0)

## W4
### Activity 1
Partner's name: Marcelo Thomas Esposo Tolosa
When I add multiple Locator objects to the scene, all but one of the locator components were destroyed upon running the game. This is because the Locator script 
actively searches for whether or not another locator component has been loaded, and if so, the locator destroys itself. One locator loaded in first when the game started, and
all of the other locators detected that first locator and destroyed themselves. 

### Activity 2
![image](https://github.com/user-attachments/assets/b42318ee-12f5-45c1-a661-318058b2a132)

### Activity 3
[Github commit link](https://github.com/Nedajist/HW4/commit/fec8998e363deebdee65a8e033564510bc0d50b7)
I've added the bird, pipe, and ground sprites into the game. Collisions and rigidbodies for the bird, pipe, and ground should be complete. I have also added
a trigger collider which will add to the player's score.

## W5
### Activity 1
I think the code for activity 1 is fine as is; one possible change I could think of is bundling IBreakable into item, such
that all items would have Damage, Break, and Use methods. Normal item classes would only need to inherit from item, not item and IBreakable.
Unbreakable items could implement empty damage and break methods. The tradeoff is less multi-inheritance, but more useless methods. 
I don't think it's a worthy exchange, but it is a possible alternative.

### Activity 2
The InventoryUI class is the view. The PlayerW5Demo2 class is the controller. The EnemyStats and itemW5Demo2 classes are the model.

### Activity 3
Scenario 1: GameController Singleton connecting UI, sound, playercontroller, data-storage classes together (model-view-controller). Polymorphism: base button class, with specialized children
buttons inheriting from it (like buttons meant to be held rather than pressed, buttons with special symbols). ScriptableObject containing player score, score value for each note. 

Scenario 2: Model tracking player stats and team-scores. View displaying all of the models, animations, and UI. Controller to handle player keyboard/mouse input. Polymorphism: basic parent gun class with 
attributes like ammo, damage. Children inherit from that class and add additional features, like specific damage effects or animation. 

Scenario 3: State machine for plants (seedling, partly-grown, fully-grown, etc). Model class tracking player inventory data and plant growth stages. View class displaying
all of the pixelart and sprites. Controller class to handle player input. ScriptableObject containing player inventory and currency balance.


### Activity 4
[Final Game Proposal Document Link](https://docs.google.com/document/d/1IXMcedZDubU3jHOIg-ZRwtj0N-xMFaV7MpOOSQTA65Q/edit?tab=t.0#heading=h.khlj2whc254g)

## W6
Talk: Narrative Writing, Cory Lanham
Senior Game writer @ Ready at Dawn
16+ years in games industry

“You throw a rock in Irvine, you’ll hit someone who worked on a cancelled Blizzard project.”

Game writers collaborate w/ design, art, animation, audio, engineering, leadership to craft a narrative which enhances the gameplay (hopefully)
- Plot & character arcs
- Worldbuilding and Lore
- Cinematic and mission dialogue
- Systemic Dialogue (“Barks”, AMbient dialogue)
- UI Text
- Marketing Text
- Voice acting documentation + other internal documentation
- “The demon” “absolute headache” localization

It is a miracle that any games get shipped at all

2 broad categories of writers: 

Freelance Writers
- Independent contractor, not official studio employee
- Hired to do specific job at specific time (barks, high-level story, polishing)
- Can work on multiple projects at once

In-House Writers
- Full-time studio employee. Writing from pre-prod → ship
- More influence over narrative, but you are not in charge. You only execute decisions.
- Need permission to work on multiple projects

Pre-production:
- Board full of sticky notes
- Deliver high-level narrative summary (key plot points)
- Understand the scope
- Eventually develop complete & detailed story outline
- Create scene description, “set pieces”, objectives
- Create narrative delivery methods 
- How the story will be told
- How the player will interact w/ story
- Find out how to import script into game 

Production:
- Write cinematic and mission scripts, collab with level design and leadership
- Write UI/UX text 
- Write barks, ambient dialogue
- Write worldbuilding and lore and history and timeline, non “player-facing” dialogue
- Sit in on voice actor recording sessions
- Much more expensive to re-write motion-captured lines
- You’re never working in a vacuum
- Re-write everything over and over and over again 
- Writing is cheap and malleable, unlike everything else


Post-production to Shipping
- Write marketing materials
- Write website
- Write trailers
- Re-write non-dialogue text (UI/UX, tooltip, etc)
- Often character names and made up words are offensive in some language 
- Provide translation notes for localization


Tools to use
- Google docs, MS Excel/Sheets
- For branching dialogue, use Arcweave, Twine, Yarn, Ink/Inkle
- Write script with Final Draft / Celtic

How to get into the games industry as a writer
- Work in another department first or a writing job not in games
- Bug a recruiter once a month for 12 months
- Get an entry level job with terrible pay

- In-House QA → Writing pipeline 
- If you’re QA-ing, try to interact with narrative in some way. Like proofreading text
- Get an internship and get a return offer 
- Make a game, preferably with others 
- Join discords & local meetups
