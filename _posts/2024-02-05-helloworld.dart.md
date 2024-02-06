---
title: Building user interfaces with Flutter
tags: TeXt
js: [{defer: true, url: https://dartpad.dev/experimental/inject_embed.dart.js}]
---
[https://docs.flutter.dev/ui](https://docs.flutter.dev/ui)

# Building user interfaces with Flutter

### Hello world

The minimal Flutter app simply calls the [`runApp()`](https://api.flutter.dev/flutter/widgets/runApp.html) function with a widget:

```dart
import 'package:flutter/material.dart';

void main() {
  runApp(
    const Center(
      child: Text(
        'Hello, world!',
        textDirection: TextDirection.ltr,
      ),
    ),
  );
}
```

The `runApp()` function takes the given [`Widget`](https://api.flutter.dev/flutter/widgets/Widget-class.html) and makes it the root of the widget tree. In this example, the widget tree consists of two widgets, the [`Center`](https://api.flutter.dev/flutter/widgets/Center-class.html) widget and its child, the [`Text`](https://api.flutter.dev/flutter/widgets/Text-class.html) widget. The framework forces the root widget to cover the screen, which means the text “Hello, world” ends up centered on screen. The text direction needs to be specified in this instance; when the `MaterialApp` widget is used, this is taken care of for you, as demonstrated later.

When writing an app, you’ll commonly author new widgets that are subclasses of either [`StatelessWidget`](https://api.flutter.dev/flutter/widgets/StatelessWidget-class.html) or [`StatefulWidget`](https://api.flutter.dev/flutter/widgets/StatefulWidget-class.html), depending on whether your widget manages any state. A widget’s main job is to implement a [`build()`](https://api.flutter.dev/flutter/widgets/StatelessWidget/build.html) function, which describes the widget in terms of other, lower-level widgets. The framework builds those widgets in turn until the process bottoms out in widgets that represent the underlying [`RenderObject`](https://api.flutter.dev/flutter/rendering/RenderObject-class.html), which computes and describes the geometry of the widget.

### Translate using DeepL

최소한의 Flutter 앱은 위젯을 사용하여 runApp() 함수를 호출하기만 하면 됩니다:

```dart
import 'package:flutter/material.dart';

void main() {
  runApp(
    const Center(
      child: Text(
        'Hello, world!',
        textDirection: TextDirection.ltr,
      ),
    ),
  );
}
```

runApp() 함수는 지정된 위젯을 받아 위젯 트리의 루트로 만듭니다. 이 예제에서 위젯 트리는 중앙 위젯과 그 자식인 텍스트 위젯이라는 두 개의 위젯으로 구성됩니다. 프레임워크는 루트 위젯이 화면을 덮도록 강제하므로 "Hello, world"라는 텍스트가 화면 중앙에 표시됩니다. 이 경우 텍스트 방향을 지정해야 하는데, MaterialApp 위젯을 사용하면 나중에 설명하는 것처럼 이 작업이 자동으로 처리됩니다.

앱을 작성할 때 위젯이 어떤 상태를 관리하는지 여부에 따라 일반적으로 StatelessWidget 또는 StatefulWidget의 서브클래스인 새 위젯을 작성하게 됩니다. 위젯의 주된 역할은 다른 하위 수준 위젯의 관점에서 위젯을 설명하는 build() 함수를 구현하는 것입니다. 프레임워크는 위젯의 지오메트리를 계산하고 설명하는 기본 렌더객체를 나타내는 위젯에서 프로세스가 바닥날 때까지 이러한 위젯을 차례로 빌드합니다.

### DartPad

<iframe src="https://dartpad.dev/embed-flutter.html?id=0ef00b2d6ceb2d9553a5428e47d2d77b&theme=dark" style="width:100%;height:400px;border:none" ></iframe>
