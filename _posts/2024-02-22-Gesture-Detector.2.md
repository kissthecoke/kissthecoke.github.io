---
title: Gesture Detector Example.2
categories: Doc_Flutter, widgets
tags: Row
---
## Gesture Detector.2

### [https://api.flutter.dev/flutter/widgets/GestureDetector-class.html](https://api.flutter.dev/flutter/widgets/GestureDetector-class.html)

### Click gesture detector.2 and Test

<iframe src="https://kissthecoke.github.io/doc_flutter_samples//" style="width:430px;height:500px;border:1px solid gray"></iframe>


This example uses a [Container](https://api.flutter.dev/flutter/widgets/Container-class.html) that wraps a [GestureDetector](https://api.flutter.dev/flutter/widgets/GestureDetector-class.html) widget which detects a tap.

Since the [GestureDetector](https://api.flutter.dev/flutter/widgets/GestureDetector-class.html) does not have a child, it takes on the size of its parent, making the entire area of the surrounding [Container](https://api.flutter.dev/flutter/widgets/Container-class.html) clickable. When tapped, the [Container](https://api.flutter.dev/flutter/widgets/Container-class.html) turns yellow by setting the `_color` field. When tapped again, it goes back to white.

### Source Code


<script src="https://gist.github.com/kissthecoke/1c05f49b6dda6df6a9adc4da0eb16100.js"></script>
