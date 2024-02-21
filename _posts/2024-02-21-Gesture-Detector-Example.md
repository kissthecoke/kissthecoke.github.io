---
title: Gesture Detector Example.1
categories: Doc_Flutter, widgets
tags: Row
---
## GestureDetector.1

### [https://api.flutter.dev/flutter/widgets/GestureDetector-class.html](https://api.flutter.dev/flutter/widgets/GestureDetector-class.html)

### Click handling gestures and Test

<iframe src="https://kissthecoke.github.io/doc_flutter_samples//" style="width:430px;height:500px;border:1px solid gray"></iframe>


A widget that detects gestures.

Attempts to recognize gestures that correspond to its non-null callbacks.

If this widget has a child, it defers to that child for its sizing behavior. If it does not have a child, it grows to fit the parent instead.


By default a GestureDetector with an invisible child ignores touches; this behavior can be controlled with [behavior](https://api.flutter.dev/flutter/widgets/GestureDetector/behavior.html).

GestureDetector also listens for accessibility events and maps them to the callbacks. To ignore accessibility events, set [excludeFromSemantics](https://api.flutter.dev/flutter/widgets/GestureDetector/excludeFromSemantics.html) to true.

See [flutter.dev/gestures/](http://flutter.dev/gestures/) for additional information.

Material design applications typically react to touches with ink splash effects. The [InkWell](https://api.flutter.dev/flutter/material/InkWell-class.html) class implements this effect and can be used in place of a [GestureDetector](https://api.flutter.dev/flutter/widgets/GestureDetector-class.html) for handling taps.

### Source Code


<script src="https://gist.github.com/kissthecoke/321406e86d02b6e95ee71bb55b1ba04c.js"></script>
