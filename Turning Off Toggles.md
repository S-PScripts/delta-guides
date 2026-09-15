# Disable Anti-Scam / Verify Teleports / Disable Robux
> ⚠️ Only turn Anti-Scam / Disable Robux / Verify Teleports off if you know what you're doing! <br>
> To learn more about these features, read https://docs.deltaexploits.gg/protections.

## UI Disable
> This only applies for one game. You must do these steps for every game you want to have the options off.
1. Remove or disable any scripts in your executor’s auto-execute (autoexec) folder.
> This prevents scripts from automatically running again when you rejoin.
2. Join the Roblox game where you want to disable the toggles. Do not execute anything.
3. Wait for the Delta UI to load (this may take a few seconds), then click the Delta icon and open settings (cog icon).
4. Toggle OFF the options you want to disable.
5. Wait about 10 seconds to ensure the settings are saved, then leave the game.
6. Wait another 10 seconds, then rejoin the game.
7. The options should now be disabled.

## ZArchiver Disable (Android)
1. Join a Roblox game.
2. Wait until the Delta UI loads. Exit out of Roblox afterwards.
3. Open ZArchiver. If you do not have it, install it from the Play Store.
4. Go to 0/storage/emulated.
5. Click on the Delta folder.
6. Click on "Internals".
7. Click on "Secured".
8. Click on the user_id file. Open with ZArchiver Text.
9. Copy the User ID that is in the file, then exit.
10. Click on allowrobux/allowteleports/disableantiscam (depending on which you want to disable). Open with ZArchiver text.
11. If it is not set already, change "user_id":"" to "user_id":"THE USER YOU COPIED IN STEP 7".
12. Change "allowed_games":"" to "allowed_games":"*".

> Example:
```
{
  "WARNING": "IF SOMEONE TELLS YOU TO PUT ANYTHING HERE, THEY ARE SCAMMING YOU! STOP!!!",
  "allowed_games": "*",
  "user_id": "10681452461",
  "version_num": 711
}
```
> Turning the toggle off for just a few games:
```
{
  "WARNING": "IF SOMEONE TELLS YOU TO PUT ANYTHING HERE, THEY ARE SCAMMING YOU! STOP!!!",
  "allowed_games": [
    3317679266,
    65241
  ],
  "user_id": "10681452461",
  "version_num": 711
}
```
13. Click the File Icon at the top right to save.
14. Go back and change the other two toggles if you want to (in the same way). That is all!
> Note: When Delta updates, you will need to update the "allowrobux" file as its contents will reset.

Delta also has a new file called "useraknet" for allowing you to use Raknet Desync. When allowed, you can run raknet.desync(true) to turn it on and raknet.desync(false) to turn it off. 
You can find its uses online.

**Please be aware that anti-scam and disable robux are NOT the same thing.**
