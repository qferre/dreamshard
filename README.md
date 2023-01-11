# Dreamshard RPG project 

A RPG system derived from the d20 framework, with its accompanying Lore. It uses a flexible classless system, with different degrees of success for the outcomes of rolls.

This is set in a low-fantasy late medieval universe, on the Dreamshard Archipelago, which was recently shaken by unexplained magical phenomena. This comes on top of an unstable geopolitical background, where powerful Magisters vie for influence. The players are mandated by the Imperial governor to investigate reports of activity from the fabled Voskari. What will you find, and should it have stayed in the shadows?


## Contents

This contains the full source code to re-create the rules manuscript.

- *main.tex* is the hub files, with the subfiles in the */tex* directory.
- Additonal elements in the the */incl* directory, including the character sheet template, an interactive table of roll modifiers, and a rules summary (in French).

The LibreOffice files here are in flat format. This takes more space, but makes them gittable.

A full compiled copy can be found at <https://drive.google.com/drive/folders/1TaOvkW6zsIso4MtEfzujdXoxl7g_9NPt?usp=sharing> and should be up to date, but when in doubt the version on this repository is more recent.

## Compiling

*The most recent release will always be on GitHub. Remember to git pull before doing anything!*

If you don't have LaTeX installed, the following command will work on Ubuntu:

```sh
sudo apt-get install texlive-full
```

You **must use LuaLaTeX** to compile this!

To recreate the files, run:
```sh
# Compile the manuscript
lualatex main.tex 

# Package it with the contents of the `incl` directory
tar -czvf dreamshard_release.tar.gz main.pdf incl/*
```


## Modifying


This work is published under the Creative Commons-BY license. As such, feel free to make any modification! That being said:

- Prioritize patching the balance in-game with Loot and Traits instead of modifying the manuscript itself.
- Remember to update the contents of */incl* when the rules change.


## Credits

Contact: <quentin.q.ferre@gmail.com>

Original repository link: <https://github.com/qferre/dreamshard>
