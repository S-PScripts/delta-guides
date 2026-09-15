Go here:

1. https://rscripts.net/
2. https://robloxscripts.com/
3. https://scriptblox.com (this is also what the cloud icon in Delta GUI uses)
4. https://haxhell.com

Search for a script, copy it, open Delta, click the game icon, and press "Execute Clipboard"

`print("denta")`

If you say that nothing AT ALL executes, copy this and execute clipboard. You should see "denta" in the developer console (type /console in chat). You can also try executing Infinite Yield.

Test Delta sUNC:
```
getgenv().sUNCDebug = {
    ["printcheckpoints"] = false,
    ["delaybetweentests"] = 0,
    ["printtesttimetaken"] = false,
}

loadstring(game:HttpGet("https://script.sunc.su/"))()```
