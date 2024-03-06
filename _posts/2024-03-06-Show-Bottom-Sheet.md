---
title: Show Bottom Sheet
categories: Doc_Flutter, widgets
tags: Row
---
Show Bottom Sheet

### [https://api.flutter.dev/flutter/material/showModalBottomSheet.html](https://api.flutter.dev/flutter/material/showModalBottomSheet.html)

### Click Show Bottom Sheet and Test

<iframe src="https://kissthecoke.github.io/doc_flutter_samples//" style="width:430px;height:900px;border:1px solid gray"></iframe>


Shows a modal Material Design bottom sheet.

A modal bottom sheet is an alternative to a menu or a dialog and prevents the user from interacting with the rest of the app.

A closely related widget is a persistent bottom sheet, which shows information that supplements the primary content of the app without preventing the user from interacting with the app. Persistent bottom sheets can be created and displayed with the [showBottomSheet](https://api.flutter.dev/flutter/material/showBottomSheet.html) function or the [ScaffoldState.showBottomSheet](https://api.flutter.dev/flutter/material/ScaffoldState/showBottomSheet.html) method.

The `isScrollControlled` parameter specifies whether this is a route for a bottom sheet that will utilize [DraggableScrollableSheet](https://api.flutter.dev/flutter/widgets/DraggableScrollableSheet-class.html). Consider setting this parameter to true if this bottom sheet has a scrollable child, such as a [ListView](https://api.flutter.dev/flutter/widgets/ListView-class.html) or a [GridView](https://api.flutter.dev/flutter/widgets/GridView-class.html), to have the bottom sheet be draggable.

The `isDismissible` parameter specifies whether the bottom sheet will be dismissed when user taps on the scrim.

The `enableDrag` parameter specifies whether the bottom sheet can be dragged up and down and dismissed by swiping downwards.

The `useSafeArea` parameter specifies whether the sheet will avoid system intrusions on the top, left, and right. If false, no [SafeArea](https://api.flutter.dev/flutter/widgets/SafeArea-class.html) is added; and [MediaQuery.removePadding](https://api.flutter.dev/flutter/widgets/MediaQuery/MediaQuery.removePadding.html) is applied to the top, so that system intrusions at the top will not be avoided by a [SafeArea](https://api.flutter.dev/flutter/widgets/SafeArea-class.html) inside the bottom sheet either. Defaults to false.

The optional `backgroundColor`, `elevation`, `shape`, `clipBehavior`, `constraints` and `transitionAnimationController` parameters can be passed in to customize the appearance and behavior of modal bottom sheets (see the documentation for these on [BottomSheet](https://api.flutter.dev/flutter/material/BottomSheet-class.html) for more details).

The `transitionAnimationController` controls the bottom sheet's entrance and exit animations. It's up to the owner of the controller to call [AnimationController.dispose](https://api.flutter.dev/flutter/animation/AnimationController/dispose.html) when the controller is no longer needed.

The optional `settings` parameter sets the [RouteSettings](https://api.flutter.dev/flutter/widgets/RouteSettings-class.html) of the modal bottom sheet sheet. This is particularly useful in the case that a user wants to observe [PopupRoute](https://api.flutter.dev/flutter/widgets/PopupRoute-class.html)s within a [NavigatorObserver](https://api.flutter.dev/flutter/widgets/NavigatorObserver-class.html).

A [DisplayFeature](https://api.flutter.dev/flutter/dart-ui/DisplayFeature-class.html) can split the screen into sub-screens. The closest one to `anchorPoint` is used to render the content.

If no `anchorPoint` is provided, then [Directionality](https://api.flutter.dev/flutter/widgets/Directionality-class.html) is used:

* for [TextDirection.ltr](https://api.flutter.dev/flutter/dart-ui/TextDirection.html), `anchorPoint` is `Offset.zero`, which will cause the content to appear in the top-left sub-screen.
* for [TextDirection.rtl](https://api.flutter.dev/flutter/dart-ui/TextDirection.html), `anchorPoint` is `Offset(double.maxFinite, 0)`, which will cause the content to appear in the top-right sub-screen.

If no `anchorPoint` is provided, and there is no [Directionality](https://api.flutter.dev/flutter/widgets/Directionality-class.html) ancestor widget in the tree, then the widget asserts during build in debug mode.

The `context` argument is used to look up the [Navigator](https://api.flutter.dev/flutter/widgets/Navigator-class.html) and [Theme](https://api.flutter.dev/flutter/material/Theme-class.html) for the bottom sheet. It is only used when the method is called. Its corresponding widget can be safely removed from the tree before the bottom sheet is closed.

The `useRootNavigator` parameter ensures that the root navigator is used to display the [BottomSheet](https://api.flutter.dev/flutter/material/BottomSheet-class.html) when set to `true`. This is useful in the case that a modal [BottomSheet](https://api.flutter.dev/flutter/material/BottomSheet-class.html) needs to be displayed above all other content but the caller is inside another [Navigator](https://api.flutter.dev/flutter/widgets/Navigator-class.html).

Returns a `Future` that resolves to the value (if any) that was passed to [Navigator.pop](https://api.flutter.dev/flutter/widgets/Navigator/pop.html) when the modal bottom sheet was closed.

The 'barrierLabel' parameter can be used to set a custom barrierlabel. Will default to modalBarrierDismissLabel of context if not set.

### Dart Pad

<iframe src="https://dartpad.dev/?id=daa78ea23441957fd24a57a363774538" style="width:100%;height:800px;border:none"></iframe>

### Source Code


<script src="https://gist.github.com/kissthecoke/daa78ea23441957fd24a57a363774538.js"></script>
