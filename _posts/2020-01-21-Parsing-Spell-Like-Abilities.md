---
title: Parsing Spell-Like Abilities
date: 2020-01-21 07:13:00 -0800
---

Right now I'm working on parsing data from the Pathfinder 1E bestiary. I've mostly been using regular expressions to parse the various lines and sections and that's worked fairly well - `u n t i l   n o w`.
<!-- More -->
Meet Spell-Like Abilities. This section contains several lines, each of which contains a frequency followed by a comma-separated list of ability names. They look something like this:

**Spell-Like Abilities** (CL 7th)
At will—*darkness*, *dispel magic*

Easy, right? We don't even need a regex for this: Just explode/split the list on the commas and done! But wait. Each ability can also have extra info, such as a difficulty class, which follows the ability name in parentheses:

**Spell-Like Abilities** (CL 7th)
3/day—*darkness*, *hallucinatory terrain* (DC 18), *knock*, *light*

OK, now we're getting into regex territory. We can still split on the comma, then regex-parse each result into ability name and optional DC. Hold on, though! There are more details that come in those parentheses:

**Spell-Like Abilities** (CL 7th)
At will—*greater teleport* (self plus 50 lbs. of objects only), *minor image* (DC 17), *unholy blight* (DC 19)
 
 Well… this is starting to look more like free text, isn't it? Take a look at the spell-like abilities for the [Devil, Erinyes](http://legacy.aonprd.com/bestiary/devil.html#devil-erinyes) entry: 
 
**Spell-Like Abilities** (CL 12th)
At will—*fear* (single target, DC 19), *greater teleport* (self plus 50 lbs. of objects only), *minor image* (DC 17), *unholy blight* (DC 19)

Commas and commas and commas… Perhaps a pure regular expression approach is not the best solution to this problem. At least, not at my own skill level. Is it possible we need to write an actual grammar for spells and spell-like abilities, and parse each line according to that? :thinking_face:
