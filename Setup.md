
## Downloading & Setting up the project
### Prerequisites:
- [Unity Hub](https://unity.com/download)
- [Unity 2021.3.15f1 (Our preferred version for XR)](unityhub://2021.3.15f1/e8e88683f834)

1. Install the latest release [here](https://github.com/HyperSilver69/SimiaVR)
2. Unzip the `SimiaVR.zip` file in a folder, preferably on your secondary disk.
3. Open Unity Hub and press the "Open" button
4. Select the folder in which you have the unzipped SimiaVR Template \
[Video Showcase](https://youtu.be/-nMC7X-Lo8o)

5. Once the project has loaded up, delete the scene presented to you and if you receive any errors, tell us in the [Discord Server](https://discord.gg/ME7UY9vYQD)




### Choosing your Locomotion style

as of version 1.0.0, Simia offers two types of locomotion!
- Gorilla Tag Locomotion/Gorilla Locomotion
- Capuchin v2-like locomotion

The Capuchin one has been known to give some issues, so it's not recommended.

Both styles have their own scene, so you can play with it if you want!
The scenes can by found in `Assets -> Resources -> Simia -> Scenes`

### What does Simia come with?
As of v1.0.0, Simia comes with working hit sounds, multiplayer (Which we'll go into detail on later), fully set up locomotion, some assets to get you started.

**MOST** of the things Simia has to offer are provided in Unity Packages. These are completely free and can be installed in literal seconds! You can find these in their own respective branch/sub-repository.

### How to install UnityPackages?

Unity packages are files created by Unity which hold certain Assets which can be moved easily around project-to-project with the click of a few buttons! Their file format is `.unitypackage`. They can be
imported via `Assets -> Import Package -> Custom package`. Each Package comes with it's own little menu showing how to use it, along with a written guide or a video tutorial.

### Multiplayer
Simia supports multiple multiplayer solutions, ranging from easy to set up solutions to ones that require a basic knowledge of networking. The following listed packages are the ones we support
- [Normcore (good for beginners, very limited.)]()








## The use of the math library

the `math` library contains a lot of useful functions.
In this tutorial we're gonna be looking at `math.random()`, `math.floor()`, and `math.ceil()`, the three most widely used.

`math.random` allows you to find a random number, whether this is in a table, just numbers, or between values.
```lua
local table1 = {
  "Hello!", "Bye!", "G'day!"
}
local table2 = {
 "Rage.","Happinness","Love"
}

local var = math.random() -- math.random() without any given argument will return a value between 0 and 1, with decimals.
local var1 = math.random(1, 65) -- math.random() with number arguments will return a value between min(first number) and max(last number), math.random allows up to 2 arguments.
local var2 = math.random(-5, 15) -- math.random() takes negative values. Remember to always put the smallest number as `min` and the largest number as `max`

local var3 = table1[math.random(#table1)] -- first, we use `table1[]` to make it obvious that we're refering to a table, then we call math.random(#table1), by doing so, we're applying math.random to `#table1`. Putting "#" before a table, will make it so we're getting a value, since "#" makes it numbered.
```
Now lets take a look at the outputs!
```lua
print(var)
print(var1)
print(var2)
print(var3)


----------------------------------------
0.91847161 -- print(var)
32 -- print(var1)
-3 -- print(var2)
Hello! -- print(var3)
```






Math.floor

Math.floor returns whatever value provided and lowers it to the nearest integer. Let's take a look!
```lua
local number = 4.9999999999 -- number with decimals
print(math.floor(number))


----------------------------------------
4 -- print(math.floor(number))
```
See how the name corrolates to the actual word "Floor"? and a floor is on the ground so we're going DOWN to the ground



Math.ceil

math.ceil returns whatever value provided and rouds it up to the nearest integer, let's take a look!
```lua
local number = 4.0000000001 -- number with decimals
print(math.ceil(number))

----------------------------------------
5 -- print(math.ceil(number))
```
See how the name corrolates to the actual word "Ceiling"? and a ceiling is above you, so we're going UP!
