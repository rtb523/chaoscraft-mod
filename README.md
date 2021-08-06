# chaoscraft-mod
[Sign up on chaosnet.ai to use the mod, it's free](https://chaosnet.ai)


Note this is v0.3.* that is currently based off of 1.15.1 and is very much unstable as we build it.

For the old version v0.2.* that is based off of 1.12.1 check out https://github.com/schematical/chaoscraft-mod/tree/release/v0.2.1


## Getting Started:
## Install jdk1.8.0_202:

Make sure you have a 64bit java installation and at least 3 gb of free memory.


https://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html

## Clone repo:
```
git clone https://github.com/schematical/chaoscraft-mod.git
```

## Run Gradle:
I recommend using IntelliJ as an IDE but the ultra quick and dirty start is to open up the terminal and type:
```
gradlew runClient
```
This will start minecraft and you are ready to go!

## Login:
When you start a game you should be prompted to login with your ChaosNet login credentials

## Select a Training Room:
Assuming you are NOT connecting to a server that has already been setup once you log in you should be prompted to set the Trianing Room.

## Start Training:
From there the simulation should kick off.

### Additional Helpful Notes for Beginners(Thank You 0xFFFF):
https://pastebin.com/GwwRkDSM


### If you get stuck and keep getting 400 or 500 errors:
Try running the following:
```
/chaoscraft-repair
```
This will attempt to repair your build.

## Other stuff:
### CurseForge:
Eventually the mod may live at the following:

https://minecraft.curseforge.com/projects/chaoscraftai





## Matt's SideNotes:
AWS APIGateway Build Commands (I now have a script for this).
```
mvn clean package -Pstandalone-jar
cp target/ChaosNet-1.0-SNAPSHOT.jar  ~/IdeaProjects/chaoscraft/libs/ChaosNet-1.0-SNAPSHOT.jar
```

### Get Time of day:

```
World#getWorldTime() % 24000
```

###Stop Mobs from Spawning:
```
/gamerule doMobSpawning false
```

```
/kill @e[type=!player,name=!rick]
```

```
/kill @e[type=slime]
```

```
/kill @e[type=!player]
```

```
/time set day
```

```
/effect @p night_vision 9999 0 true
```

```
/tp @e[type=chaoscraft:rick] @p
```

```
/tp @e[name=adam] @p
```



shift click on a item in creative tab it grabs a max stack for you
```ctrl+q``` to drop a stack

https://github.com/socketio/socket.io-client-java

Networking Example 1.13 - https://github.com/sinkillerj/ProjectE/blob/mc1.13.x/src/main/java/moze_intel/projecte/network/PacketHandler.java



${stageVariables.LAMBDA} 
