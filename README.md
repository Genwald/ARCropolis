# ARCropolis

A Skyline plugin for replacing arbitrary files in Smash Ultimate with files of arbitrary size. Made in equal parts by Raytwo and jam1garner, with lots of help from Shadow as well.

### Installation

Copy the content of the zip from the latest release onto the SD so the plugin is in the following folder:

```
    sd:/atmosphere/contents/01006A800016E000/romfs/skyline/plugins/
```

### Usage

Place your files in the following folder:

```
    sd:/atmosphere/contents/01006A800016E000/romfs/arc/
```

For example, if you want to replace the file

```
    ui/message/msg_melee.msbt
```

you place it in

```
    sd:/atmosphere/contents/01006A800016E000/romfs/arc/ui/message/msg_melee.msbt
```

### Configuration

As of version 0.1.4, ARCropolis uses a configuration file that can be found here:

```
    sd:/atmosphere/contents/01006A800016E000/romfs/arcropolis.toml
```

If you do not have one, it will be created the next time you run Smash Ultimate, with a default configuration (The same one ARCropolis used prior to the use of a configuration file).

This configuration file is made in an effort to support workspaces generated by [Quasar](https://github.com/Mowjoh/Quasar) by [Mowjoh](https://github.com/Mowjoh), a mod downloader and manager for Smash Ultimate (and more!) with support for one-click download for GameBanana mods.

Even so, you can manually edit the configuration file using any text editor of your choice to change the directory where files and streams are read from.

Error messages have been added for most cases, so if you manage to butcher your configuration somehow, don't open an issue for it. Delete your configuration file and generate a new one. (ARCropolis will most likely do it in your stead if everything goes right)

### Auto-Update

As of version 0.9.0, ARCropolis comes with a auto-updater.

From now on, you might see a dialog on boot prompting you to update. You're free to refuse, but updates coming through this prompt should usually be well tested before being published.

You can also opt-in for beta builds for experimental features through your configuration file, which, while usually sufficiently tested, might still have some bugs while shipped. By default, the configuration is set to not use them.

### Ultimate Mod Manager Backwards Compatibility

The plugin also supports backwards compatibility with UMM paths to allow for mods to continue to work. You can simply rename your `UltimateModManager` folder to `ultimate` and all mods will work. If you no longer need UMM, it is recommended you delete your data.arc file from romfs.
