---
title: Text Class
tags: Text, Text.rich
---
## Text class

### https://api.flutter.dev/flutter/widgets/Text-class.html


A run of text with a single style.

The [Text](https://api.flutter.dev/flutter/widgets/Text-class.html) widget displays a string of text with single style. The string might break across multiple lines or might all be displayed on the same line depending on the layout constraints.

The [style](https://api.flutter.dev/flutter/widgets/Text/style.html) argument is optional. When omitted, the text will use the style from the closest enclosing [DefaultTextStyle](https://api.flutter.dev/flutter/widgets/DefaultTextStyle-class.html). If the given style's [TextStyle.inherit](https://api.flutter.dev/flutter/painting/TextStyle/inherit.html) property is true (the default), the given style will be merged with the closest enclosing [DefaultTextStyle](https://api.flutter.dev/flutter/widgets/DefaultTextStyle-class.html). This merging behavior is useful, for example, to make the text bold while using the default font family and size.

Using the [Text.rich](https://api.flutter.dev/flutter/widgets/Text/Text.rich.html) constructor, the [Text](https://api.flutter.dev/flutter/widgets/Text-class.html) widget can display a paragraph with differently styled [TextSpan](https://api.flutter.dev/flutter/painting/TextSpan-class.html)s. The sample that follows displays "Hello beautiful world" with different styles for each word.

### Translate using DeepL


단일 스타일의 텍스트 문자열.

텍스트](https://api.flutter.dev/flutter/widgets/Text-class.html) 위젯은 단일 스타일의 텍스트 문자열을 표시합니다. 레이아웃 제약 조건에 따라 문자열이 여러 줄로 나뉘거나 모두 같은 줄에 표시될 수 있습니다.

스타일](https://api.flutter.dev/flutter/widgets/Text/style.html) 인수는 선택 사항입니다. 생략하면 텍스트는 가장 가깝게 둘러싸는 [DefaultTextStyle](https://api.flutter.dev/flutter/widgets/DefaultTextStyle-class.html)의 스타일을 사용합니다. 지정된 스타일의 [TextStyle.inherit](https://api.flutter.dev/flutter/painting/TextStyle/inherit.html) 속성이 참이면(기본값), 지정된 스타일은 가장 가까운 [DefaultTextStyle](https://api.flutter.dev/flutter/widgets/DefaultTextStyle-class.html)을 둘러싸는 스타일과 병합됩니다. 이 병합 동작은 예를 들어 기본 글꼴 패밀리 및 크기를 사용하면서 텍스트를 굵게 만들 때 유용합니다.

Text.rich](https://api.flutter.dev/flutter/widgets/Text/Text.rich.html) 생성자를 사용하면 [Text](https://api.flutter.dev/flutter/widgets/Text-class.html) 위젯은 다양한 스타일의 [TextSpan](https://api.flutter.dev/flutter/painting/TextSpan-class.html)으로 단락을 표시할 수 있습니다. 다음 샘플은 각 단어마다 다른 스타일로 "안녕하세요 아름다운 세상"을 표시합니다.

<iframe src="https://dartpad.dev/?id=15ed8436d89314b49ffa1f097b3950c0" style="width:100%;height:800px;border:none"></iframe>
