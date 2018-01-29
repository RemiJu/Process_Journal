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

# Initial Ideas

As we were discussing lights and the TANKS! unity game in general I came up with some ideas about what to play around with. Simple things like adding a sort of day night cycle to the game in which the sun/ light just moves over the area and out to represent the course of day and night, maybe adding lamp objects that turn on at night time.

As continuation to my puzzle ideas from last week I decided it'd be interesting if rather than the tank having a flash light the player can only see the environment based on the bullet emission to navigate an area. Or the tank shoots some form of Light rounds that illuminate an area for a while after they explode or remain where they land emmitting light for things like platforming and such. Need to work on the exit and enter tank script for the little soldier I modelled for my unfinished idea. 

In regards to camera I thought mainly of having it change depending on whether the player is in the tank or out. Hard to come up with other ideas, except maybe changing from orthographic to dynamic/regular 3D camera to solve environmental puzzles that otherwise couldn't be solved. Maybe even a First person mode that can be accessed through key press to examine other things. Need to research this further.

In regards to my original idea as well, the scattering of other tanks and having the soldier be the true goal adds to the use of the map which was criticized in class. I have ideas of how to make things work, such as when soldier collides with tank they switch layers. The main issue I have though is how the tank script must be changed for my idea to work as well as the game manager, mainly with things such as having the tank be assigned the controls of the player that enters and not having them interfere with others. As well as already having the tanks be active before being entered.

-Turret game idea: Have different tanks set around the area with their own cameras which are only controlled when you select their camera and chooose to shoot. May be a security panel like situation with UI buttons to control the shooting action. Have the bullets work as light source again so as to make it seem horror like as well. What are we shooting at and why, etc. Camera turns off when collision with enemy.(Becomes fuzzy or static if enemy nearby maybe?)

-Make Camera change rotation or position when a shot is fired/hits at random. Making the game disorienting and the such.

-Cutscene like situation, when tank exits the area and starts falling time slows down and actions must be taken to complete an objective in a specified time. Shoot something or have panels with story around. Can serve as transition from one place to another. During this the camera changes places to obscure things and maybe moves around the tank before the area changes. Scene changes are like jump cuts. Can use that to advantage in code.

Turns out the day/night idea was already done haha. But there are still many other things that can be edited. Illuminated 3D objects for environmental navigation. Think about more interesting things to work with for the rough prototype next week. Time Based light switches for navigation as well. For example panels that only light up at certain intervals.

-Game in which tank is controlled in a 3D area but navigates through the viewpoints of many cameras, and thats how you must determine where the tank is in the map. Dont get to see the tank, only either light or camera static.

# Secondary Progress Update

I've been experimenting with the camera and Lights, I've decided that itd be interesting if there were many screens displayed simultaneously and that the player must navigate a maze of displays in order to achieve their goal. I am still loking into entering and exiting vehicles as well. It'd also be interesting if the lights would only turn on if the player is in front of the camera that corresponds to the particular light. The goal may be to reach the enmy player or to enter their tank and then leave the area. 

This is the version I want to focus my efforts onto for now, as the more complex puzzle horror game would require many things I'm still not familiar/confident enough in. I will research things further. There are quite a few dumb bugs I must eke out.

# Jan 22 - Jan 28

# Lights and Camera Idea Evolution Week 2

New Idea has developed from issues trying to get the cameras to work as I want them to. The new Idea involves keeping the 16 cameras (but presenting the better aesthetically) but having them each represent a different level. So the pprogression must be tracked by the player from monitor to monitor while solving puzzles. Maybe bring down number of cameras from 16 to something more manageable and interesting. With different camera angles and setups.

# Jan 29 - Feb 4

# Lights and Camera Process Evolution Week 3

# Monday Update:

The past week was spent mainly on designing the levels/Puzzles as well as deciding what the final camera set up would be. Ultimately I decided to cut it down from 4 to 3 main puzzles (With one being a tutorial for all intents and purposes). I modelled out their Layouts based off of sketches and then brought them over to Unity. Where I realized that I must also take into account how far the light reaches for the puzzles to work... or that I'd need to make it so that the bullets a tank shoots only explode if they leave the area and will instead remain as light sources where they Landed. This may be preferable and much more interesting. in the end. This Does mean that some things need to be changed in terms of level design. Though theyre minor changes. I must get this to work as Intended, which should not really pose much Issue now that most of the Additional code has been done (Minus the bullet aspect) I must now just set up all the level collisions and materials as intended, set the cameras and test it out.
