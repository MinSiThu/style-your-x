## Flutter Style Guide

Flutter style guide ဖြစ်ပါသည်။
- Code တွေကို dartfmt သုံးပြီး format လုပ်နိုင်ပါတယ်။

- ပထမဆုံး widget တွေမှာ comma နေရာမှာဖြတ်တောက်တာကိုလုပ်သင့်ပါတယ်။
```dart
children.add(Expanded(
  child: Center(
      child: Container(
        width: 64.0,
        height: 64.0,
        child: FuchsiaSpinner(),
      ),
   ),
));
```

- Package တူတူထဲမှာဆိုရင် Relative path ကိုပဲသုံးသင့်ပါတယ်။ Absolute path ကိုတော့ 3rd party lib တွေမှာပဲသုံးသင့်ပါတယ်။
  
**Good:**
```dart
import 'access_point.dart';
```
**Bad:**
```dart
import 'package:wifi/access_point.dart';
```

- mutation တွေကိုတတ်နိုင်သမျှရှောင်ဖို့ const keyword ကိုသုံးပါ။

- Flutter Widget type ကိုပဲ return ပြန်သင့်ပါတယ်။ Specific Widgetတွေအစား။

**Good:**
```dart
Widget returnContainerWidget() {
  return Container();
}
```

**Bad:**
```dart
Container returnContainerWidget() {
  return Container();
}
```

အထက်ပါ Guide ကို [Fuschia Style Guide](https://fuchsia.dev/fuchsia-src/development/languages/dart/style )မှ ထုတ်နုတ်ဖော်ပြထားခြင်းဖြစ်သည်။