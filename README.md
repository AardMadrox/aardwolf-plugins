# Aardwolf MUSHclient Plugins

A collection of plugins I wrote for the [Aardwolf MUD](https://www.aardwolf.com/)
running under [MUSHclient](https://www.gammon.com.au/mushclient/). Each plugin is a
self-contained `.xml` file in the [`plugins/`](plugins/) folder.

## Plugins

| Plugin | What it does |
| --- | --- |
| **PortalValue** | Finds the closest saved portal to a room and shows the value of a portal to it. |
| **PortalUse** | Tracks how often you use each worn portal, with a top-usage list (`portalusetop`) and an optional destination area + landing room lookup. |
| **FHX** | Repeatedly casts `incomp` on yourself or others until healed; `hx` casts once; queues commands typed in combat; optional auto-heal after each fight. |
| **PupPaths** | Step-by-step pup pathing with named, saved routes. |
| **ChaosCast** | Tracks chaos-portal casts (normal vs golden). |
| **FractalReport** | Tracks Fractal run rewards and reports them to a channel. |
| **TEDReport** | Times TED (Fury) runs and reports trains/gold/TP rewards. |
| **MatronReporter** | Times Matron Dragon runs and reports rewards. |
| **SKDReport** | Times SKD runs and reports trains/gold/TP/Repop Token/Sigil rewards. |
| **SKDMoonlight** | Finds the good moonlight room during the SKD taunt phase (`ml` / `mlf`). ⚠️ New — still needs live testing. |
| **MarketWatch** | Watches the marketplace and the live auction/market channels for items on your list and gives you a one-click bid or buyout up to a maximum price you set per item (`marketw`), optionally as a pop-up window (`marketw popup on`). |
| **Nokfah's Dull with Epic Bonus Reward tracking** | Character development tracker (`dull`) — session/lifetime XP, gold, QP, trains, TP, epics, and per-epic lifetime reward records (`dull epic<name>`). Modified from Nokfah's DullTracker. |
| **RetreatFnSucks** | Retreat in one direction and keep retrying it on every `You FAIL to retreat!` (`re` `rw` `rn` `rs` `ru` `rd`), with on/off (`ret`) and a quiet mode (`retsilent`). ⚠️ New — still needs live testing. |
| **MazeMobber** | Solves the shuffling mazes in thirteen areas and finds what is in them: **Prosper** (the 201 theater maze), **Gauntlet**, **Gwillimberry** (Botanical Gardens), **Nenukon**, **Xylmos** (Rose Ether), **Helegear**, **Infamy** (three levels), **Sahuagin**, **Darklight** (Skullgore Plains), **Times of Old** (the Cindery Village), **Promises** (the ocean off Westport), **Rhodus** (the Nixie rebellion) and **Astral** (the Chamber of Destiny and the nightmare behind it). Three commands: **`mm`** puts up a clickable list for whichever of them you are standing in — mobs to hunt, rooms to walk to — **`mmg`** carries on, and **`mmout`** (or `mmo`) leaves by the nearest way out. It walks the whole way by default; `mmslow` makes it one room per press, `mmr` resumes after a fight, and `mm list` stops an area putting its list up on arrival. Scans where a mob scans, reads the room where it does not, reads the exit listing where the room names its exits, and only searches the rooms a mob actually uses. `mm help` lists every area and the word that drives it. |

## Easiest way to install & stay updated: the Plugin Manager

Install **`Madrox_PluginManager.xml`** once (see steps below), then just type
**`mpm`** in the MUD. You'll get a clickable list of all the plugins with
**Install / Update / Reload / Remove** buttons and version indicators, so you can
grab new ones and keep existing ones current without touching files by hand.

- `mpm` — show the list
- `mpm updateall` — update everything that's out of date
- `mpm selfupdate` — update the manager itself
- `mpm help` — full command list

## Installing a plugin (manually)

1. Download the `.xml` file you want from the [`plugins/`](plugins/) folder
   (open the file, then click **Download raw file** / the download icon).
2. Put it in your MUSHclient plugins folder, usually:
   `C:\MUSHclient\worlds\plugins\`
3. In MUSHclient, open the **Plugins** dialog (File menu &rarr; **Plugins...**),
   click **Add**, browse to the file, and open it.

   *Or* just drop the file into the plugins folder above and reconnect — many of
   these load automatically if MUSHclient is set to do so.

## Notes

- Written for the Aardwolf MUD specifically; they rely on Aardwolf's GMCP data and
  command output, so they won't work as-is on other MUDs.
- Use at your own risk. These follow Aardwolf's rules (no true automation /
  botting), but you're responsible for how you use them.

## License

Released under the MIT License — see [LICENSE](LICENSE). You're free to use, modify,
and share these; attribution is appreciated but not required.
