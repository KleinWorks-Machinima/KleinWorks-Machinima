# KleinWorks Machinima

Welcome! KleinWorks Machinima is a Source Mod project dedicated to creating tools to aid in the creation of/special effects for Half Life 2 related machinimas.

Currently, this is entirely a passion project, so development may or may not be sporadic.


## Setting Up KleinWorks

The setup for getting KleinWorks Machinima to work is relatively simple, though if you are confused or encounter any problems with the installation of KleinWorks Machinima feel free to join our [Discord Server™](https://discord.gg/9asB83GFS) to ask for help.

For KleinWorks to function, you must first install Source SDK Base Singleplayer 2013, which should be in your Steam library under the 'tools' category, as pictured below:

![alt text](https://i.imgur.com/rnaI36a.png)

Source SDK Base Singleplayer 2013 ___needs___ to specifically be on the _upcoming_ beta branch, if it is not on the _upcoming_ beta branch then KleinWorks will crash to desktop on the main menu. To set the Source SDK Base Singleplayer 2013 to the _upcoming_ beta branch, right click on it in your library and open its _properties_, then under the _Betas_ tab of the properties window change _Beta Participation_ from None to _upcoming - upcoming_, as pictured below:

![alt text](https://i.imgur.com/hm38pJv.png)
![alt text](https://i.imgur.com/l6HWx04.png)

After you do that, you can download the latest version of KleinWorks Machinima from this github under [Releases](https://github.com/compact-colonist/KleinWorks-Machinima/releases). Inside of the release should be a folder named 'KleinWorks [version number]' and the EntRec Blender addon named 'kw_entrec_blender_addon', all you have to do is drag and drop the folder named KleinWorks into Steam's _sourcemods_ folder, which is under Steam->steamapps->sourcemods (example picture below). Restart Steam, and KleinWorks: Machinima should show up in your library.

![alt text](https://i.imgur.com/2JACBki.png)
![alt text](https://i.imgur.com/KlgIR3M.png)

Lastly, you need to install the EntRec Blender Addon, which is done like any other Blender addon: open Blender, go to Edit->Preferences, then under Addons click Install Addon and select 'kw_entrec_blender_addon.zip'.

__NOTE:__ The EntRec Blender addon REQUIRES the latest version of the [SourceIO](https://github.com/REDxEYE/SourceIO/releases) Blender addon to be _installed_ and _enabled_ to function properly.

Example photo for Blender 4.2 (layout may be slightly different for each Blender version):

![alt text](https://i.imgur.com/j42rIAQ.png) ![alt text](https://i.imgur.com/j6ojcc0.png)

# EntRec

__!WARNING!__: Entrec is early in development, and is therefor currently __unstable__. EntRec __may suddenly crash Blender straight to desktop without warning__ after being initialized, I will remove this warning when it's stable. Use with caution, save often!


EntRec is the first (and as of writing, the only) tool in Kleinworks Machinima. In short, it allows you to select entities in-game and 'record' them, sending things like positional data to Blender every tick, where it is then turned into a keyframe in an animation, effectively creating a 1 to 1 animation of the entity's movement in Blender.

The main purpose of this tool being to capture physics objects (such as props or ragdolls) for use in machinimas.


### Demonstration/How To Use

Heres a [link to a basic video demonstrating the successful use of EntRec](https://youtu.be/uBtXsWGtlJA)

This video roughly explains all of the features of KleinWorks Machinima as of v0.1. For indepth information on EntRec's functionality, visit the [Wiki](https://github.com/compact-colonist/KleinWorks-Machinima/wiki), everything should be kept up to date and explained in detail there.






# Contribution

Any and all contribution is welcome, so feel free to contribute anything you'd like to the code! If you'd like to contribute, you can also join the [Discord Server](https://discord.gg/9asB83GFS) and communicate your ideas or talk about the code with me or any other possible developers there.

Any modification to Mapbase code or Half-Life 2 source code by the Kleinworks Machinima project is marked by two code comments, enclosing where the modification begins and ends, for example:

```C++
/*========================*/
/*| KLEINWORKS™ ADDITION |*/

extern CzmqManager g_CzmqManager;

/*| KLEINWORKS™ ADDITION |*/
/*========================*/
```

Any new file created by the Kleinworks Machinima project is marked with a unique code comment header, optionally displaying who worked on the code in that file and what the purpose of the code is, for example:

```C++
//===================| PROPERTY OF THE KLEINWORKS™ CORPORTATION®® |===================\\
//
// Purpose: 
// 
// Product Contributors: Barber
//
//===================| PROPERTY OF THE KLEINWORKS™ CORPORTATION®® |===================\\
```

If you plan to contribute to Kleinworks Machinima, I would ask that you conform to this standard for the sake of tracking changes made to the original source code.

## Source Code Credit

KleinWorks Machinima uses [MapBase](https://github.com/mapbase-source/source-sdk-2013) as its SDK base, uses and contains binary files/code from various [ZeroMQ](https://github.com/zeromq) coding projects such as [libzmq](https://github.com/zeromq/libzmq), [cppzmq](https://github.com/zeromq/cppzmq) and [pyzmq](https://github.com/zeromq/pyzmq) to achieve Inter-Process-Commuinication, and uses [RapidJson](https://github.com/Tencent/rapidjson) as a format for Inter-Process-Communication messages.

Information on the licensing of these third party libraries can be found in this repo's LICENSE file.
