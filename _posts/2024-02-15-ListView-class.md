---
title: ListView Class
categories: Doc_Flutter, widgets
tags: Row
---
## ListView class

https://api.flutter.dev/flutter/widgets/ListView-class.html

[ListView](https://api.flutter.dev/flutter/widgets/ListView-class.html) is the most commonly used scrolling widget. It displays its children one after another in the scroll direction. In the cross axis, the children are required to fill the [ListView](https://api.flutter.dev/flutter/widgets/ListView-class.html).

If non-null, the [itemExtent](https://api.flutter.dev/flutter/widgets/ListView/itemExtent.html) forces the children to have the given extent in the scroll direction.

If non-null, the [prototypeItem](https://api.flutter.dev/flutter/widgets/ListView/prototypeItem.html) forces the children to have the same extent as the given widget in the scroll direction.

Specifying an [itemExtent](https://api.flutter.dev/flutter/widgets/ListView/itemExtent.html) or an [prototypeItem](https://api.flutter.dev/flutter/widgets/ListView/prototypeItem.html) is more efficient than letting the children determine their own extent because the scrolling machinery can make use of the foreknowledge of the children's extent to save work, for example when the scroll position changes drastically.

You can't specify both [itemExtent](https://api.flutter.dev/flutter/widgets/ListView/itemExtent.html) and [prototypeItem](https://api.flutter.dev/flutter/widgets/ListView/prototypeItem.html), only one or none of them.

There are four options for constructing a [ListView](https://api.flutter.dev/flutter/widgets/ListView-class.html):

1. The default constructor takes an explicit [List&lt;Widget&gt;](https://api.flutter.dev/flutter/dart-core/List-class.html) of children. This constructor is appropriate for list views with a small number of children because constructing the [List](https://api.flutter.dev/flutter/dart-core/List-class.html) requires doing work for every child that could possibly be displayed in the list view instead of just those children that are actually visible.
2. The [ListView.builder](https://api.flutter.dev/flutter/widgets/ListView/ListView.builder.html) constructor takes an [IndexedWidgetBuilder](https://api.flutter.dev/flutter/widgets/IndexedWidgetBuilder.html), which builds the children on demand. This constructor is appropriate for list views with a large (or infinite) number of children because the builder is called only for those children that are actually visible.
3. The [ListView.separated](https://api.flutter.dev/flutter/widgets/ListView/ListView.separated.html) constructor takes two [IndexedWidgetBuilder](https://api.flutter.dev/flutter/widgets/IndexedWidgetBuilder.html)s: `itemBuilder` builds child items on demand, and `separatorBuilder` similarly builds separator children which appear in between the child items. This constructor is appropriate for list views with a fixed number of children.
4. The [ListView.custom](https://api.flutter.dev/flutter/widgets/ListView/ListView.custom.html) constructor takes a [SliverChildDelegate](https://api.flutter.dev/flutter/widgets/SliverChildDelegate-class.html), which provides the ability to customize additional aspects of the child model. For example, a [SliverChildDelegate](https://api.flutter.dev/flutter/widgets/SliverChildDelegate-class.html) can control the algorithm used to estimate the size of children that are not actually visible.

To control the initial scroll offset of the scroll view, provide a [controller](https://api.flutter.dev/flutter/widgets/ScrollView/controller.html) with its [ScrollController.initialScrollOffset](https://api.flutter.dev/flutter/widgets/ScrollController/initialScrollOffset.html) property set.

By default, [ListView](https://api.flutter.dev/flutter/widgets/ListView-class.html) will automatically pad the list's scrollable extremities to avoid partial obstructions indicated by [MediaQuery](https://api.flutter.dev/flutter/widgets/MediaQuery-class.html)'s padding. To avoid this behavior, override with a zero [padding](https://api.flutter.dev/flutter/widgets/BoxScrollView/padding.html) property.

### Examples

   1-1.This example uses the default constructor for [ListView](https://api.flutter.dev/flutter/widgets/ListView-class.html) which takes an explicit  [List&lt;Widget&gt;](https://api.flutter.dev/flutter/dart-core/List-class.html) of children. This [ListView](https://api.flutter.dev/flutter/widgets/ListView-class.html)'s children are made up of [Container](https://api.flutter.dev/flutter/widgets/Container-class.html)s with [Text](https://api.flutter.dev/flutter/widgets/Text-class.html).

<iframe src="https://dartpad.dev/?id=4c31b2f2d4b487faa4f75a04660f5edb" style="width:100%;height:800px;border:none"></iframe>

1-2.This example mirrors the previous one, creating the same list using the [ListView.builder](https://api.flutter.dev/flutter/widgets/ListView/ListView.builder.html) constructor. Using the [IndexedWidgetBuilder](https://api.flutter.dev/flutter/widgets/IndexedWidgetBuilder.html), children are built lazily and can be infinite in number.

<iframe src="https://dartpad.dev/?id=2edc13bbe2876e9274b7a64963bd32c4" style="width:100%;height:800px;border:none"></iframe>

1-3.This example continues to build from our the previous ones, creating a similar list using [ListView.separated](https://api.flutter.dev/flutter/widgets/ListView/ListView.separated.html). Here, a [Divider](https://api.flutter.dev/flutter/material/Divider-class.html) is used as a separator.

<iframe src="https://dartpad.dev/?id=e677f36902860be0eb706485b773158b" style="width:100%;height:800px;border:none"></iframe>

### Translate using DeepL

[ListView](https://api.flutter.dev/flutter/widgets/ListView-class.html)는 가장 일반적으로 사용되는 스크롤 위젯입니다. 스크롤 방향으로 자식을 차례로 표시합니다. 십자축에서 자식들은 [ListView](https://api.flutter.dev/flutter/widgets/ListView-class.html)를 채워야 합니다.

null이 아닌 경우, [itemExtent](https://api.flutter.dev/flutter/widgets/ListView/itemExtent.html)는 스크롤 방향에서 자식들이 지정된 범위를 갖도록 강제합니다.

null이 아닌 경우, [prototypeItem](https://api.flutter.dev/flutter/widgets/ListView/prototypeItem.html)은 자식들이 스크롤 방향에서 주어진 위젯과 동일한 범위를 갖도록 강제합니다.

[ListView](https://api.flutter.dev/flutter/widgets/ListView-class.html)는 가장 일반적으로 사용되는 스크롤 위젯입니다. 스크롤 방향으로 자식을 차례로 표시합니다. 십자축에서 자식들은 [ListView](https://api.flutter.dev/flutter/widgets/ListView-class.html)를 채워야 합니다.

null이 아닌 경우, [itemExtent](https://api.flutter.dev/flutter/widgets/ListView/itemExtent.html)는 스크롤 방향에서 자식들이 지정된 범위를 갖도록 강제합니다.

null이 아닌 경우, [prototypeItem](https://api.flutter.dev/flutter/widgets/ListView/prototypeItem.html)은 자식들이 스크롤 방향에서 주어진 위젯과 동일한 범위를 갖도록 강제합니다.

[ListView](https://api.flutter.dev/flutter/widgets/ListView-class.html)는 가장 일반적으로 사용되는 스크롤 위젯입니다. 스크롤 방향으로 자식을 차례로 표시합니다. 십자축에서 자식들은 [ListView](https://api.flutter.dev/flutter/widgets/ListView-class.html)를 채워야 합니다.

null이 아닌 경우, [itemExtent](https://api.flutter.dev/flutter/widgets/ListView/itemExtent.html)는 스크롤 방향에서 자식들이 지정된 범위를 갖도록 강제합니다.

null이 아닌 경우, [prototypeItem](https://api.flutter.dev/flutter/widgets/ListView/prototypeItem.html)은 자식들이 스크롤 방향에서 주어진 위젯과 동일한 범위를 갖도록 강제합니다.


항목범위](https://api.flutter.dev/flutter/widgets/ListView/itemExtent.html) 또는 [프로토타입 항목](https://api.flutter.dev/flutter/widgets/ListView/prototypeItem.html)을 지정하면 스크롤 위치가 급격하게 변경되는 경우와 같이 스크롤 기계가 항목범위를 미리 파악하여 작업을 줄일 수 있으므로 자식들이 스스로 범위를 결정하도록 하는 것보다 효율적입니다.

itemExtent](https://api.flutter.dev/flutter/widgets/ListView/itemExtent.html)와 [prototypeItem](https://api.flutter.dev/flutter/widgets/ListView/prototypeItem.html)을 모두 지정할 수 없으며, 둘 중 하나만 지정하거나 지정하지 않을 수 있습니다.

ListView](https://api.flutter.dev/flutter/widgets/ListView-class.html)를 구성하는 데는 네 가지 옵션이 있습니다:


1. 기본 생성자는 명시적인 [목록 위젯](https://api.flutter.dev/flutter/dart-core/List-class.html)의 자식을 취합니다. 이 생성자는 [목록](https://api.flutter.dev/flutter/dart-core/List-class.html)을 구성하려면 실제로 표시되는 자식만 아니라 목록 보기에 표시될 수 있는 모든 자식에 대해 작업을 수행해야 하므로 자식 수가 적은 목록 보기에 적합합니다.
2. ListView.builder](https://api.flutter.dev/flutter/widgets/ListView/ListView.builder.html) 생성자는 필요에 따라 자식을 빌드하는 [IndexedWidgetBuilder](https://api.flutter.dev/flutter/widgets/IndexedWidgetBuilder.html)를 취합니다. 이 생성자는 실제로 표시되는 자식에 대해서만 빌더가 호출되므로 자식 수가 많은(또는 무한대로 많은) 목록 보기에 적합합니다.
3. ListView.separated](https://api.flutter.dev/flutter/widgets/ListView/ListView.separated.html) 생성자는 두 개의 [IndexedWidgetBuilder](https://api.flutter.dev/flutter/widgets/IndexedWidgetBuilder.html)를 받습니다: itemBuilder `는 필요에 따라 자식 항목을 빌드하고 `separatorBuilder`는 마찬가지로 자식 항목 사이에 표시되는 구분자 자식을 빌드합니다. 이 생성자는 고정된 수의 자식이 있는 목록 보기에 적합합니다.
4. ListView.custom](https://api.flutter.dev/flutter/widgets/ListView/ListView.custom.html) 생성자는 자식 모델의 추가 측면을 사용자 지정할 수 있는 기능을 제공하는 [SliverChildDelegate](https://api.flutter.dev/flutter/widgets/SliverChildDelegate-class.html)를 받습니다. 예를 들어, [SliverChildDelegate](https://api.flutter.dev/flutter/widgets/SliverChildDelegate-class.html)는 실제로 표시되지 않는 자식의 크기를 추정하는 데 사용되는 알고리즘을 제어할 수 있습니다.

스크롤 뷰의 초기 스크롤 오프셋을 제어하려면 [컨트롤러](https://api.flutter.dev/flutter/widgets/ScrollView/controller.html)에 [ScrollController.initialScrollOffset](https://api.flutter.dev/flutter/widgets/ScrollController/initialScrollOffset.html) 속성이 설정된 [컨트롤러]를 제공하세요.

기본적으로 [ListView](https://api.flutter.dev/flutter/widgets/ListView-class.html)는 [MediaQuery](https://api.flutter.dev/flutter/widgets/MediaQuery-class.html)의 패딩으로 표시되는 부분적인 장애물을 피하기 위해 목록의 스크롤 가능한 끝부분을 자동으로 패딩합니다. 이 동작을 방지하려면 0 [padding](https://api.flutter.dev/flutter/widgets/BoxScrollView/padding.html) 속성으로 재정의하세요.

예제


1-1.이 예제에서는 명시적인 [List&amp;;Widget;](https://api.flutter.dev/flutter/dart-core/List-class.html)의 자식을 취하는 [ListView](https://api.flutter.dev/flutter/widgets/ListView-class.html)의 기본 생성자를 사용합니다. 이 [ListView](https://api.flutter.dev/flutter/widgets/ListView-class.html)의 자식은 [Container](https://api.flutter.dev/flutter/widgets/Container-class.html)와 [Text](https://api.flutter.dev/flutter/widgets/Text-class.html)로 구성됩니다.

1-2.이 예제는 이전 예제를 미러링하여 [ListView.builder](https://api.flutter.dev/flutter/widgets/ListView/ListView.builder.html) 생성자를 사용하여 동일한 목록을 생성합니다. 인덱싱된 위젯 빌더](https://api.flutter.dev/flutter/widgets/IndexedWidgetBuilder.html)를 사용하면 자식이 느리게 빌드되며 그 수는 무한대로 늘어날 수 있습니다.

1-3.이 예제는 이전 예제에서 계속 빌드하여 [ListView.separated](https://api.flutter.dev/flutter/widgets/ListView/ListView.separated.html)를 사용하여 유사한 목록을 만듭니다. 여기서는 [디바이더](https://api.flutter.dev/flutter/material/Divider-class.html)를 구분 기호로 사용합니다.
