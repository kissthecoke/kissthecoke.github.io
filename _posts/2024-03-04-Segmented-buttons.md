---
title: Segmented Buttons
categories: Doc_Flutter, widgets
tags: Row
---
Segmented Buttons

### [https://api.flutter.dev/flutter/material/SegmentedButton-class.html](https://api.flutter.dev/flutter/material/SegmentedButton-class.html)

### Click segmented buttons and Test

<iframe src="https://kissthecoke.github.io/doc_flutter_samples//" style="width:430px;height:700px;border:1px solid gray"></iframe>


A Material button that allows the user to select from limited set of options.

Segmented buttons are used to help people select options, switch views, or sort elements. They are typically used in cases where there are only 2-5 options.

The options are represented by segments described with [ButtonSegment](https://api.flutter.dev/flutter/material/ButtonSegment-class.html) entries in the [segments](https://api.flutter.dev/flutter/material/SegmentedButton/segments.html) field. Each segment has a [ButtonSegment.value](https://api.flutter.dev/flutter/material/ButtonSegment/value.html) that is used to indicate which segments are selected.

The [selected](https://api.flutter.dev/flutter/material/SegmentedButton/selected.html) field is a set of selected [ButtonSegment.value](https://api.flutter.dev/flutter/material/ButtonSegment/value.html)s. This should be updated by the app in response to [onSelectionChanged](https://api.flutter.dev/flutter/material/SegmentedButton/onSelectionChanged.html) updates.

By default, only a single segment can be selected (for mutually exclusive choices). This can be relaxed with the [multiSelectionEnabled](https://api.flutter.dev/flutter/material/SegmentedButton/multiSelectionEnabled.html) field.

Like [ButtonStyleButton](https://api.flutter.dev/flutter/material/ButtonStyleButton-class.html)s, the [SegmentedButton](https://api.flutter.dev/flutter/material/SegmentedButton-class.html)'s visuals can be configured with a [ButtonStyle](https://api.flutter.dev/flutter/material/ButtonStyle-class.html) [style](https://api.flutter.dev/flutter/material/SegmentedButton/style.html) field. However, unlike other buttons, some of the style parameters are applied to the entire segmented button, and others are used for each of the segments.

By default, a checkmark icon is used to show selected items. To configure this behavior, you can use the [showSelectedIcon](https://api.flutter.dev/flutter/material/SegmentedButton/showSelectedIcon.html) and [selectedIcon](https://api.flutter.dev/flutter/material/SegmentedButton/selectedIcon.html) fields.

Individual segments can be enabled or disabled with their [ButtonSegment.enabled](https://api.flutter.dev/flutter/material/ButtonSegment/enabled.html) flag. If the [onSelectionChanged](https://api.flutter.dev/flutter/material/SegmentedButton/onSelectionChanged.html) field is null, then the entire segmented button will be disabled, regardless of the individual segment settings.

### Source Code


<script src="https://gist.github.com/kissthecoke/4218cc7c423dd4c45694a37546d32299.js"></script>
