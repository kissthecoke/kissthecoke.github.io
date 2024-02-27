---
title: Shopping List Item.2
categories: Doc_Flutter, widgets
tags: Row
---
## Bringing it all together

### [https://docs.flutter.dev/ui#bringing-it-all-together](https://docs.flutter.dev/ui#bringing-it-all-together)

### Click shopping_list_item and Test

<iframe src="https://kissthecoke.github.io/doc_flutter_samples//" style="width:430px;height:500px;border:1px solid gray"></iframe>

The `ShoppingList` class extends [`StatefulWidget`](https://api.flutter.dev/flutter/widgets/StatefulWidget-class.html), which means this widget stores mutable state. When the `ShoppingList` widget is first inserted into the tree, the framework calls the [`createState()`](https://api.flutter.dev/flutter/widgets/StatefulWidget-class.html#createState) function to create a fresh instance of `_ShoppingListState` to associate with that location in the tree. (Notice that subclasses of [`State`](https://api.flutter.dev/flutter/widgets/State-class.html) are typically named with leading underscores to indicate that they are private implementation details.) When this widget’s parent rebuilds, the parent creates a new instance of `ShoppingList`, but the framework reuses the `_ShoppingListState` instance that is already in the tree rather than calling `createState` again.

To access properties of the current `ShoppingList`, the `_ShoppingListState` can use its [`widget`](https://api.flutter.dev/flutter/widgets/Widget-class.html) property. If the parent rebuilds and creates a new `ShoppingList`, the `_ShoppingListState` rebuilds with the new widget value. If you wish to be notified when the `widget` property changes, override the [`didUpdateWidget()`](https://api.flutter.dev/flutter/widgets/State-class.html#didUpdateWidget) function, which is passed an `oldWidget` to let you compare the old widget with the current widget.

When handling the `onCartChanged` callback, the `_ShoppingListState` mutates its internal state by either adding or removing a product from `_shoppingCart`. To signal to the framework that it changed its internal state, it wraps those calls in a [`setState()`](https://api.flutter.dev/flutter/widgets/State/setState.html) call. Calling `setState` marks this widget as dirty and schedules it to be rebuilt the next time your app needs to update the screen. If you forget to call `setState` when modifying the internal state of a widget, the framework won’t know your widget is dirty and might not call the widget’s [`build()`](https://api.flutter.dev/flutter/widgets/StatelessWidget/build.html) function, which means the user interface might not update to reflect the changed state. By managing state in this way, you don’t need to write separate code for creating and updating child widgets. Instead, you simply implement the `build` function, which handles both situations.

### Source Code


<script src="https://gist.github.com/kissthecoke/1933ace7b883063f938c9146ead77dd3.js"></script>
