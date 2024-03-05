---
title: Linear Progress Indicator
categories: Doc_Flutter, widgets
tags: Row
---
Linear Progress Indicator

### [https://api.flutter.dev/flutter/material/LinearProgressIndicator-class.html](https://api.flutter.dev/flutter/material/LinearProgressIndicator-class.html)

### Click linear progress Indicator and Test

<iframe src="https://kissthecoke.github.io/doc_flutter_samples//" style="width:430px;height:700px;border:1px solid gray"></iframe>


A widget that shows progress along a line. There are two kinds of linear progress indicators:

* *Determinate* . Determinate progress indicators have a specific value at each point in time, and the value should increase monotonically from 0.0 to 1.0, at which time the indicator is complete. To create a determinate progress indicator, use a non-null [value](https://api.flutter.dev/flutter/material/ProgressIndicator/value.html) between 0.0 and 1.0.
* *Indeterminate* . Indeterminate progress indicators do not have a specific value at each point in time and instead indicate that progress is being made without indicating how much progress remains. To create an indeterminate progress indicator, use a null [value](https://api.flutter.dev/flutter/material/ProgressIndicator/value.html).

The indicator line is displayed with [valueColor](https://api.flutter.dev/flutter/material/ProgressIndicator/valueColor.html), an animated value. To specify a constant color value use: `AlwaysStoppedAnimation<Color>(color)`.

The minimum height of the indicator can be specified using [minHeight](https://api.flutter.dev/flutter/material/LinearProgressIndicator/minHeight.html). The indicator can be made taller by wrapping the widget with a [SizedBox](https://api.flutter.dev/flutter/widgets/SizedBox-class.html).


### Dart Pad


<iframe src="https://dartpad.dev/?id=0e5f0ac982309d4997e56824776d530e" style="width:100%;height:800px;border:none"></iframe>



### Source Code


<script src="https://gist.github.com/kissthecoke/0e5f0ac982309d4997e56824776d530e.js"></script>
