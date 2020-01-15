---
layout: default
title: The Heavy Door Creaks as You Push It Open…
date: 2020-01-15 09:00:00 -0700
---

# Hi There!

Here's an inaugural post for a blog to chronicle the development of the Zagnok project. It's mostly to help me remember and document stuff, but you're welcome to follow along if you like!

The idea for Zagnok began as a hackathon project I worked on with my sister. We were big into Slackbots and big into being nerds, so we decided to try writing a bot that acted as a sort of DM for Slack-based D&D/Pathfinder-style encounters.

Which is pretty much the most productive way possible to use Slack, and I'm sure exactly what was envisioned for the product.

# Vision

Our goal with future versions is to implement an API that can be used to track encounter state: Things like turn order, character status, monster health, etc. This API could be put to any number of novel uses; in parallel I'm working on a project for displaying various monster details.

We were able to get _something_ playable and fun within a single day for the hackathon, but it forced to the surface something that is paradoxically easy to overlook when playing a tabletop RPG: It turns out that role-playing games are quite data-heavy. In order to facilitate an immersive experience, we were going to need data. A lot of it. Monsters! Spells! Items! Turn rules! But from where..?

Enter the [Open Game License](https://en.wikipedia.org/wiki/Open_Game_License). The Pathfinder RPG core rules and such are released under the OGL, which allows certain portions of game info to be reproduced as long as the reproduction/derivative work is released under the same terms. It makes the distinction between a game's "open content" (or "OC") and its "product identity" ("PI" for short). Open content is, for example, what makes Pathfinder **a game** - rules and mechanics, basic monster info, etc. Product identity is the copyright-able stuff that makes a game **Pathfinder** - the world of Golarion, artwork, iconic characters like Ezren and Merisiel, and Adventure Path storylines, for example. This fits our needs very well as we mostly want _all the stats_.

As it happens, the data-conversion aspect is what I'm finding most interesting at this point. I haven't found a top-notch resource like the one I hope I'm building - they all seemed out-of-date, proprietary, or clunky and web-only. Decent enough  at best for reference, but not useful at all for automation. My goal is to create a robust way to parse the official OC sources and transform them into something usable for a data-driven RPG experience. Or an RPG-driven data experience. User's choice if the API is good, right?
