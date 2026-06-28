# Aardwolf MUSHclient Plugins

A collection of plugins I wrote for the [Aardwolf MUD](https://www.aardwolf.com/)
running under [MUSHclient](https://www.gammon.com.au/mushclient/). Each plugin is a
self-contained `.xml` file in the [`plugins/`](plugins/) folder.

## Plugins

| Plugin | What it does |
| --- | --- |
| **PortalValue** | Finds the closest saved portal to a room and shows the value of a portal to it. |
| **FHX** | Repeatedly casts `incomp` on yourself or others until healed. |
| **PupPaths** | Step-by-step pup pathing with named, saved routes. |
| **Pot_miniwindow** | Tracks your available potions in a small on-screen window. |
| **ChaosCast** | Tracks chaos-portal casts (normal vs golden). |
| **FractalReport** | Tracks Fractal run rewards and reports them to a channel. |
| **TEDReport** | Times TED (Fury) runs and reports trains/gold/TP rewards. |
| **MatronReporter** | Times Matron Dragon runs and reports rewards. |
| **SKDReport** | Times SKD runs and reports trains/gold/TP/Repop Token/Sigil rewards. |

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
