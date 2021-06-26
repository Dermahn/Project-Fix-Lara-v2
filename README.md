# TRLE - Project Fix Lara <!-- omit in toc -->

This project aims to fix all of the little bugs and oddities in Lara's animations. It should be used as the basis for every new project before Lara's animations are altered in any way.

# Table of contents <!-- omit in toc -->
- [1. Installation](#1-installation)
	- [1.1. Copying Lara's Animations](#11-copying-laras-animations)
	- [1.2. Copying Shotgun Animations](#12-copying-shotgun-animations)
	- [1.3. Copying Torch Animations](#13-copying-torch-animations)
	- [1.4. Applying FLEP Patches](#14-applying-flep-patches)
	- [1.5. Using TRNG Scripts](#15-using-trng-scripts)
- [2. FAQ](#2-faq)
	- [2.1. Why do I need to use Tomb Editor for this?](#21-why-do-i-need-to-use-tomb-editor-for-this)
	- [2.2. Do I need to use TRNG for this?](#22-do-i-need-to-use-trng-for-this)
- [3. Note about encryption](#3-note-about-encryption)
- [4. See also](#4-see-also)

# 1. Installation
Download the [latest release](https://github.com/Dermahn/Project-Fix-Lara-v2/releases/latest).

## 1.1. Copying Lara's Animations
There are two ways to copy Lara's main animations into you WAD.  
For the first method, simply open your level WAD as "destination" WAD on the left side, and the Fix Lara WAD as "source" WAD on the right side.
Then copy **LARA** from [wad\fixlara.wad2](wad/fixlara.wad2) into your level WAD.

The second method requires no WAD editing. Simply load [wad\fixlara.wad2](wad/fixlara.wad2) as additional WAD in Tomb Editor. Make sure that it is the first WAD in the list, so it overwrites any duplicate **LARA** object you might have in other WADs.

## 1.2. Copying Shotgun Animations
The Shotgun requires some additional work if you're **not** using the default Lara skin in your level.
1) Load [wad\fixlara.wad2](wad/fixlara.wad2) in WadTool and open **SHOTGUN_ANIM**.
2) Select **(2) SHOTGUN_RELOAD** and **(5) SHOTGUN_IDLE_TRANSITION**, then go to **Animation -> Export...**
3) Now, load your level WAD and open **SHOTGUN_ANIM**.
4) Go to **Animation -> Import...** and replace the same animations we just exported. **(5) SHOTGUN_IDLE_TRANSITION** doesn't exist by default, so you'll have to add a new empty animation before you import it.

## 1.3. Copying Torch Animations
The Torch requires some additional work if you're **not** using the default Lara skin in your level.
1) Load [wad\fixlara.wad2](wad/fixlara.wad2) in WadTool and open **TORCH_ANIM**.
2) Select **(1) Animation 1**, then go to **Animation -> Export...**
3) Now, load your level WAD and open **TORCH_ANIM**.
4) Go to **Animation -> Import...** and replace the same animations we just exported.

## 1.4. Applying FLEP Patches
To be written...

## 1.5. Using TRNG Scripts
To be written...


# 2. FAQ

## 2.1. Why do I need to use Tomb Editor for this?
The only program that allows us to edit old WAD files is WADMerger, which has the unfortunate side effect that corrupts every animation a tiny bit. Using the new Wad2 format allows me to keep the animations in the best sate they can possibly be in.

## 2.2. Do I need to use TRNG for this?
Yes and no. The animations themselves can be used even with the original game engine. However, there are some tweaks that require TRNG specific features, such as scripting and plugins.


# 3. Note about encryption
A simple request:
> If you are going to **encrypt your levels**, then please **do not use this project**.

I don't agree with encryption for many reasons, and I'll just sum it up this way: when making your game, you're using software, assets, tutorials, advices, etc... which are all **community effort**. Community effort is what kept Tomb Raider level editing going after 20 years.

My project is following the same spirit. If you want to encrypt your levels, well it's your choice, but then I ask you to not use any of my stuff in it. Thank you.

# 4. See also

- [**TRLE - AOD Animations**][trle-aod_animations]

[trle-aod_animations]: https://github.com/Joey79100/trle-aod_animations
