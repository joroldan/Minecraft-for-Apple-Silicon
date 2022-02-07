# Minecraft for Apple Silicon
Minecraft 1.18.1 for Apple Silicon

## How to use it?

The way to use it, it is the same as [official 1.18 experimental snapshots](https://www.minecraft.net/en-us/article/new-world-generation-java-available-testing). There it is a [visual guide with pictures](https://images.ctfassets.net/8y6ykjruobr4/5npJyh6JAV5ShVPjnZ74wM/a10d21227d399e94c904526ce8c313db/how-to-install-experimental-snapshots.jpg) which can help you through this process.

1. Simply create a folder called `arm-1.18.1` inside your `minecraft/versions` folder and put [`arm-1.18.1.json`](https://github.com/joroldan/Minecraft-for-Apple-Silicon/blob/main/arm-1.18.1.json?raw=true) file inside.
2. Create a new launch installation in the launcher and select the "release arm-1.18.1" version
3. Below, in more options select a ARM Java Virtual Machine.
4. Play and enjoy!

## Where is my `minecraft/versions` folder?

In Finder, in the Go menu, select "Go to Folder" and enter `~/Library/Application Support/minecraft/versions`

## How can I gen a ARM Java Machine?

There are several ways. The recommended one is:

1. [Install Homebrew](https://brew.sh/) for ARM
2. Execute in terminal `brew install openjdk`
3. By default, the java path is `/opt/homebrew/opt/openjdk/bin/java`

## What does it change respect to the original?

It is the same Minecraft except:
* Library `lwjgl` is updated from 3.2.1 to 3.3.0 (required to work in arm64)
* Library `java-objc-bridge` is updated from 1.0.0 to 1.1 (required to work in arm64)
* Library `log4j` is updated from 2.14.1 to 2.17.1 (not necessary)
* Some Windows/Linux dependencies of `lwjgl` have been removed as they are unnecessary.

## Future updates?
* Compatibility with fabric
* Compatibility with new Minecraft versions until Microsoft/Mojang release a native version.
