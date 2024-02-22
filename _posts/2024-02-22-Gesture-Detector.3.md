---
title: Gesture Detector Example.3
categories: Doc_Flutter, widgets
tags: Row
---
## Gesture Detector.3

### [https://api.flutter.dev/flutter/widgets/GestureDetector-class.html](https://api.flutter.dev/flutter/widgets/GestureDetector-class.html)

### Click nested gesture detectors and Test

<iframe src="https://kissthecoke.github.io/doc_flutter_samples//" style="width:430px;height:500px;border:1px solid gray"></iframe>


This example uses a [GestureDetector](https://api.flutter.dev/flutter/widgets/GestureDetector-class.html) that wraps a green [Container](https://api.flutter.dev/flutter/widgets/Container-class.html) and a second GestureDetector that wraps a yellow Container. The second GestureDetector is a child of the green Container. Both GestureDetectors define an onTap callback. When the callback is called it adds a red border to the corresponding Container.

When the green Container is tapped, it's parent GestureDetector enters the gesture arena. It wins because there is no competing GestureDetector and the green Container shows a red border. When the yellow Container is tapped, it's parent GestureDetector enters the gesture arena. The GestureDetector that wraps the green Container also enters the gesture arena (the pointer events coordinates are inside both GestureDetectors bounds). The GestureDetector that wraps the yellow Container wins because it was the first detector to enter the arena.

This example sets [debugPrintGestureArenaDiagnostics](https://api.flutter.dev/flutter/gestures/debugPrintGestureArenaDiagnostics.html) to true. This flag prints useful information about gesture arenas.

Changing the [GestureDetector.behavior](https://api.flutter.dev/flutter/widgets/GestureDetector/behavior.html) property to [HitTestBehavior.translucent](https://api.flutter.dev/flutter/rendering/HitTestBehavior.html) or [HitTestBehavior.opaque](https://api.flutter.dev/flutter/rendering/HitTestBehavior.html) has no impact: both GestureDetectors send a [GestureRecognizer](https://api.flutter.dev/flutter/gestures/GestureRecognizer-class.html) into the gesture arena, only one wins.

### Source Code

<script src="https://gist.github.com/kissthecoke/c7e5be12dcd73135bef2fd6a0539a024.js"></script>
