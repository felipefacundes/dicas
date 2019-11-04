# PlayOnGit Installation Process 🕹

**Attention: READ, there are three Gifs below. Read, and see the Gifs.**
<br></br>

See **Gif** for a **notion** of how to **install** the desired **Game** (or Windows software). **REMEMBERING THAT GIF IS FOREIGNALLY EXAMPLE.** WHAT IS, IT FITS EVERYTHING ON PLAYOnGIT. **JUST ADAPT THE CONCEPT.**

![Tuto install](https://raw.githubusercontent.com/felipefacundes/desktop/master/wine-jogos/imagens/TuToinst.gif)

**See how easy it is**. Just copy the entire command line and paste it into **terminal**: hit ENTER, and you're done. Game installed, ready to use: right in the start menu> games.

<br></br>
**If you need to** install the game from your hard drive, because you already have it, and don't want to download it again. Just go to **PlayOnGit** in the part:

###### "Opcional para quem quiser fazer alterações"

Copy the command: **xdg-open ~/.jogos/scripts/run/...** for your game. And make changes to the installer path and executable to install. Know, that the script is high explanatory, is EASY. After installing **change again**, this time enter the path of the executable already installed. **DO NOT forget to SAVE (Ctrl + s)**. See this other **Gif** below, look how easy:

![Tuto install manual](https://raw.githubusercontent.com/felipefacundes/desktop/master/wine-jogos/imagens/TuToinst_manual.gif)

<br></br>
All **PlayOnGit** Game installations will show the option to enable **Virtual Desktop**. This option is important as it becomes more compatible with games, eg GTA San Andreas, only runs on Virtual Desktop. Not to mention, enabling this option makes it easier to close your games with the keyboard shortcut: Alt + F4, making your gameplay extremely efficient. So it's always worth enabling this option on the **Graphics Tab** as shown in the Gif below.
![Desktop Virtual](https://raw.githubusercontent.com/felipefacundes/desktop/master/wine-jogos/imagens/Desktop_Virtual.gif)

**If you want to delete the "Wine" menu from your "start menu"** DO THE FOLLOWING:

```
rm -rf ~/.local/share/applications/*wine*
```

**To kill the process of a Windows game or software** RUN THE FOLLOWING COMMAND:

```
bash -c "pkill -9 .exe; pkill -9 wine; pkill -9 wineserver"
```
