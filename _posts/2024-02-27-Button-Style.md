---
title: Button Style
categories: Doc_Flutter, widgets
tags: Row
---
## Bringing it all together

### [https://api.flutter.dev/flutter/material/ButtonStyle-class.html#material-3-button-types](https://api.flutter.dev/flutter/material/ButtonStyle-class.html#material-3-button-types)

### Click button style and Test

<iframe src="https://kissthecoke.github.io/doc_flutter_samples//" style="width:430px;height:500px;border:1px solid gray"></iframe>


The visual properties that most buttons have in common.

Buttons and their themes have a ButtonStyle property which defines the visual properties whose default values are to be overridden. The default values are defined by the individual button widgets and are typically based on overall theme's [ThemeData.colorScheme](https://api.flutter.dev/flutter/material/ThemeData/colorScheme.html) and [ThemeData.textTheme](https://api.flutter.dev/flutter/material/ThemeData/textTheme.html).

All of the ButtonStyle properties are null by default.

Many of the ButtonStyle properties are [MaterialStateProperty](https://api.flutter.dev/flutter/material/MaterialStateProperty-class.html) objects which resolve to different values depending on the button's state. For example the [Color](https://api.flutter.dev/flutter/dart-ui/Color-class.html) properties are defined with `MaterialStateProperty<Color>` and can resolve to different colors depending on if the button is pressed, hovered, focused, disabled, etc.

These properties can override the default value for just one state or all of them. For example to create a [ElevatedButton](https://api.flutter.dev/flutter/material/ElevatedButton-class.html) whose background color is the color scheme’s primary color with 50% opacity, but only when the button is pressed, one could write:

### Source Code


<script src="https://gist.github.com/kissthecoke/692d994a38afc41306925ac5868a0bad.js"></script>
