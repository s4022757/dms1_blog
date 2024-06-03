---
title: DMS1 Week 7
published_at: 2024-05-02
snippet: Moving onto 3D modelling on Unity
---

# Session 1 - Spatial composition

In today's session Thomas introduced us to Unity, a game engine that can be used to create virtual environments for a range of different applications and platforms.

Luckily I had already installed Unity Hub and created an account and license but today I opened it up properly for the first time, installed the Editor and started a new 3D Core project.

Once opened, Thomas gave us a quick tour of the UI.

With the power of a virtual god...

![Cube GameObject](/w07s01/cube.png)

I made a cube!

## Solar System 

Thomas pointed us to Solar System Scope, a free resource that hosts a 3D model of our solar system. On their website can be found a number of high resolution textures for us to play around with in unity. As it was free, I made sure to download every available texture! 
*Not long until I'll need yet another hardrive.*

With the new snazzy textures, I returned to unity and imported all of the textures into the new project assets folder so we can put them to use.

With the textures imported, I then created a corresponding Material, necessary to apply textures to a GameObject. 

Let's see a texture at work.

![Moon Texture applied](/w07s01/moon_cube.png)

*I hope cube likes its new suit.*

Looks good but the shape is not quite right. Lets carve up the cube to look more moon-like.

![Sphericool](/w07s01/sverycool.png)

Much better.

Well now I have all these textures so let's make the moon some friends.

Beyond planet maps, Solar System Scope also provided a star map. I'll use this to make a new material but this time with Skybox/Panoramic shader settings to apply to the environment's background.

![Starbox & more planets](/w07s01/starboxd.png)

Much better, but there are still more textures to play around with. 

Let's complete an object for each of the 8 planets of our solar system.

![Virtual Solar System](/w07s01/SolarSystemNotToScale.png)

*R.I.P. Pluto*

Amongst the textures were additional textures like atmospheres. Lets now try creating a transparent material.

![Atmosphere](/w07s01/atmosphere.png)

Success!

Saturn's ring also has a texture. Lets try creating a GameObject to map the texture onto.

Hmm... Unity does not support the Torus shape natively in a 3D Core project. Let's see if there's a solution.

After searching online, there is an optional package available which might work. Let's try importing ProBuilder from the package manager.

![Torus](/w07s01/Torus404.png)

After a number of attempts, patience wears thin. Saturn will stay unadorned for now. 

This might be a good reminder to reign in ambition and ensure that plans for the environment I'll need to build for the next assignment are actually tenable.

## LinkedIn Learning

To build off of what I learnt today, I navigated to LinkedIn Learning's *Unity 2023 Essential Training* course run by Emmanuel Henri.

![Chapter 1 through 3](/w07s01/LiL/Chapter1-3.png)

Got through the first three chapters. Time for one more.

![Chapter 4](/w07s01/LiL/Chapter4.png)

Good to know.


## Assignment 3 Brainstorm

The next assignment ask that I design a virtual 3D environment which represents a *meaningful change or a transformational experience*. 

Thinking about my life there are a few options which might work:
- Early childhood and the move from the USA to Australia
- The loss of my mother and other loved ones in quick succession
- Moving from Sydney to Canberra 
- Starting secondary schooling
- Losing my path during high school
- Moving to India
- Coming to terms with my childhood and familial relationships
- Leaving secondary schooling
- Starting a career in hospitality back in Australia
- Backpacking adventures and moving to the UK
- Surviving and thriving during the pandemic
- Trapped in the tower
- Moving to Melbourne and starting Tertiary Education

Quite a lot to work with byt the list must be refined.

There are a number of options which could be quite abstract, and difficult to represent in a captivating 3D environment. With that in mind, let's eliminate the following:
- Moving from Sydney to Canberra
- Moving to India
- Coming to terms with my childhood and familial relationships
- Surviving and thriving during the pandemic

The assignment brief also mentions that the experience *could be in relation to a place, an event, an object, a person or group of people, or a **relationship** between these things*. Let's import the remaining options into an Obsidian canvas and draw relationships between these experience. 

![Mindmap of transformation](/w07s01/Transformative_Mindmap.png)

The options that I've highlighted in red seem to be quite interconnected. This will likely be the right direction.

### Outline

The environment that I intend to design will represent my move from New York City to Sydney, Australia. Starting in a metropolitan cityscape, the player will be lead towards a junction from which they will fall from the assumed path forward, drifting into void until arriving on a sunny beach.

### Assets required

#### Cityscape

For the cityscape, creating a terrain including streets and building facades will be fairly simply, although models with a higher level of detail may not be possible to create personally within the required time frame. 

3D models to find:
- Vehicles
- Street lights
- Human pedestrians
- Metropolitan backdrop

To flesh out this environment, bringing in sound will be imperative. I will review the audio recordings I have been amassing this semester, although this will be very simple to supplement with stock audio. 

Audio to find:
- Inner city traffic
- Ambient sounds of the city

Much of the cityscape will be comprised of concrete and glass. Depending on the 3D models I bring in, there textures may need to be replaced.

Textures to Find:
- Variations of concrete
- Brick
- Asphalt
- Glass

#### Void

Much of what we used for the solar system environment in today's class will be useful for the transition between cityscape and seaside. I'll need to check the usage rights for these and seek alternatives if they can't be used.

#### Seaside

With the seaside scene, the terrain should be fairly simple to create which should include a sandy beach, headlands on either side, a surf life saving club, and typical for a Sydney beach, a rock pool underneath the headland. This may still be bare, so I should find some additional foliage the outskirt dunes and headland. While it would be nice to have animated waves, I will need to look into tutorials and determine whether or not I can implement this in time.

3D models to find:
- Palm tree
- Long grass
- Assorted shrubs & foliage

What would the beach be without the calming sound of the tide crashing in? While I do already have some additional sounds of birdcall and such, I may not have time to travel to the beach to record waves crashing. Luckily there will certainly be hours of stock audio available freely online.

Audio to find:
- Waves crashing
- Cicadas chirping

Sydney beaches are notoriously adorned with golden sands, with of course, the ocean nearby. Headlands bare the rocks that comprise them, and will often have some amount of untouched foliage supporting the topsoil from eroding away.

Textures to find:
- Sand
- Ocean water
- Rock
- Grass
- Sandstone brick
- Red roof tiles

Finally, it would be of great personal significance to reproduce the scene in the following:

![Bench](/w07s01/HeadlandBench.jpg)

This would entail building or importing the following assets:
- Bench
- Wooden boardwalk
- Wooden fence

### Map

I've drafted an incredibly rough map for the scenes that I intend to make. 

Scene 1 - Cityscape

![Cityscape map](/w07s01/city.jpg)

Scene 2 - Void

![Void map](/w07s01/void.jpg)

Scene 3 - Seaside

![Seaside map](/w07s01/beach.jpg)

In drafting these maps, I've realised that it may not be obvious to the player where they must go to get to the next scene. Will revise and reiterate.


# Session 2 - Navigation design

To start this session off, Thomas gave a lecture about guiding navigation. There was some great information to factor into the environment I need to build such as:
- Entrances
- Paths
- Thresholds
- Wayfinding

I will definitely need to refine my plans and help design navigation through the scenes and environment.

## Wayfinding Activity

To put this new knowledge to the test, Thomas assigned us into groups to tackle an activity together.

I teamed up with Yifan and Kunzes and was assigned Muji as our destination. 

### Brief

The task was simple, we had to navigate ourselves to the destination by only utilising elements of our surroundings to help us find our way. 

### Step 1 - Orientation

To start, our group discussed where our starting point was in relation to our destination. Our DMS1 class is in Building 9 at the northern side of RMIT's City Campus which lies to the northern boundary of Melbourne's CBD.

We then needed to determine where our starting point was in relation to nearby landmarks and other surrounding features.

Outside of bulding 9 is Bowen St which runs north to south. To the south of the campus lies La Trobe St which runs east to west and which Bowen st terminates on its southern end. On the opposite side of La Trobe St to the south lies the State Library, a recognisable landmark with its great domed roof. The block south of the State Library, across Little Lonsdale St lies QV square, a shopping centre. The block west of the State Library, across Swanston St and a busy tram stop, lies Melbourne Central station and shopping centre. This shopping centre expands south across Little Lonsdale St, ending where it meets Lonsdale St proper. In the block opposite Lonsdale St to the south lies Emporium, a luxury shopping centre in which Muji has one of its retail stores.

This should be plenty of landmarks to keep in mind and orient ourselves with.


### Step 2 - Route Decision

Before making our way, our group had to decide on the route that we should follow to reach our destination. We though that following the streets would be straightforward as there was bound to be street signs to assist us stay on our route. Plus, we were certain to get lost if we entered the labrynthian mall too early. 

Leaving building 9, we would follow Bowen St south until La Trobe St, where we would turn right towards the west. Continuing on La Trobe, we would follow it to the end of the State Library and turn left onto Swanston Street. Following Swanston Street south, we would then continue on until either we determined we'd reached the boundary of QV Square on our left, towards the east, or saw a street sign demarking Lonsdale St running across Swanston, East to West. At that point we would look for an enterance for Emporium, heading either south or west towards it and looking out for anything to guide us further towards Muji. 


### Step 3 - Route Monitoring

Enough deliberation. Yifan, Kunzes and I then set out following our route.

We made it through Bowen St, onto La Trobe and reached the end of the State Library.

![Signs of Commerce](/w07s02/Wayfinding/Signs_of_Commerce.jpeg)

Hey look, certain signs of commerce! Oh, and there's the busy tram stop on Swanston. We don't seem to be lost yet. 
We then continued south on Swanston. *Or tried.*

![Obstacle](/w07s02/Wayfinding/Agitators.jpeg)

*We must act before we lose our way, Israel shant lead us astray.*

Circumventing the agitating masses, we continued south on the other side of the street.

![Japan Lies Ahead](/w07s02/Wayfinding/Japanese_Culture.jpeg)

Sushi? Japanese cultural breadcrumbing? We must be making progress.

We kept following Swanston south until we noticed that QV Square stopped at the upcoming road. Emporium must be towards the south-west. Looking to our right, we saw an enterance to Emporium and made haste.

At this point, our pre-planned route was exhausted and we were left only with our perception to guide us to the destination. We searched around our surroundings for any hint on where to find Muji. Once we entered Emporium we struck gold.

![Information Point](/w07s02/Wayfinding/Info_Icon.jpg)

Equip with the recent memory of our previous assignment, we knew that the icon we found represented information and was likely able to guide us the rest of the way. Using the information point, we used the interactive map it provided which told us where exactly inside the mall Muji was and laid out a path for us to follow the rest of the way to our destination.

### Step 4 - Destination Recognition

Lo and behold, the iconography saved the day and we spotted the calming, incandescent glow of the Muji Sign

![Destination Reached](/w07s02/Wayfinding/Muji.jpeg)

To verify that the destination was indeed Muji, and not an immitative illusion, we participated in the economy!

![Muji Haul](/w07s02/Wayfinding/Loot.jpeg)

Muji sure sells good stationary. *Maybe I need some new socks too.*


## The Terrain Tool

Having returned to class, Thomas continued the session with a lecture about the terrain tool. 

Let's start off by creating a new 3D Core project in unity. Then, lets create a new terrain found under Create GameObject.

![New Terrain](/w07s02/New_Terrain.png)

Then using the paint terrain tool, lets create some hills and a platform for a player character to look out from.

![Building Terrain](/w07s02/Build_Terrain.png)

Looks good, although a little plain. 

Thomas directed us to some textures provided on Canvas. After importing these assets, the paint texture tool will allow us to draw these textures onto our new terrain.

![Paint on textures](/w07s02/Paint_Texture.png)

Looks better than the greybox. We've now created some rolling green grassy hills and exposed rock on the sheer cliffs.

## Character Controller

Now we have a terrain, we'll need a character controller to enable a player to navigate the environment.

Luckily, there is also a pre-made character controller available to us on Canvas. Lets import this package and see our environment from the player's 1st person POV.

![1st person character controller](/w07s02/1stPersonCharacterController.png)

And here's what it now looks like when we play the game in our environment.

![1st Person POV](/w07s02/1stPersonPOV.png)

It's looking like a real game now. Or playable at least. I should now have the tools to create the physical elements of the environment for the next assignment.

## Homework

With our new knowledge, lets convert the plans from last session into a unity environment.

### Cityscape

First off, I'll convert the environment we made in session 2 into an environment that closer resembles the plan for Scene 1 - Cityscape.

First off, the building the player will start in.

![Starting Building](/w07s02/GreyboxPrototype/city/startbuilding.png)

And the environment that surrounds this building.

![Starting Area](/w07s02/GreyboxPrototype/city/startblock.png)

Then the connecting area, a avenue with surrounding skyscrapers.

![Skyline Avenue](/w07s02/GreyboxPrototype/city/skyline.png)

And a bird's eye view of the scene for reference.

![Bird's eye view](/w07s02/GreyboxPrototype/city/overview.png)


### Void

I'm thinking that the environment we created for the solar system system scope activity in last session will be perfect for the void scene I had intended to link the cityscape to the seaside scenes. I'll have to think of a way to transition between night and day, but for now it will do.


### Seaside scene

Next let's also convert the initial draft of the seaside scene into a greybox prototype.

First off, I'll use the terrain tool to create a headland.

![Headland](/w07s02/GreyboxPrototype/beach/headland.png)

Not exactly pretty but it'll do as a rough draft for now. 

I'll create another headland for the opposite side of the beach which will help frame things. We'll also need the surf life saving club. A cube will suffice for now.

![SLSC](/w07s02/GreyboxPrototype/beach/slsc.png)

With both headlands in place and the SLSC placed in between, lets start altering the terrain to look more beach-like. First I'll stamp out some sand dunes, and the stamp some ocean surface onto the water beyond.

![Sand Dunes](/w07s02/GreyboxPrototype/beach/dunes.png)

Again, it ain't pretty but it's definitely reminiscent.

Finally, here is a bird's eye view to provide perspective.

![Bird's eye view](/w07s02/GreyboxPrototype/beach/overview.png)


