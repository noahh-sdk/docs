![Noahh Logo](https://github.com/noahh-sdk.png?size=80) 

# Noahh SDK

**Noahh** is a [Geometry Dash](https://store.steampowered.com/app/322170/Geometry_Dash/) mod loader and modding SDK with a modern approach towards mod development. Unlike previous mod loaders, which merely inject the DLLs and let devs handle the rest, Noahh aims to be a more comprehensive project, which manages loaded mods & hooks itself. Noahh has been built to ensure performance, compatibility, portability and ease of use. For devs, Noahh means easy development and portability; for end users, Noahh means an uniform and easy experience using mods.

## Why Noahh?

The main goal of Noahh is to **end mod incompatability**. Traditional modding leads very easily to compatability problems, many of which Noahh attempts to address with better solutions.

On top of this, and perhaps more interestingly, **Noahh provides much better ergonomics for modding**. Instead of having to deal with calling conventions, trampolines, manually setting hooks (likely in another source file), you can have all the code relevant to hooks in a [nice, clean, readable syntax](/tutorials/modify.md) contained within a single source file.

See [What is Noahh](/whatisnoahh.md) for more detailed information about why you should use Noahh.

## Help, Contributing, Etc.

If you need help using Noahh or would like to contribute, feel free to join our [Discord Server](https://discord.gg/9e43WMKzhp).

Alternatively, if you hate joining Discord servers to work with a framework, you can also just **open up an issue or pull request** on any [Noahh repository on Github](https://github.com/orgs/noahh-sdk/repositories).

## Getting Started

See [Installation](/installation) for instructions on how to install the Noahh SDK on your computer.

See [Creating a new mod](/noahh/creating) for instructions on how to make your first mod.

See [Building](/source/building) for instructions on how to build the Noahh Loader + SDK from scratch on your computer.

See [Handbook](/handbook/chap0) for a beginner-friendly tutorial series on using Noahh and GD Modding in general (WIP!!).

## Credits

### Contributors

<a href="https://github.com/noahh-sdk/noahh/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=geode-sdk/geode" />
</a>

### Libraries

 * [Cocos2d-x](https://github.com/cocos2d/cocos2d-x/tree/cocos2d-x-2.2.3)
 * [FMOD](https://www.fmod.com/)
 * [fmt](https://fmt.dev/latest/index.html)

### Special Thanks

 * [NachoBIT](https://github.com/TheNachoBIT)
 * [RobTop Games](https://twitter.com/RobTopGames/) for making this amazing game and providing us and so many others with hours of entertainment ❤