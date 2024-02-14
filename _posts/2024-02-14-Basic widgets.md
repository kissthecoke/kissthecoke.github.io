---
title: Basic widgets 
tags: Text, Row, Column, Stack, Container
---
## Begin widgets 

### https://docs.flutter.dev/ui#basic-widgets

Flutter comes with a suite of powerful basic widgets, of which the following are commonly used:

**[`Text`](https://api.flutter.dev/flutter/widgets/Text-class.html)**

The `Text` widget lets you create a run of styled text within your application.



**[`Row`](https://api.flutter.dev/flutter/widgets/Row-class.html), [`Column`](https://api.flutter.dev/flutter/widgets/Column-class.html)**

These flex widgets let you create flexible layouts in both the horizontal (`Row`) and vertical (`Column`) directions. The design of these objects is based on the web’s flexbox layout model.


**[`Stack`](https://api.flutter.dev/flutter/widgets/Stack-class.html)**

Instead of being linearly oriented (either horizontally or vertically), a `Stack` widget lets you place widgets on top of each other in paint order. You can then use the [`Positioned`](https://api.flutter.dev/flutter/widgets/Positioned-class.html) widget on children of a `Stack` to position them relative to the top, right, bottom, or left edge of the stack. Stacks are based on the web’s absolute positioning layout model.


**[`Container`](https://api.flutter.dev/flutter/widgets/Container-class.html)**

The `Container` widget lets you create a rectangular visual element. A container can be decorated with a [`BoxDecoration`](https://api.flutter.dev/flutter/painting/BoxDecoration-class.html), such as a background, a border, or a shadow. A `Container` can also have margins, padding, and constraints applied to its size. In addition, a `Container` can be transformed in three-dimensional space using a matrix.

Below are some simple widgets that combine these and other widgets:


### Translate using DeepL

Text

'텍스트' 위젯을 사용하면 애플리케이션 내에서 스타일이 지정된 텍스트의 실행을 만들 수 있습니다.

[`Row`](https://api.flutter.dev/flutter/widgets/Row-class.html), [`Column`](https://api.flutter.dev/flutter/widgets/Column-class.html)

이러한 플렉스 위젯을 사용하면 가로(`행`) 및 세로(`열`) 방향 모두에서 유연한 레이아웃을 만들 수 있습니다. 이러한 개체의 디자인은 웹의 플렉스박스 레이아웃 모델을 기반으로 합니다.

**[`Stack`](https://api.flutter.dev/flutter/widgets/Stack-class.html)**

선형 방향(가로 또는 세로)이 아닌 `스택` 위젯을 사용하면 위젯을 페인트 순서대로 서로 위에 배치할 수 있습니다. 그런 다음 `스택`의 자식 위젯에 [`포지셔닝`] 위젯을 사용하여 스택의 위쪽, 오른쪽, 아래쪽 또는 왼쪽 가장자리를 기준으로 위젯을 배치할 수 있습니다. 스택은 웹의 절대 위치 지정 레이아웃 모델을 기반으로 합니다.

**[`Container`](https://api.flutter.dev/flutter/widgets/Container-class.html)**

컨테이너 ` 위젯을 사용하면 직사각형의 시각적 요소를 만들 수 있습니다. 컨테이너는 배경, 테두리 또는 그림자와 같은 [`BoxDecoration `](https://api.flutter.dev/flutter/painting/BoxDecoration-class.html)으로 장식할 수 있습니다. 컨테이너`에는 여백, 패딩 및 크기에 대한 제약 조건을 적용할 수도 있습니다. 또한 `Container`는 매트릭스를 사용하여 3차원 공간에서 변형할 수 있습니다.

다음은 이러한 위젯과 다른 위젯을 결합한 몇 가지 간단한 위젯입니다:


<iframe src="https://dartpad.dev/?id=6a1c54c289f2c5208a3284a82fa793f7" style="width:100%;height:800px;border:none"></iframe>
