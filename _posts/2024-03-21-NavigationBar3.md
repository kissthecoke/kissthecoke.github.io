---
title: NavigationBar3
categories: Doc_Flutter, widgets
tags: NavigationBar3
---
NavigationBar3

### [https://api.flutter.dev/flutter/material/NavigationBar-class.html](https://api.flutter.dev/flutter/material/NavigationBar-class.html)

This example shows a [NavigationBar](https://api.flutter.dev/flutter/material/NavigationBar-class.html) within a main [Scaffold](https://api.flutter.dev/flutter/material/Scaffold-class.html) widget that's used to control the visibility of destination pages. Each destination has its own scaffold and a nested navigator that provides local navigation. The example's [NavigationBar](https://api.flutter.dev/flutter/material/NavigationBar-class.html) has four [NavigationDestination](https://api.flutter.dev/flutter/material/NavigationDestination-class.html) widgets with different color schemes. Its [onDestinationSelected](https://api.flutter.dev/flutter/material/NavigationBar/onDestinationSelected.html) callback changes the selected destination's index and displays a corresponding page with its own local navigator and scaffold - all within the body of the main scaffold. The destination pages are organized in a [Stack](https://api.flutter.dev/flutter/widgets/Stack-class.html) and switching destinations fades out the current page and fades in the new one. Destinations that aren't visible or animating are kept [Offstage](https://api.flutter.dev/flutter/widgets/Offstage-class.html).

### Click NavigationBarExampleApp3 and Test

<iframe src="https://kissthecoke.github.io/doc_flutter_samples//" style="width:650px;height:600px;border:1px solid gray"></iframe>

### Dart Pad

<iframe src="https://dartpad.dev/?id=057983d825a71b07a2ce115760bd6038" style="width:100%;height:800px;border:none"></iframe>

### Source Code

<script src="https://gist.github.com/kissthecoke/057983d825a71b07a2ce115760bd6038.js"></script>
