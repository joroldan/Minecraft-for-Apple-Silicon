# Minecraft for Apple Silicon
Minecraft 1.18.1 for Apple Silicon

## How to use it?

1. Simply create a folder called `arm-1.18.1` inside your `minecraft/versions` folder and put `arm-1.18.1.json` inside.
2. Create a new profile using this version
3. In the profile settings specify an ARM Java Virtual Machine
4. Play and enjoy!

## Where is my `minecraft/versions` folder?

By default it is in `~/Library/Application Support/minecraft/versions`

## How can I gen a ARM Java Machine?

1. Install Homebrew for ARM
2. Execute in terminal `brew install openjdk`
3. By default, the java path is `/opt/homebrew/opt/openjdk/bin/java`

## What does it change respect to the original?

It is the same minecraft except:
* Library `lwjgl` is updated from 3.2.1 to 3.3.0 (required to work in arm64)
* Library `java-objc-bridge` is updated from 1.0.0 to 1.1 (required to work in arm64)
* Library `log4j` is updated from 2.14.1 to 2.17.1 (not necessary)

## Future updates?
* Compatibility with fabric
* Compatibility with new Minecraft versions until Microsoft/Mojang release a native version.

## Does it work online or with my current world?

Sure!