
### Fix update v0.1.5.0

#### Creating a new installation

In the panel, in the `Games` tab, create a new Palworld installation (your current data will be retained).

Modify the active installation for the new installation and restart the server once.

#### Recovering the backup of the old installation

Switch off the server. 

In FTP access, copy the _content_ of the old installation's backup folder and paste it into the new installation's backup folder.
Do NOT copy the folder itself.

If the old backup folder is
> 42679FFB7E0B4775A46948D3E6238455

and the new installation folder is
> A308DA0E450C4734BF7224FAA288A9E3

You need to copy the files 
 - 42679FFB7E0B4775A46948D3E6238455/Players
 - 42679FFB7E0B4775A46948D3E6238455/Level.sav
 - 42679FFB7E0B4775A46948D3E6238455/LevelMeta.save

in the folder `SaveGames/0/A308DA0E450C4734BF7224FAA288A9E3`.

When the copy is complete, you can restart the server.

#### Progress retrieval (must be done by each player)

Progress data (tutorial, map discovery) is saved on the client side (on the player's computer). Each player must do the following if they wish to keep their progress.

Connect to the server once so that the game can create the folder with the progress on the new server game installation, then close the game.

Open the folder `C:\Users\{User}\AppData\Local\Pal\Saved\SaveGames\{Palworld-user-ID}` in which `{User}` match to your Windows session name `{Palworld-user-ID}` to your Palworld id.

In this folder you'll find a file for each server installation to which you've connected.
To find out which file is which, compare the modification dates.
If you haven't connected to any other servers since the update:

 1. The most recently modified folder corresponds to the data of the new installation on the server. Rename it by adding a recognizable prefix or suffix (underscore, date or other).
 2. The second most recently modified folder corresponds to data from the old installation on the server. Copy it and rename the copy with the name of the new folder.

You can now reboot your game and connect to the server.

![Client-side handling explained in image](../img/Update_0.1.5.0_clientside.png?raw=true)
