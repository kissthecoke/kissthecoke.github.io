---
title: Snack Bars
categories: Doc_Flutter, widgets
tags: Row
---
Snack Bars

### [https://api.flutter.dev/flutter/material/SnackBar-class.html](https://api.flutter.dev/flutter/material/SnackBar-class.html)

### Click Snack Bars and Test

<iframe src="https://kissthecoke.github.io/doc_flutter_samples//" style="width:430px;height:800px;border:1px solid gray"></iframe>


To display a snack bar, call `ScaffoldMessenger.of(context).showSnackBar()`, passing an instance of [SnackBar](https://api.flutter.dev/flutter/material/SnackBar-class.html) that describes the message.

To control how long the [SnackBar](https://api.flutter.dev/flutter/material/SnackBar-class.html) remains visible, specify a [duration](https://api.flutter.dev/flutter/material/SnackBar/duration.html).

A SnackBar with an action will not time out when TalkBack or VoiceOver are enabled. This is controlled by [AccessibilityFeatures.accessibleNavigation](https://api.flutter.dev/flutter/dart-ui/AccessibilityFeatures/accessibleNavigation.html).

During page transitions, the [SnackBar](https://api.flutter.dev/flutter/material/SnackBar-class.html) will smoothly animate to its location on the other page. For example if the [SnackBar.behavior](https://api.flutter.dev/flutter/material/SnackBar/behavior.html) is set to [SnackBarBehavior.floating](https://api.flutter.dev/flutter/material/SnackBarBehavior.html) and the next page has a floating action button, while the current one does not, the [SnackBar](https://api.flutter.dev/flutter/material/SnackBar-class.html) will smoothly animate above the floating action button. It also works in the case of a back gesture transition.

### Dart Pad

<iframe src="https://dartpad.dev/?id=29e69e537954114d0e906c3257c72d7f" style="width:100%;height:800px;border:none"></iframe>

### Source Code


<script src="https://gist.github.com/kissthecoke/29e69e537954114d0e906c3257c72d7f.js"></script>
