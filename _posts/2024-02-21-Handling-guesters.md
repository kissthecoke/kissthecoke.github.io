---
title: Handling gestures
categories: Doc_Flutter, widgets
tags: Row
---
## Handling gestures

### [https://docs.flutter.dev/ui#handling-gestures](https://docs.flutter.dev/ui#handling-gestures)

### Click handling gestures and Test

<iframe src="https://kissthecoke.github.io/doc_flutter_samples//" style="width:430px;height:500px;border:1px solid gray"></iframe>

Most applications include some form of user interaction with the system. The first step in building an interactive application is to detect input gestures. See how that works by creating a simple button:

The [`GestureDetector`](https://api.flutter.dev/flutter/widgets/GestureDetector-class.html) widget doesn’t have a visual representation but instead detects gestures made by the user. When the user taps the [`Container`](https://api.flutter.dev/flutter/widgets/Container-class.html), the `GestureDetector` calls its [`onTap()`](https://api.flutter.dev/flutter/widgets/GestureDetector-class.html#onTap) callback, in this case printing a message to the console. You can use `GestureDetector` to detect a variety of input gestures, including taps, drags, and scales.

Many widgets use a [`GestureDetector`](https://api.flutter.dev/flutter/widgets/GestureDetector-class.html) to provide optional callbacks for other widgets. For example, the [`IconButton`](https://api.flutter.dev/flutter/material/IconButton-class.html), [`ElevatedButton`](https://api.flutter.dev/flutter/material/ElevatedButton-class.html), and [`FloatingActionButton`](https://api.flutter.dev/flutter/material/FloatingActionButton-class.html) widgets have [`onPressed()`](https://api.flutter.dev/flutter/material/ElevatedButton-class.html#onPressed) callbacks that are triggered when the user taps the widget.

For more information, check out [Gestures in Flutter](https://docs.flutter.dev/ui/interactivity/gestures).

### Source Code


<script src="https://gist.github.com/kissthecoke/a0e3a27224f28e9d74f171e6ad398e04.js"></script>
