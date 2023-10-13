# 🥬 FARMUS, 팜어스 🥗

![서비스 이미지](https://devmint.s3.ap-northeast-2.amazonaws.com/readme/servicetitle.png)

### 슬로건, FARMUS

최근 집에서 채소를 길러서 먹는 사람들이 부쩍 늘어났는데요. 저마다의 동기를 가지고 홈파밍을 시작한 사람들이 여러 가지 어려움을 겪고 있습니다.

베란다에서 직접 기른 채소가 테이블 위 나의 접시 위에 성공적으로 올라오게 하기 위해서는 **꾸준한 관리**와 **부지런한 정보 탐색**, 그리고 그 과정에서 **지루함보다는 즐거움**을 느끼는 것이 중요합니다. FARMUS는 누구나 **홈파밍의 즐거움을 느껴 포기하지 않도록** 돕고자 합니다.

## 🧑🏻‍🌾 팀명 : 모던 파머

### R&R

| 분야   | 이름                                      | 포지션                                                     |
| ------ | ----------------------------------------- | ---------------------------------------------------------- |
| 기획   | 국준호                                    | 📑 데스크리서치, 정성리서치, 비즈니스모델 담당             |
| 기획   | 김서연                                    | 📊 기획 리드, 데스크리서치, 정량리서치, 서비스 브랜딩 담당 |
| 기획   | 이장미                                    | 🔍 데스크리서치, 정성리서치, 비즈니스모델 담당             |
| 디자인 | 남서윤                                    | 🖼️ 디자인 리드, 서비스 브랜딩, UI 디자인                   |
| 개발   | [김아린](https://github.com/arinming)     | 💻 개발 리드, Android 개발 담당                            |
| 개발   | [양건희](https://github.com/geonheey)     | 📱 Android 개발 담당                                       |
| 개발   | [이승렬](https://github.com/Ryeolee)      | 🖥️ 서버 개발 담당                                          |
| 개발   | [이은섭](https://github.com/MinchoGreenT) | 📢 프로젝트 매니징, 서버 개발 담당                         |

# [디자인 파트]

![로고, 아이콘](https://devmint.s3.ap-northeast-2.amazonaws.com/readme/logo_icon.png)

|          | 디자인 의도                                                                                                                                                                                                    |
| -------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 로고     | 작물을 심는 지면의 흙 모양을 모티브로 합니다. GT Pressura Black 영문의 서체를 변형해 아웃라인을 울퉁불퉁하게 만들어 즐거움을 추구하는 서비스의 무드에 맞게 생동감이 느껴지도록 합니다.                         |
| 색상     | 농업 관련 서비스이기 때문에 자연에서 볼 수 있는 컬러를 바탕으로, 목적에 맞게 조정해 사용합니다. 차분하고 부드러운 톤의 브라운을 메인 컬러로, 비비드한 녹색을 포인트 컬러로 사용해 경쾌함을 잃지 않도록 합니다. |
| 아이콘   | 아이콘은 로고와 같은 스타일로 디자인해 친근한 투박함이 느껴지도록 합니다. 작물이 성장하며 뻗어가는 모습을 나타냅니다.                                                                                          |
| 무드보드 | 생동감이 느껴지는 플랫한 그래픽을 활용한 레퍼런스를 위주로 구성했습니다.                                                                                                                                       |

# [개발 파트]

## 🛠️ 기술 스택 🛠️

### 📱 Frontend 📱

- ### 언어, 프레임워크

  ![Java](https://img.shields.io/badge/dart-%230175C2.svg?style=for-the-badge&logo=dart&logoColor=white)
  ![Java](https://img.shields.io/badge/flutter-%2302569B.svg?style=for-the-badge&logo=flutter&logoColor=white)

- ### 스키아 엔진과 직접 통신
  - 렌더링이 필요한 위젯들만 렌더링한다
  - 웹뷰를 사용하지 않고 스키아 엔진으로 직접 화면에 UI를 그린다
  - 안드로이드, iOS 개발을 동시에 할 수 있는 네이티브 앱 개발
  - 크로스 플랫폼 프레임워크
- ### 디자인 패턴

  > **MVVM (Model - View - ViewModel)**
  >
  > - View와 Model의 의존성이 없다
  > - View와 ViewModel은 양방향 소통이 아니므로 여러 View가 ViewModel 하나를 참조할 수 있다
  >
  > **View** : 사용자에게 보여지는 영역
  >
  > **ViewModel** : View 상태, 비즈니스 로직 담당
  >
  > **Repository** : 데이터 저장소
  >
  > **DataSource** : 데이터를 가져오는 영역
  >
  > **Model** : 데이터 설계

  <details>
  <summary style = " font-size:1.3em;">라이브러리</summary>
  <div markdown="1">

  - `Dio`
    - Flutter에서 API 통신을 가능하게 하는 http 라이브러리
  - `GetX`
    - 상속 위젯을 더 쉽게 사용하고 재사용할 수 있도록 만들어진 Wrapper 패키지
  - `SharedPrefrences`
    - 로컬에 값을 저장하고 읽어올 수 있게 하는 라이브러리
  - `flutter_staggerd_grid_view`
    - 화면 레이아웃을 자유롭게 나눠줌
  - `ImagePicker`
    - 갤러리에서 이미지를 선택하거나 카메라로 새로운 사진을 찍을 수 있는 플러그인
  - `flutter_screenutil`
    - 바로 화면 및 글꼴 크리를 조정하기 위한 라이브러리
    - 다양한 화면 크기에서 UI가 적절한 레이아웃을 표시할 수 있음

  </div>
  </details>

### 🖥️ Backend 🖥️

- ### 언어, 프레임워크
  ![Java](https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=java&logoColor=white)
  ![Springboot](https://img.shields.io/badge/spring%20boot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white)
  ![Spring](https://img.shields.io/badge/spring-6DB33F?style=for-the-badge&logo=spring&logoColor=white)
  ![Gradle](https://img.shields.io/badge/Gradle-02303A.svg?style=for-the-badge&logo=Gradle&logoColor=white)
  - 가장 많이 사용하는 웹 서버 프레임워크
  - MVC 패턴을 활용하여 깔끔한 코드 구성이 가능
- ### 클라우드
  ![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazonaws&logoColor=white)
  ![EC2](https://img.shields.io/badge/EC2-FF9900?style=for-the-badge&logo=Amazon%20EC2&logoColor=white)
  ![S3](https://img.shields.io/badge/S3-569A31?style=for-the-badge&logo=amazons3&logoColor=white)
  ![RDS](https://img.shields.io/badge/RDS-527FFF?style=for-the-badge&logo=Amazon%20RDS&logoColor=white)
  ![ElastiCache](https://img.shields.io/badge/ElastiCache-527FFF?style=for-the-badge&logo=Amazon)
  - AWS 프리티어를 통해 클라우드 인프라 구축
  - 서비스 생태계가 잘 구성되어 있기 때문에 AWS 하나만 활용해도 간편한 설계가 가능
  - 여기에 스프링 클라우드 라이브러리의 기능을 더해 msa 게이트웨이를 구현
- ### cicd
  ![GitHub Actions](https://img.shields.io/badge/github%20actions-%232671E5.svg?style=for-the-badge&logo=githubactions&logoColor=white)
  ![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white)
  - 어느 환경에서나 배포할 수 있도록 하는 대표적인 컨테이너 런타임
  - 깃허브 액션을 활용하여 별도의 인스턴스 없이 간편하게 ci-cd 파이프라인 구축
- ### 데이터베이스
  ![MySQL](https://img.shields.io/badge/mysql-%2300f.svg?style=for-the-badge&logo=mysql&logoColor=white)
  ![Redis](https://img.shields.io/badge/redis-%23DD0031.svg?style=for-the-badge&logo=redis&logoColor=white)
  ![Redis](https://img.shields.io/badge/MongoDB-%2347A248.svg?style=for-the-badge&logo=mongodb&logoColor=white)
  - msa의 이점을 활용하여 정형, 비정형 데이터베이스를 동시에 사용
  - redis를 통해 유저 리프레시 토큰 관리
- ### api 테스트, 명세서
  ![Notion](https://img.shields.io/badge/Notion-%23000000.svg?style=for-the-badge&logo=notion&logoColor=white)
  ![Postman](https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white)
  ![Swagger](https://img.shields.io/badge/-Swagger-%23Clojure?style=for-the-badge&logo=swagger&logoColor=white)
  - 노션에 명세서 페이지 및 swagger를 동시에 활용함으로 프론트 개발자에게 편리성 제공

## 📝 코드, 커밋 컨벤션 📝

### 📌 Frontend Code Convention

---

<details>
<summary style = " font-size:1.3em;">식별자(Identifiers)</summary>
<div markdown="1">

### UpperCamelCase : 첫 글자가 대문자

- Classes
- enum types
- typedefs
- type parameters
- extension

```dart
class SliderMenu { ... }

class HttpRequest { ... }

typedef Predicate<T> = bool Function(T value);

class Foo {
  const Foo([Object? arg]);
}

@Foo(anArg)
class A { ... }

@Foo()
class B { ... }

xtension MyFancyList<T> on List<T> { ... }

extension SmartIterable<T> on Iterable<T> { ... }
```

### lowerCamelCase : 첫 글자가 소문자

- 클래스 멤버
- 최상위 정의
- 변수
- 매개변수
- 상수

```dart
const pi = 3.14;
const defaultTimeout = 1000;
final urlScheme = RegExp('^([a-z]+):');

class Dice {
  static final numberGenerator = Random();
}
```

### lowercase_with_underscores : 소문자와 언더바

- 패키지
- 디렉토리
- 소스 파일
- import prefixes

```dart
my_package
└─ lib
   └─ file_system.dart
   └─ slider_menu.dart

import 'dart:math' as math;
import 'package:angular_components/angular_components.dart' as angular_components;
import 'package:js/js.dart' as js;
```

</div>
</details>
<details>
<summary style = " font-size:1.3em;">정렬(Ordering)</summary>
<div markdown="1">

### dart: 로 시작하는 패키지를 제일 앞에 배치

```dart
import 'dart:async';
import 'dart:html';

import 'package:bar/bar.dart';
import 'package:foo/foo.dart';
```

### package: 로 시작하는 패키지는 Relative의 앞에 배치

```dart
import 'package:bar/bar.dart';
import 'package:foo/foo.dart';

import 'util.dart';
```

### import는 import끼리, export는 export끼리

```dart
import 'src/error.dart';
import 'src/foo_bar.dart';

export 'src/error.dart';
```

### 섹션을 알파벳 순으로 정렬

```dart
import 'package:bar/bar.dart';
import 'package:foo/foo.dart';

import 'foo.dart';
import 'foo/foo.dart';
```

</div>
</details>
<details>
<summary style = " font-size:1.3em;">코드 구조(Formatting)</summary>
<div markdown="1">

### 1. 한줄 주석\_변수 설명

```dart
// 한 줄 주석일 때
```

### 2. 여러줄 주석\_함수, 위젯 설명

```dart
/**
* 여러줄
* 주석일 때
*/
```

</div>
</details>
<details>
<summary style = " font-size:1.3em;">주석(Comments)</summary>
<div markdown="1">

### 1. K&R 스타일로 중괄호 선언

> 클래스 선언, 메서드 선언, 조건/반복문 등의 코드 블럭을 감싸는 중괄호에 적용되는 규칙이다. 중괄호 선언은 K&R 스타일(Kernighan and Ritchie style)을 따른다. 줄의 마지막에서 시작 중괄호`{`를 쓰고 열고 새줄을 삽입한다. 블럭을 마친후에는 새줄 삽입 후 중괄호를 닫는다.

### 2. 닫는 중괄호와 같은 줄에 `else`, `catch`, `finally`, `while` 선언

> 아래의 키워드는 닫는 중괄호(`}`) 와 같은 줄에 쓴다.

- else
- catch, finaly
- do-while 문에서의 while

### 3. 빈 블럭에 새줄 없이 중괄호 닫기 허용

> 내용이 없는 블럭을 선언할 때는 같은 줄에서 중괄호를 닫는 것을 허용한다.

### 4. 조건/반복문에 중괄호 필수 사용

> 조건, 반복문이 한 줄로 끝더라도 중괄호를 활용한다. 이 문서에 언급된 중괄호의 전후의 공백, 제어문 앞 뒤의 새줄 규칙도 함께 고려한다.

</div>
</details>

### 📌 Backend Code Convention

---

<details>
<summary style = " font-size:1.3em;">네이밍</summary>
<div markdown="1">

### 1. 패키지 이름은 소문자로 구성

> 패키지 이름은 소문자를 사용하여 작성한다. 단어별 구문을 위해 언더스코어(`_`)나 대문자를 섞지 않는다.

### 2. 클래스/인터페이스 이름에 대문자 카멜표기법 적용

> 클래스 이름은 단어의 첫 글자를 대문자로 시작하는 대문자 카멜표기법(Upper camel case)을 사용한다. 파스칼표기법(Pascal case)으로도 불린다.

### 3. 클래스 이름에 명사 사용

> 클래스 이름은 명사나 명사절로 짓는다.

### 4. 인터페이스 이름에 명사/형용사 사용

> 인터페이스(interface)의 이름은 클래스 이름은 명사/명사절로 혹은 형용사/형용사절로 짓는다.

### 5. 테스트 클래스는 'Test'로 끝남

> JUnit 등으로 작성한 테스트 코드를 담은 클래스는 'Test’을 마지막에 붙인다.

### 6. 메서드 이름에 소문자 카멜표기법 적용

> 메서드의 이름에는 첫 번째 단어를 소문자로 작성하고, 이어지는 단어의 첫 글자를 대문자로 작성하는 소문자 카멜표기법(Lower camel case)를 사용한다. 테스트 클래스의 메서드 이름에서는 언더스코어를 허용한다.

### 7. 메서드 이름은 동사/전치사로 시작

> 메서드명은 기본적으로는 동사로 시작한다. 다른 타입으로 전환하는 메서드나 빌더 패턴을 구현한 클래스의 메서드에는 전치사를 쓸 수 있다.

_좋은 예_

- 동사사용 : `renderHtml()`
- 전환메서드의 전치사 : `toString()`
- Builder 패턴 적용한 클래스의 메서드의 전치사 : `withUserId(String id)`

### 8. 상수는 대문자와 언더스코어로 구성

> 상태를 가지지 않는 자료형이면서 `static final`로 선언되어 있는 필드일 때를 상수로 간주한다. 상수 이름은 대문자로 작성하며, 복합어는 언더스코어(`_`)를 사용하여 단어를 구분한다.

### 9. 변수에 소문자 카멜표기법 적용

> 상수가 아닌 클래스의 멤버변수/지역변수/메서드 파라미터에는 소문자 카멜표기법(Lower camel case)을 사용한다.

### 10. 임시 변수 외에는 1 글자 이름 사용 금지

> 메서드 블럭 범위 이상의 생명 주기를 가지는 변수에는 1글자로 된 이름을 쓰지 않는다. 반복문의 인덱스나 람다 표현식의 파라미터 등 짧은 범위의 임시 변수에는 관례적으로 1글자 변수명을 사용할 수 있다.

</div>
</details>
<details>
<summary style = " font-size:1.3em;">주석</summary>
<div markdown="1">

### 1. 한줄 주석은 // 를 사용한다.

```java
// 하이~
```

### 2. Bracket 사용 시 내부에 주석을 작성한다.

```java
/*
   하이~!
*/
```

### 3. 주요 함수에 대한 주석

```java
/*
 * 입력 : 인덱스:Long
 * 기능 : 유저 인덱스로 db에 접근해 유저 객체를 반환한다
 * 출력 : 유저:User
 */
public User getUser(Long idx)
```

</div>
</details>
<details>
<summary style = " font-size:1.3em;">선언</summary>
<div markdown="1">

### 1. 소스파일당 1개의 탑레벨 클래스를 담기

> 탑레벨 클래스(Top level class)는 소스 파일에 1개만 존재해야 한다. ( 탑레벨 클래스 선언의 컴파일타임 에러 체크에 대해서는 [Java Language Specification 7.6](http://docs.oracle.com/javase/specs/jls/se7/html/jls-7.html#jls-7.6) 참조 )

### 2. static import에만 와일드 카드 허용

> 클래스를 import할때는 와일드카드(`*`) 없이 모든 클래스명을 다 쓴다. static import에서는 와일드카드를 허용한다.

### 3. 애너테이션 선언 후 새줄 사용

> 클래스, 인터페이스, 메서드, 생성자에 붙는 애너테이션은 선언 후 새줄을 사용한다. 이 위치에서도 파라미터가 없는 애너테이션 1개는 같은 줄에 선언할 수 있다.

### 4. 한 줄에 한 문장

> 문장이 끝나는 `;` 뒤에는 새줄을 삽입한다. 한 줄에 여러 문장을 쓰지 않는다.

### 5. 하나의 선언문에는 하나의 변수만

> 변수 선언문은 한 문장에서 하나의 변수만을 다룬다.

### 6. 배열에서 대괄호는 타입 뒤에 선언

> 배열 선언에 오는 대괄호(`[]`)는 타입의 바로 뒤에 붙인다. 변수명 뒤에 붙이지 않는다.

### 7. `long`형 값의 마지막에 `L`붙이기

> long형의 숫자에는 마지막에 대문자 'L’을 붙인다. 소문자 'l’보다 숫자 '1’과의 차이가 커서 가독성이 높아진다.

</div>
</details>
<details>
<summary style = " font-size:1.3em;">중괄호</summary>
<div markdown="1">

### 1. K&R 스타일로 중괄호 선언

> 클래스 선언, 메서드 선언, 조건/반복문 등의 코드 블럭을 감싸는 중괄호에 적용되는 규칙이다. 중괄호 선언은 K&R 스타일(Kernighan and Ritchie style)을 따른다. 줄의 마지막에서 시작 중괄호`{`를 쓰고 열고 새줄을 삽입한다. 블럭을 마친후에는 새줄 삽입 후 중괄호를 닫는다.

### 2. 닫는 중괄호와 같은 줄에 `else`, `catch`, `finally`, `while` 선언

> 아래의 키워드는 닫는 중괄호(`}`) 와 같은 줄에 쓴다.

- else
- catch, finaly
- do-while 문에서의 while

### 3. 빈 블럭에 새줄 없이 중괄호 닫기 허용

> 내용이 없는 블럭을 선언할 때는 같은 줄에서 중괄호를 닫는 것을 허용한다.

### 4. 조건/반복문에 중괄호 필수 사용

> 조건, 반복문이 한 줄로 끝더라도 중괄호를 활용한다. 이 문서에 언급된 중괄호의 전후의 공백, 제어문 앞 뒤의 새줄 규칙도 함께 고려한다.

</div>
</details>

### 📌 Commit Convention

---

**형식** - `[TAG] : Message (#Issue)`

**태그 구분**

> feat : 새로운 기능 구현
>
> fix : 버그, 오류 해결, 코드 수정
>
> chore : 내부 파일 수정
>
> style : 코드에 관련 없는 주석 달기, 줄바꿈
>
> docs : README, WIKI, PR 템플릿 등의 문서 개정
>
> add : feat 이외의 부수적인 코드 추가, 라이브러리 추가, 새로운 파일 생성

## 🖍️ Git Flow

**브랜치 형식** - `feature_이슈번호/제목`

| master  | 제품으로 출시될 수 있는 브랜치   |
| ------- | -------------------------------- |
| develop | 다음 출시 버전을 개발하는 브랜치 |
| feature | 기능을 개발하는 브랜치           |
| release | 이번 출시 버전을 준비하는 브랜치 |

깃 플로우 이미지

## ⚙️ 시스템 아키텍처 ⚙️

![아키텍처](https://devmint.s3.ap-northeast-2.amazonaws.com/readme/Farm-Us-Arch.png)
