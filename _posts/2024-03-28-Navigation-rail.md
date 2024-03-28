---
title: Navigation Rail
categories: Doc_Flutter, widgets
tags: Navigation Rail
---
Navigation Rail

### [https://api.flutter.dev/flutter/material/NavigationRail-class.html](https://api.flutter.dev/flutter/material/NavigationRail-class.html)


The navigation rail is meant for layouts with wide viewports, such as a desktop web or tablet landscape layout. For smaller layouts, like mobile portrait, a [BottomNavigationBar](https://api.flutter.dev/flutter/material/BottomNavigationBar-class.html) should be used instead.

A navigation rail is usually used as the first or last element of a [Row](https://api.flutter.dev/flutter/widgets/Row-class.html) which defines the app's [Scaffold](https://api.flutter.dev/flutter/material/Scaffold-class.html) body.

The appearance of all of the [NavigationRail](https://api.flutter.dev/flutter/material/NavigationRail-class.html)s within an app can be specified with [NavigationRailTheme](https://api.flutter.dev/flutter/material/NavigationRailTheme-class.html). The default values for null theme properties are based on the [Theme](https://api.flutter.dev/flutter/material/Theme-class.html)'s [ThemeData.textTheme](https://api.flutter.dev/flutter/material/ThemeData/textTheme.html), [ThemeData.iconTheme](https://api.flutter.dev/flutter/material/ThemeData/iconTheme.html), and [ThemeData.colorScheme](https://api.flutter.dev/flutter/material/ThemeData/colorScheme.html).

Adaptive layouts can build different instances of the [Scaffold](https://api.flutter.dev/flutter/material/Scaffold-class.html) in order to have a navigation rail for more horizontal layouts and a bottom navigation bar for more vertical layouts. See [the adaptive_scaffold.dart sample](https://github.com/flutter/samples/blob/master/experimental/web_dashboard/lib/src/widgets/third_party/adaptive_scaffold.dart) for an example.

### Click NavigationRailExampleApp_1 and Test

<iframe src="https://kissthecoke.github.io/doc_flutter_samples//" style="width:650px;height:600px;border:1px solid gray"></iframe>

### Dart Pad

<iframe src="https://dartpad.dev/?id=ad8a46a0c281936872420262b189a40e" style="width:100%;height:800px;border:none"></iframe>

### Source Code

<script src="https://gist.github.com/kissthecoke/ad8a46a0c281936872420262b189a40e.js"></script>
