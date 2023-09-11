# 1주차 WIL - 김지송

## Chapter 1 Variables

### 1.1 The Var Keyword
`var` 로 변수 선언 가능
값을 업데이트 할땐 변수의 본래 `타입`과 일치해야 한다.

`변수의 타입`으로 도 변수 선언 가능

```dart
var name = 'GDSC';
String name2 = 'App Front';
```

### 1.2 Dynamic Type
Dynamic → 동적인

변수의 타입 → Dynamic

**변수의 타입을 특정할 수 없을 때 사용한다.**
```dart
dynamic name;
var name2;

name = 1;
name = 'GDSC';
```

### 1.3 Nullable Variables
Null Safety → 개발자가 null 값을 참조할 수 없도록 하는 기능

**null 은 존재 자체가 없는 상태! 부재!**

null 이 될 수 있음을 표시해야 한다.

기본적으로 모든 변수는 null이 허용되지 않는다.
```dart
String? nico = 'nico'
nico?.length
```

### 1.4 final Variables
나중에 수정할 수 있는 변수 → `var`

한 번 정의된 변수를 수정할 수 없게 하는 법! → `final`
```dart
final name = 'GDSC';
// 불가능!
// name = 'GDG';
```

### 1.5 Late Variables
`late` 는 `var`이나 `final` 앞에 붙일 수 있는 수식어

초기 데이터 없이 변수를 선언할 수 있게 해주는 수식어

아직 어떤 데이터가 올지 모른다고 말해주는 것!

정의되기 전에는 사용할 수 없다! → Null safety와 같은 기능
```dart
late final String name; //이러면 한 번만 값을 넣을 수 있는 변수를 생성
name = 'GDSC';
```

### 1.6 Constant Variables
`const`→ 상수

`compile-time constant` → **컴파일 될 때 알고 있는 값!!**

수정이 불가능하다는 점에선 final과 같다.
앱이 시작될 때 이전에 알고 있어야 하는 값!!
```dart
const API_KEY = 'eyzdfst2';
```

# 소감
강의를 들을 당시에는 양이 많다고 못 느꼈는데, WIL 쓰면서 보니까 공부해야할 양이 매우 많다는걸 알았다..
문법 자체는 python과 kotlin이랑 유사해서 익히기 어려운 언어는 아니라고 생각된다.
