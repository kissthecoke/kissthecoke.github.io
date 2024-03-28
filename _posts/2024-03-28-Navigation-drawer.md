---
title: NavigationDrawer
categories: Doc_Flutter, widgets
tags: NavigationDrawer
---
NavigationDrawer

### [https://api.flutter.dev/flutter/material/NavigationDrawer-class.html](https://api.flutter.dev/flutter/material/NavigationDrawer-class.html)

Material Design Navigation Drawer component.

On top of [Drawer](https://api.flutter.dev/flutter/material/Drawer-class.html)s, Navigation drawers offer a persistent and convenient way to switch between primary destinations in an app.

The style for the icons and text are not affected by parent [DefaultTextStyle](https://api.flutter.dev/flutter/widgets/DefaultTextStyle-class.html)s or [IconTheme](https://api.flutter.dev/flutter/widgets/IconTheme-class.html)s but rather controlled by parameters or the [NavigationDrawerThemeData](https://api.flutter.dev/flutter/material/NavigationDrawerThemeData-class.html).

The [children](https://api.flutter.dev/flutter/material/NavigationDrawer/children.html) are a list of widgets to be displayed in the drawer. These can be a mixture of any widgets, but there is special handling for [NavigationDrawerDestination](https://api.flutter.dev/flutter/material/NavigationDrawerDestination-class.html)s. They are treated as a group and when one is selected, the [onDestinationSelected](https://api.flutter.dev/flutter/material/NavigationDrawer/onDestinationSelected.html) is called with the index into the group that corresponds to the selected destination.

### Click NavigationDrawer and Test

<iframe src="https://kissthecoke.github.io/doc_flutter_samples//" style="width:650px;height:600px;border:1px solid gray"></iframe>

### Dart Pad

<iframe src="https://dartpad.dev/?id=8ce5c19d1e4c2f8cdd4cd97c7d769388" style="width:100%;height:800px;border:none"></iframe>

### Source Code

<script src="https://gist.github.com/kissthecoke/8ce5c19d1e4c2f8cdd4cd97c7d769388.js"></script>
