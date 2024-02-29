---
title: Icon Buttons
categories: Doc_Flutter, widgets
tags: Row
---
Icon Buttons

### [https://api.flutter.dev/flutter/material/IconButton-class.html](https://api.flutter.dev/flutter/material/IconButton-class.html)

### Click icon buttons and Test

<iframe src="https://kissthecoke.github.io/doc_flutter_samples//" style="width:430px;height:700px;border:1px solid gray"></iframe>


A Material Design icon button.

An icon button is a picture printed on a [Material](https://api.flutter.dev/flutter/material/Material-class.html) widget that reacts to touches by filling with color (ink).

Icon buttons are commonly used in the [AppBar.actions](https://api.flutter.dev/flutter/material/AppBar/actions.html) field, but they can be used in many other places as well.

If the [onPressed](https://api.flutter.dev/flutter/material/IconButton/onPressed.html) callback is null, then the button will be disabled and will not react to touch.

Requires one of its ancestors to be a [Material](https://api.flutter.dev/flutter/material/Material-class.html) widget. In Material Design 3, this requirement no longer exists because this widget builds a subclass of [ButtonStyleButton](https://api.flutter.dev/flutter/material/ButtonStyleButton-class.html).

The hit region of an icon button will, if possible, be at least kMinInteractiveDimension pixels in size, regardless of the actual [iconSize](https://api.flutter.dev/flutter/material/IconButton/iconSize.html), to satisfy the [touch target size](https://material.io/design/layout/spacing-methods.html#touch-targets) requirements in the Material Design specification. The [alignment](https://api.flutter.dev/flutter/material/IconButton/alignment.html) controls how the icon itself is positioned within the hit region.

1.This sample shows an [IconButton](https://api.flutter.dev/flutter/material/IconButton-class.html) that uses the Material icon "volume_up" to increase the volume.

2.In this sample the icon button's background color is defined with an [Ink](https://api.flutter.dev/flutter/material/Ink-class.html) widget whose child is an [IconButton](https://api.flutter.dev/flutter/material/IconButton-class.html). The icon button's filled background is a light shade of blue, it's a filled circle, and it's as big as the button is.

3.This sample shows creation of [IconButton](https://api.flutter.dev/flutter/material/IconButton-class.html) widgets for standard, filled, filled tonal and outlined types, as described in: [https://m3.material.io/components/icon-buttons/overview](https://m3.material.io/components/icon-buttons/overview)


### Source Code


<script src="https://gist.github.com/kissthecoke/ce3396dd881fd6e0a2819f1df16f0d29.js"></script>
