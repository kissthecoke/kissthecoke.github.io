---
title: Changing widgets in response to input.2
categories: Doc_Flutter, widgets
tags: Row
---
## Changing widgets in response to input.2

### [https://docs.flutter.dev/ui#changing-widgets-in-response-to-input](https://docs.flutter.dev/ui#changing-widgets-in-response-to-input)

### Click counter2 using statefulwidget and Test

<iframe src="https://kissthecoke.github.io/doc_flutter_samples//" style="width:430px;height:500px;border:1px solid gray"></iframe>


You might wonder why `StatefulWidget` and `State` are separate objects. In Flutter, these two types of objects have different life cycles. `Widgets` are temporary objects, used to construct a presentation of the application in its current state. `State` objects, on the other hand, are persistent between calls to `build()`, allowing them to remember information.

The example above accepts user input and directly uses the result in its `build()` method. In more complex applications, different parts of the widget hierarchy might be responsible for different concerns; for example, one widget might present a complex user interface with the goal of gathering specific information, such as a date or location, while another widget might use that information to change the overall presentation.

In Flutter, change notifications flow “up” the widget hierarchy by way of callbacks, while current state flows “down” to the stateless widgets that do presentation. The common parent that redirects this flow is the `State`. The following slightly more complex example shows how this works in practice:

Notice the creation of two new stateless widgets, cleanly separating the concerns of *displaying* the counter (`CounterDisplay`) and *changing* the counter (`CounterIncrementor`). Although the net result is the same as the previous example, the separation of responsibility allows greater complexity to be encapsulated in the individual widgets, while maintaining simplicity in the parent.

### Source Code

<script src="https://gist.github.com/kissthecoke/09fe7de3658bb8e3e0008e3fbdef0251.js"></script>
