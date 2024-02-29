---
title: Floating Action Buttons
categories: Doc_Flutter, widgets
tags: Row
---
Floating Action Buttons

### [https://api.flutter.dev/flutter/material/FloatingActionButton-class.html](https://api.flutter.dev/flutter/material/FloatingActionButton-class.html)

### Click floating action buttons and Test

<iframe src="https://kissthecoke.github.io/doc_flutter_samples//" style="width:430px;height:700px;border:1px solid gray"></iframe>


Use at most a single floating action button per screen. Floating action buttons should be used for positive actions such as "create", "share", or "navigate". (If more than one floating action button is used within a [Route](https://api.flutter.dev/flutter/widgets/Route-class.html), then make sure that each button has a unique [heroTag](https://api.flutter.dev/flutter/material/FloatingActionButton/heroTag.html), otherwise an exception will be thrown.)

If the [onPressed](https://api.flutter.dev/flutter/material/FloatingActionButton/onPressed.html) callback is null, then the button will be disabled and will not react to touch. It is highly discouraged to disable a floating action button as there is no indication to the user that the button is disabled. Consider changing the [backgroundColor](https://api.flutter.dev/flutter/material/FloatingActionButton/backgroundColor.html) if disabling the floating action button.

### Source Code


<script src="https://gist.github.com/kissthecoke/fb163ae2c7b7f07b8b9fb3a5acf98c86.js"></script>
