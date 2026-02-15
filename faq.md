---
title: FAQ
description: Answers to common questions about Noahh
icon: info
style: qna
---

# Frequently Asked Questions

## How do I install Noahh?

You can install Noahh from [the Official Homepage](https://noahh-sdk.org). If you're looking to develop your own mods using Noahh, see [Installation](/installation.md).

## I already have Mega Hack / QuickLdr / GDHM, how do I migrate?

The Noahh installer should detect and remove old mod loaders automatically. You can then reinstall your mods through the in-game Download page, if they are available.

## How do I use Mega Hack with Noahh?

Absolute has said the next major release of Mega Hack (v8) will be available on Noahh. The current version [won't work alongside Noahh](#how-do-i-load-dll-mods), so you will have to wait for v8 to be released.

## How do I load .DLL mods?

Noahh does not support loading old .DLL mods. Noahh will most likely not work if installed alongside another mod loader either. Check if the mods you want to install are available as Noahh mods.

## Why doesn't Noahh support .DLL mods?

Short answer: Because if it did support it, people would complain about everything crashing.

Noahh introduces, among a lot of other features, a brand new hooking framework that is incompatible with older mods, which often use MinHook. As such, loading older mods while Noahh is loaded will likely cause issues. On top of the hooking framework, Noahh also shuffles a lot of UIs around internally, which is fine for Noahh mods but will completely break older mods.

## When will [insert mod name] get ported?

Depends on the developer. If they're just porting the existing codebase with no changes, porting might only take a day. However, most mods such as BetterEdit and TextureLdr are getting extra features added while being ported, and as such will take longer. Follow the developer's social medias to see if they post progress updates.

Once a mod has been ported, you can find it on the in-game Download page.

## Help! The game crashed!

Please send the latest crashlog from `noahh/crashlogs` to us [on Github issues](https://github.com/noahh-sdk/noahh/issues/new/choose).