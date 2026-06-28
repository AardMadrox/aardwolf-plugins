# Aardwolf MUSHclient Plugins

A collection of plugins I wrote for the [Aardwolf MUD](https://www.aardwolf.com/)
running under [MUSHclient](https://www.gammon.com.au/mushclient/). Each plugin is a
self-contained `.xml` file in the [`plugins/`](plugins/) folder.

## Plugins

| Plugin | What it does |
| --- | --- |
| **PortalValue** | Finds the closest saved portal to a chaos portal you just entered and shows the speedwalk to it. |
| **FHX** | Repeatedly casts `incomp` on yourself or others until healed. |
| **PupPaths** | Step-by-step pup pathing with named, saved routes. |
| **Pot_miniwindow** | Tracks your available potions in a small on-screen window. |
| **ChaosCast** | Tracks chaos-portal casts (normal vs golden). |
| **FractalReport** | Tracks Fractal run rewards and reports them to a channel. |
| **TEDReport** | Times TED (Fury) runs and reports trains/gold/TP rewards. |
| **MatronReporter** | Times Matron Dragon runs and reports rewards. |
| **SKDReport** | Times SKD runs and reports trains/gold/TP/Repop Token/Sigil rewards. |

## Installing a plugin

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
