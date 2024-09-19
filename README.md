# Picta Graphic Rename Plugin

## Table of Contents

- [About](#about)
- [Description](#description)
- [Installation](#installation)
- [Usage](#usage)

## About

This plugin for [Picta Graphic](https://graphic.com/) (formerly known as Autodesk Graphic or Indeeo iDraw) can rename multiple Graphic objects simultaneously.

Once installed, select an item, choose **Graphic > Plugins > Graphic iDraw Rename Selection**, and assign a new name. Note that every selected element will get the same name. Select **Edit > Undo Name** to revert the action.

Drawing applications like Picta Graphic often create documents with hundreds of objects and layers. To keep elements organized, you may need to assign recognizable names for each. By default, you can rename one item at a time. This plugin can rename all of them at once.

- Author: Jay Petronis
- Website: [https://arcplanning.com/]

## Features

- Rename multiple items quickly
- Works with objects, groups, and layers

## System Requirements

- Picta Graphic version 3.1 or later
- macOS Mojave (version 10.14) or later

## Installation

To install, double-click the file **`Graphic iDraw Rename Selection.idplugin`** to launch Graphic, which should then ask if you'd like to add the plugin to your Plugins menu.

### Plugin File:

![00-graphic-plugin-icon](img/00-graphic-plugin-icon.png)

### Add Plugin:

![01-graphic-plugin-install](img/01-graphic-plugin-install.png)

Or you can manually drag the file to its destination in Graphic's `Application Support` folder in your `Library` folder:

`~/Library/Containers/com.indeeo.idraw/Data/Library/Application Support/iDraw/Plug-ins/Graphic iDraw Rename Selection.idplugin`

## Usage

Open a document in Graphic, select one or more objects, groups, or layers, then choose **Plugins > Graphic iDraw Rename Selection**.

![02-graphic-plugin-run](img/02-graphic-plugin-run.png)

Then type in a new name and confirm the entry.

![04-graphic-rename-dialog](img/04-graphic-rename-dialog.png)

The new name will apply to every selected element, and the change should be nearly instantaneous.

![05-graphic-renamed-shapes](img/05-graphic-renamed-shapes.png)

The plugin works for groups and layers, too.

![06-graphic-renamed-layers](img/06-graphic-renamed-layers.png)

Select **Edit > Undo Name** to revert the change.

## Details

Feel free to change the plugin's filename at any time. Alternatives include:

- Graphic Renamer.idplugin
- GrafikUmbenennen.idplugin
- iDraw Renombrar Lote.idplugin

You can assign a custom keyboard shortcut to the plugin using **System Settings > Keyboard > Keyboard Shortcuts**, or with a third-party utility like Keyboard Maestro by Stairways Software:

https://www.keyboardmaestro.com/

The Graphic `idplugin` format is a JavaScript/CocoaScript file saved as plain text. Open it using any text editor to see how it works or make changes.

![07-script-content-example](img/07-script-content-example.png)

## Troubleshooting

If the plugin fails to load, ensure you have Picta Graphic version 3.1 or later installed.
macOS security settings may block the plugin. Check under **System Settings > Security & Privacy** if a prompt appears.

This plugin relies on Apple's [Cocoa APIs](<https://en.wikipedia.org/wiki/Cocoa_(API)>) and is not compatible with other platforms, such as Microsoft Windows. Additionally, it is only available in English and may exhibit anomalies when used with other language settings.

Graphic hasn't received updates since 2018, and might stop working in future macOS versions.

## Version History

2024-09-03

- Version 0.1: Initial release

## License

This work is dedicated to the public domain under the CC0 1.0 Universal (CC0 1.0) Public Domain Dedication.

## Support

For further information about Graphic plugins, visit:

- https://www.graphic.com/
- https://graphic.com/plugins/api
- https://www.graphic.com/docs/scripts
- https://github.com/ccgus/CocoaScript

Developed for Graphic 3.1 for macOS Sonoma 14.0.

2024-09-18
