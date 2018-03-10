# Process_Journal
Keeping Track of my weekly process and thoughts I guess.

# Jan 8 - Jan 14

We were introduced to the class. We introduced ourselves and got an understanding of what we'd be doing through the course of the semester. For next week we need to finish the Tanks! Tutorial. And add additional components if we can.

We started the tutorials after looking at Pippin's games. The idea of coming up with many game concepts interests me, as I am similar but in terms of coming up with short story ideas at fast speeds. Not so much mechanics.

I've been thinking a lot about an interview of Shigeru Miyamoto in which he discussed how they tend to hire non gamers as they tend to come up with more interesting ideas and bring in outside influences as opposed to sticking to established mechanics and simply improving them. This interests me as well though it's a bit late for me as I'd consider myself already a gamer. But maybe I can still think up other things.

On the other hand, after class as I talked a bit with Melina, and Geoff before that, I threw out some ideas, which may have been aided or hampered by a headache I'd been having. But I thought they were interesting at the time. Will have to check again when the headache has died down. But mainly I thought it'd be funny if when a tank was destroyed a soldier would come out and need to be killed also to complete the game.

This led later while I was on the bus, to think about how this mechanic could be expanded like having empty tanks on the environment which would need to be destroyed so that when a pilot exits they can't get a new one and keep fighting. And even further developed into ideas for the main project where the player could exit the tank at will and would need to use the tank for puzzle solving situations of such. A horror like situation where a player must make it through a nightmarish landscape with the help of their tank for combat and visualization as well as general safety from enemies as the soldiers battle capabilities would be limited.

Also been thinking of fairy tales a lot and possible ways to integrate them into this game.

Wonder if I can make the soldier and extra tank version for next week.

# Jan 15 - Jan 21

## Initial Ideas

As we were discussing lights and the TANKS! unity game in general I came up with some ideas about what to play around with. Simple things like adding a sort of day night cycle to the game in which the sun/ light just moves over the area and out to represent the course of day and night, maybe adding lamp objects that turn on at night time.

As continuation to my puzzle ideas from last week I decided it'd be interesting if rather than the tank having a flash light the player can only see the environment based on the bullet emission to navigate an area. Or the tank shoots some form of Light rounds that illuminate an area for a while after they explode or remain where they land emmitting light for things like platforming and such. Need to work on the exit and enter tank script for the little soldier I modelled for my unfinished idea. 

In regards to camera I thought mainly of having it change depending on whether the player is in the tank or out. Hard to come up with other ideas, except maybe changing from orthographic to dynamic/regular 3D camera to solve environmental puzzles that otherwise couldn't be solved. Maybe even a First person mode that can be accessed through key press to examine other things. Need to research this further.

In regards to my original idea as well, the scattering of other tanks and having the soldier be the true goal adds to the use of the map which was criticized in class. I have ideas of how to make things work, such as when soldier collides with tank they switch layers. The main issue I have though is how the tank script must be changed for my idea to work as well as the game manager, mainly with things such as having the tank be assigned the controls of the player that enters and not having them interfere with others. As well as already having the tanks be active before being entered.

- Turret game idea: Have different tanks set around the area with their own cameras which are only controlled when you select their camera and chooose to shoot. May be a security panel like situation with UI buttons to control the shooting action. Have the bullets work as light source again so as to make it seem horror like as well. What are we shooting at and why, etc. Camera turns off when collision with enemy.(Becomes fuzzy or static if enemy nearby maybe?)

- Make Camera change rotation or position when a shot is fired/hits at random. Making the game disorienting and the such.

- Cutscene like situation, when tank exits the area and starts falling time slows down and actions must be taken to complete an objective in a specified time. Shoot something or have panels with story around. Can serve as transition from one place to another. During this the camera changes places to obscure things and maybe moves around the tank before the area changes. Scene changes are like jump cuts. Can use that to advantage in code.

Turns out the day/night idea was already done haha. But there are still many other things that can be edited. Illuminated 3D objects for environmental navigation. Think about more interesting things to work with for the rough prototype next week. Time Based light switches for navigation as well. For example panels that only light up at certain intervals.

- Game in which tank is controlled in a 3D area but navigates through the viewpoints of many cameras, and thats how you must determine where the tank is in the map. Dont get to see the tank, only either light or camera static.

## Secondary Progress Update

I've been experimenting with the camera and Lights, I've decided that itd be interesting if there were many screens displayed simultaneously and that the player must navigate a maze of displays in order to achieve their goal. I am still loking into entering and exiting vehicles as well. It'd also be interesting if the lights would only turn on if the player is in front of the camera that corresponds to the particular light. The goal may be to reach the enmy player or to enter their tank and then leave the area. 

This is the version I want to focus my efforts onto for now, as the more complex puzzle horror game would require many things I'm still not familiar/confident enough in. I will research things further. There are quite a few dumb bugs I must eke out.

# Jan 22 - Jan 28

## Lights and Camera Idea Evolution Week 2

New Idea has developed from issues trying to get the cameras to work as I want them to. The new Idea involves keeping the 16 cameras (but presenting the better aesthetically) but having them each represent a different level. So the pprogression must be tracked by the player from monitor to monitor while solving puzzles. Maybe bring down number of cameras from 16 to something more manageable and interesting. With different camera angles and setups.

# Jan 29 - Feb 4

## Lights and Camera Process Evolution Week 3

## Monday Update:

The past week was spent mainly on designing the levels/Puzzles as well as deciding what the final camera set up would be. Ultimately I decided to cut it down from 4 to 3 main puzzles (With one being a tutorial for all intents and purposes). I modelled out their Layouts based off of sketches and then brought them over to Unity. Where I realized that I must also take into account how far the light reaches for the puzzles to work... or that I'd need to make it so that the bullets a tank shoots only explode if they leave the area and will instead remain as light sources where they Landed. This may be preferable and much more interesting. in the end. This Does mean that some things need to be changed in terms of level design. Though theyre minor changes. I must get this to work as Intended, which should not really pose much Issue now that most of the Additional code has been done (Minus the bullet aspect) I must now just set up all the level collisions and materials as intended, set the cameras and test it out.

## Saturday Update:

I spent time adding colliders to the level and testing the camera arrangement. In the end I have 4 Cameras. 3 are Puzzle cameras and the last is the player camera. This camera follows the player around at a closer zoom than the others to clarify the direction of movement and overall navigation in the larger less visible areas. Tested to make sure It still showed under certain points. Now just need to make some small tweaks to the tanksand win/lose conditions and I should have a good prototype for class. Also Increased Tank Light Intensity to make sure theyre visible in the darkness. Also maybe deal with the music.

## Sunday Final Lights Update(?)

AAARGH, The Player entering Tank Script isnt working as I want It to, And the Lights similarly Have a rough time staying put, There are also some visibility issues. So I've decided to make a change to the overall structure. Rather than control the tanks independently, they are all controlled simultaneously, an issue lies with them faling off level so that will be changed as well so that they are more like rotating turrets used to light the soldier's way. I hope to fix it down the line, but sadly my prototype for tomorrow wont be what I hoped.

## Monday Final Lights Camera Update (For now)

Ran into a few issues in making the build for the game and making the game over and win conditions happen as intended. They still are't exactly as I want them currently but they're there. I was terrified for a bit when my home version of unity crashed and everything seemed to have been deleted. Thankfully it wasn't. I couldn't build at home so I brought it to class only to find out that the Unity version on the school computers had been updated so things apparently became obsolete and incompatible. I kept having issues making a build till fairly late into class.

# Feb 5 - Feb 11

## Monday Sound Ideas

Some initial Ideas for what to do for the prototype are coming to mind, such as making a sort of red light green light style game based on music in which certain areas become damage areas when music plays or doesn't or at certain beats. Or the ability to create sounds from the bullet collisions. References to bring to class have also come to mind such as the NieR Automata Blog post on sound, and videos on music and other sound implementation in games like Bastion, Transistor and other games. Diegetic and non diegetic implementations and interesting compositions.

I will post more Ideas here as they come to mind and develop them further, this time trying to not overcomplicate my idea and prototype. Scope is important, I sure wish I were good at managing it.

## Tuesday Sound Ideas

Main Game idea concept for now came to mind while in class, The idea of sound boxes or areas that make noise when triggered but also trigger so that the enemy AI targets the point from where the sound came. In this way a stealth game of sorts can be made in which the soldier must avoid making noise or the AI will be alerted. When the AI either sees the player or reaches the sound box the bool would turn off and return to original behaviours.

# Feb 12 - Feb 18

## Monday Sound Process

Basic sound prototype test with some features available. I couldn't get the AI to work from the addon so I looked up a way to make a basic tutorial that would serve my purposes. As such the prototype is still the base LevelArt (May change), and the base functions are that the tank will move towards the sound if the soundsource is triggered, and will chase the player if the player goes into the Tank's range. Currently the alternating floorboards aren't working but when they do it should damage the soldier or heal them depending on the boolean state which corresponds to the music/sound that plays. There will also be more tanks in the final edition and sound sources. The concept is based mainly off of the fight against David in _[The Last of Us](https://www.youtube.com/watch?v=-hqYCczGt7k)_, and the floor is both inspired in part by _[Crypt of the Necrodancer](https://www.youtube.com/watch?v=Rs4Sc6-PjQI)_ and also serves as motivation to keep the character moving.

Explore the theme of the game and idea behind it as per recommendation. Realize the good aesthetics and setting for the game. An Idea has come to mind in which the game is set in a haunted wood type area and the enemy is some sort of vengefulspirit or soldier and the player must escape them and the forest while avoiding certain areas which are haunted by weird damage area spirits or obstacles at certain points.Have a shepard's tone when enemies nearby. This is the super complicated version, though it may be possible due to the time available for it. Basic low poly character models. Maybe use the robot from long ago.

## Sunday Sound Process

While working on this I realized I probably won't have time for the big sound prototype as imagined after all but would like to implement it as a sort of large ongoing project in the end. After the class is finished I can work on it on the side and hopefully bring it to fruition in a sense. It would serve as a combination of all of the prototypes in the end Making use of camera and lights in a similar manner to that prototype and sound as well, though with edits to make it work of course. It has become a sort of narrative driven sci fi coop survival scenario in which one player controls movement and the other combat and lights. Soldiers trying to escape a nefarious robotic entity in a dark snowy forest location while also dealing with the fact that a war is going on simultaneously. But that isn't important at the moment.

In the current sound prototype the soldier will be followed if seen and also the tank will check a noise source if they hear it and are in range. It is possible for the soldier to lose the tank if they exit their field of effect, otherwise they may be trampled and damaged. Navigate the area listening for enemies and avoiding them. Tank is in the process of likely being replaced by something else like a robot or a monster, nthough nothing too detailed. More detailed versions would be saved for the large on going project.

# Feb 19 - Feb 25
## Friday Report

The past week has been spent mainly on adding a bit of further functionality to the AI, which may ultimately go to waste if things don't go according to plan in the implementation of the new 3D models that have been the focus of the past week. Though they could be changed to accomodate if necessary.

Main focus is the implementation of gravity to a spherical environment and allowing both the player and AIs to navigate said environment while avoiding obstacles. As well as implementing special triggers for the enemies and newly recorded sound effects.

## Saturday Update

There were some issues with the area modelling but those were fixed easily. However in the end I had to go against the mini planet idea due to peculiarities with the code. I instead made the levels into hill like structures that must be traversed for a similar effect to that of the original Idea. Now I just have to iron out some code edits and fix up the sound as well as menus and It should be done. I Need to manage multiple projects simultaneously better because a lot of time was wasted due to a roundtable rendering on the main PC interfering my other work due to strange lag. I need to lookinto this.

## Sunday Update

Hahaha, It was a day. I always end up stressing out over things and not noticing simple mistakes but it has been rather productive. I almost reset things multiple times due to minor issues I didn't understand till getting up and looking again. A major problem with me is that I don't feel as though what I've done is good enough or it is too simple so I end up forcing myself to add more stuff where it isn't necessary. I think the enemy noticing the player when a sound is made is good enough, though I was able to add enemy patrols now, and the tank does damage over time when it hits the soldier. I still have issues with the menu implementation but thats that, I'll find a way to fix it in the final version. I also do not know how to reset all the parameters when a scene is reloaded yet either so thats something that needs to change. I'm glad I was able to make use of most of my aesthetic decisions in spite of some issues. I'm generally happy with what I've made but my idea for a greater project to come out of this one still remains as well.

# Feb 26th to March 5th
## Saturday Update

I've been having abit of trouble coming up with ideas for this new project prototype. Interesting Ideas and just ideas that would work well with my final game idea conccept. One of the reasons I may be having a bit of trouble is because I have already been working with 3D environments or space to varying degrees in my past projects. 

One Idea I may pursue is an expansion of the world and gravity Idea I had for my past project, but this time with a sor of explorable insides of the area. Exploring moving areas that are antered for additional esher like aspect perhaps. Mazes into strange areas. This would take some work but I'd love to explore the concept further.

## Sunday Update

While looking for references that would allow me to make a round planet to walk o, I instead ran into a code that pulls objects towards it. Amongst other code this made me think that it could be interesting to instead work on a sort of endless falling survival game. In which the player must survive a certain amount of time without being pulled in by the pits of despair or some such. Rather than avoid obstacles the goal would be to use them to your advantage as platforms that slow down the player's descent, as they'd likely fall slower than the player, allowing the player to think a bit on their next move in order to survive.

# Maech 6th to March 12th
## Monday follow up and Tuesday Update

As discussed in class, I've now decided to work wit impossible spaces and the illusion of changing gravity by implementing portals into the game which will teleport the player onto separaate faces of the cubic area. However this is an illusion as the player is actually being teleported to a completely different cube on a different are that has the new face set as the bottom face so as to allow gravity to work normally. It serves as a sort of purgatory and look back on the past/life of the soldier in each face.

## Saturday Update

I've mainly been working on modelling out the cube zones as the code for the gameplay aspect I hope to pursue should be pretty much complete. I just need to integrate it into the game. The focus is 3D objects which I hope I can manage well enough. I am also developing the story for the characters further in my mind and trying to see how it'd all fit in well together. And how I could achieve everything in a much grander scale.
