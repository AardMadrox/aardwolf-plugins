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
| **PupPaths** | Step-by-step pup pathing with named, saved routes. `pp list` opens a window to add, edit and delete paths. |
| **ChaosCast** | Tracks chaos-portal casts (normal vs golden). |
| **MarketWatch** | Watches the marketplace and the live auction/market channels for items on your list and gives you a one-click bid or buyout up to a maximum price you set per item (`marketw`), optionally as a pop-up window (`marketw popup on`). A watch-list window (`marketw win`) lets you edit each item, set its three max bids, and switch it between market, auction or both. |
| **Nokfah's Dull with Epic Bonus Reward tracking** | Character development tracker (`dull`) — session/lifetime XP, gold, QP, trains, TP, epics, and per-epic lifetime reward records (`dull epic<name>`). Campaign and quest reports show your best and average time **for the level you took it at** (`[lvl 134 best 1m 32s | avg 2m 57s]`), read from Search and Destroy's history if you have it installed. Modified from Nokfah's DullTracker. |
| **RetreatFnSucks** | Retreat in one direction and keep retrying it on every `You FAIL to retreat!` (`re` `rw` `rn` `rs` `ru` `rd`), with on/off (`ret`) and a quiet mode (`retsilent`). ⚠️ New — still needs live testing. |
| **PKReport** | A PK Alert system for when you can't fight your own battles. When someone attacks you, it reports who, the area and the room (`PK Alert: Name has attacked me in Area - Fury City pkvnum[45682]`) to any of spouse, group or clan chat you switch on (`pkr spo on`, `pkr gt on`, `pkr clan on`; all off = a local echo only). Anyone else running PKReport sees the report as a clickable link that walks them straight to you with `mapper goto`. `pkr` shows help and which channels are on. ⚠️ New — still needs live testing. |
| **MazeMobber** | Solves the shuffling mazes in twenty-two areas and walks you to what matters in them: **Prosper** (the 201 theater and the Sea Witch), **Gauntlet**, **Gwillimberry**, **Nenukon**, **Xylmos**, **Helegear**, **Infamy**, **Sahuagin**, **Darklight**, **Times of Old**, **Promises**, **Rhodus**, **Astral**, **Fairy Tales 1**, **Scarred Lands**, **Nottingham**, **Deadlights**, **Mayhem**, **Sundered Vale**, **Gallows**, **Gold Rush** and **Mount duNoir**. Three commands: **`mm`** puts up a clickable list for whichever one you are standing in — mobs to hunt, rooms to walk to — and it walks the whole way; **`mmr`** picks a run back up after a fight or a warded door stops it; and **`mmout`** (or `mmo`) leaves by the nearest way out, with `mmout <area>` naming one you are not in. The list opens in a small scrolling window — when you walk in and every time you type `mm` (`mm window` switches it back to the main window, `mm win` reopens it any time; it closes itself when you leave the area, and `mm font` / `mm fontsize` change its font); `mm list` stops an area putting its list up on arrival, and `mm areas` lists every area with a switch so you can turn MazeMobber off in the ones you would rather it left alone. Outside all of them, `mm` lists the areas it works in - click one to be taken there. Scans where a mob scans, reads the room where it does not, never walks into a wall or out of the maze, and only searches the rooms a mob actually uses. `mm help` lists every area and the word that names it - areas are arguments, not commands of their own: `mm gaunt`, `mm prosper 3`, `mmout gwill`. |
| **BlootReport** | Allows you to set what bloot to ID into a mini window. With options to keep, or unkeep. Requires ID wish for now.
| **BlackClawCrag** | Modified version of Casteil's.
| **PortalMapper** | Lets you point to a bag, and then it maps all portals to mapper. Will set up dualweap if no wish, and wearportal if you have wish, or use custom mode to write the exact command yourself so it matches portals you already mapped. Optional start bag / end bag: put unmapped portals in the start bag and they move to the end bag once mapped. Note: it enters every portal to map it, so be careful with higher level portals.
| **RankTracker** | Shows your top 100 rankings, shows those around you, and shows top 10 in ranks. Works on channels as well.
| **Target** | Reports where you are, and what you are fighting, to a channel: `target say`, `target gt`, `target ft`, `target clan`, `target reply` or `target spo`. In a fight it sends `[Target Report] Enemy: [the Fractal Anomaly] \| HP: [14%] \| Area: fractal \| Room: Fractals of the Weave \| vnum: [40600]`, with the mob's name (in its own colours, if it has any), its health left, the area, the room name and room number. Out of combat it sends the same line without the enemy and HP. It is all read live from GMCP. `target` shows help. |
| **Finger Notes** | Keep your own note on any player and see it at the bottom of their `finger`, online or offline. `fnote <player> <note>` adds or replaces a note, `fnote <player>` shows it, `fnote clear <player>` removes it and `fnote list` shows them all. Long notes wrap to fit the finger box. Notes are saved in `FNotes_data.txt` beside the plugin. |
| **Gradients** | Reworked version of Orphean's Gradients plugin, with a new color scheme and a character limit added. Make and save color gradients, then send them to any channel or tell. `grad100 send freshness say The Coolest Sword Ever` fades your text through the `freshness` gradient and keeps the whole string to 100 characters or fewer, counting color codes, spaces and the closing `@w`, using fewer color steps if it has to. Any limit works, such as `grad80` or `grad50`. `string @x99H@x45i@w` doubles every `@` and copies it to your clipboard, ready to paste. Start with `grad list` and `grad help`. Comes with four starter gradients.
| **PotAndPapers** | Scribe scrolls and brew potions in batches from your own saved profiles. `pnp config` opens a window where each profile has its own command, Scribe or Brew, the spell, how many spells go on each scroll or potion (1x to 4x), how many to make, and a command to run when the batch is done (`sleep` by default). Click any value to change it, and add spells of your own to the list. Type a profile's command to make a batch: `sinc` makes its usual number, `sinc 8` uses 8 blank scrolls, made or failed, like Alchemist did. Each one counts down as it goes (`Making 5 of 8`, then `Scribe 3xIncomp made   Batch 5/8, 3 made 60.0%`), a lost concentration is retried for you, running out of mana pauses the batch and sleeps (`sleepx` or `sleep`, set with `pnp mana`) and it carries on by itself when you wake, and the results add up per batch, per session (every batch until an hour after your last spell, or `pnp end`) and over each profile's lifetime. Replaces Nok3_Alchemist, so remove that one first. Brewing has not been tested live yet. |
| **Partroxis** | Walks you through the Partroxis maze. Type `psx` at the maze door for a clickable list of every room and the mob in it, then click one and it walks you there, one exit at a time, with a short pause in every room so it never runs past the one you picked. Wrong exits are learned and doubled back from, and it reads your affects and casts any missing invis / sneak / hide before it sets off. If you are attacked the walk stops; once the fight is over type `psxgo` to carry on. `psx stop` stops a walk and `psx help` lists the rest. Room and mob data from Galaban's Partroxis plugin. |
| **IMPGoals** | Set goals for your Instinct, Mastery and Potential and see what it costs to reach them. `imp config` quietly reads all three (none of the game output shows) and opens a window with every current level and a box beside each one: click a box and type your goal. `impgoals` re-reads your levels and echoes the cost of each section and the total; `impgoals gt` (or `say`, `reply`, `spo`, `ft`, `clan`) sends it as one line: `[IMPGoals] Instinct (Dodge 139>140): 3,675 trains, 15,900,000 gold \| Mastery (Electric 175>200): 96,000 QP, 1,218,750,000 gold \| Potential (275>300): 267,500 QP \| Total: 363,500 QP, 3,675 trains, 1,234,650,000 gold`. Costs run from your current level to your goal at full price; the QP, gold and trains you already have are not taken off. `impgoals help` shows help. |
| **ReportID** | Reports an item's identify stats on one line, to yourself or any channel: `rid obsidian spouse` sends `a jagged shard of obsidian [3976940213] [lv290] [wield] [843dam -30] [740pts] [10str 10int 1wis 11dex 10con] [16dr] [150hp] [10mental]`. Weapons show how far their average damage is above (`+42`, green) or below (`-30`, red) an aard weapon of the same level (level x2.5 up to 79, x3 from 80, and 287 to 291 all count as 291); every weapon you identify also gets that number added on its Average Dam line, keeping the box lined up. `rid bag <bag id> [channel]` reports a whole bag, `rid id \| spell \| lore` picks how to identify, `rid help` shows help. Rewritten from Nokfah's Report Identify, so remove that one first. |
| **Keycheck** | All-around key manager for your keyring. `keycheck` opens a window of every key on your list: missing keys first in red, keys melting within 20 hours in pink, the time left on each, and a `[go]` link that walks you to where the key comes from. Two tabs, 201 and Sub, and it opens the one for your level. Every key has its own number (201 keys 1-100, Sub keys 101-200). `keyrecord`: stand where a key comes from, type it, then get the key - looted, picked up, stolen, bought or handed to you - and it is added with that room; passes count too. If Search and Destroy has seen the mob in more than one room, it is treated as a wanderer and `[go]` takes you to the area's first room instead; `keyroom <#> area` does the same for any key by hand. Getting any key on your list puts it straight on your keyring, and the keyring's reply shows as a green `Key Added` (it brings its own `krk` = `keyring replace key`). `warnkey <#>` watches a key: under 20 hours left you get a `[Gather Keys]` warning, repeated every 2 hours until you replace it. Each row also has `[remove]` (take it off the keyring) and `[delete]` (drop it from the list). Your list is saved in `Keycheck_data.lua` in your MUSHclient folder (safe to edit by hand any time; the plugin reads your changes in before it next saves); a new install starts with two example keys. `keycheck help` lists everything. |

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
