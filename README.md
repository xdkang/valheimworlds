=======
# valheimworlds

## What is this?
This is a repository for sharing Valheim world files across my friends so that my friends can play on each other's servers (most especially *mine*) without needing their respective hosts to be online to run the server.

## Where are my world files located?
World files can be found in `C:/Users/[user]/AppData/LocalLow/IronGate/Valheim/worlds`.

Take note that the `/AppData` folder is normally invisible so you'll have to type it into the URI bar manually while in your [user] folder.

Every Valheim world comprises two files, `[worldname].db` and `[worldname].fwl`, so we will only concern ourselves with these two files and nothing else.

## How do I obtain these files?
1. Download [Git](https://git-scm.com/downloads) if you don't already have it. Or go ahead and use Mercurial/Subversion/Azure/whathaveyou if you want.

2. Go to your `/worlds` folder and execute Git Bash or Git GUI, whichever you prefer. (For other VCS's I assume you already know what to do.)

3. Use this URL: https://github.com/xdkang/valheimworlds.git to clone this repo.

You should now have a local repo of this remote and an up-to-date copy of the files contained in this repo inside your folder.

## How do I add/update my world files here?
1. If you have your local repository already set up simply execute an `add` command for your `[worldname].db` and `[worldname].fwl` files while in your `/worlds` folder.

2. Then execute a `commit` command with a message (I typically write in this format -> [worldname] dd/mm/yy).

3. Finally, execute a `push` command.

The `[worldname].fwl` file appears to be static and likely contains simple metadata for the game to fetch the server, so it only needs to be added once, on the initial commit.

The `[worldname].db` file, however, gets locally updated constantly so this is the main file we want to push and pull all other times.

## How do I play on my friends' worlds?
If you have managed to do everything right and pulled the files into the right folder you'll be able to find the name of your friends' world in-game in the list of servers after the character select screen.

You can now host your friends' worlds and play in them while they're offline, but if they want to play while you are in the midst of hosting their world it is best that they join you in-game instead of starting their own instance.

Every time you finish playing in a friend's world (or your own world for that matter) do remember to update the `[worldname].db` file remotely as per the previous section.

## What do I do when other people add/update their files here?
When a friend has updated the `[worldname].db` file to their world remotely and you're about to host that world, simply execute a `pull` command while in your `/worlds` folder to update all the files locally.

If you're about to host your own world after a friend had been hosting it remember to first pull the `[worldname].db` file that your friend had (hopefully) updated.

## Get on my Discord!
I have a Discord server for chatting and communicating in-game.

Ping me on Facebook/Steam/wherever for a link to join my server.

## Help?!
If you get stuck or need guidance using Git let me know on Facebook/Steam/Discord and I'll do my best to assist.
>>>>>>> fd77a7e0ae55be5dd4d6238879b7861e7cc8e6f1
