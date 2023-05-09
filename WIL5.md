# WIL5
Stateless Widget > build 메소드를 통해 UI 출력
## Stateful Widget
- 상태를 가지고 있음
- 위젯에 데이터를 정하거나 실시간으로 데이터의 변화를 보고 싶을 때 사용
1. 두 개의 부분으로 나뉨
- 첫번째 부분은 상태가 없는 위젯 그자체
- 두번째 부분은 위젯의 상태로 위젯에 들어갈 데이터와 UI를 넣는 곳
*데이터가 변경되면 해당 위젯의 UI도 변경됨
*위젯에 들어가는 데이터는 단순한 Dart 클래스 프로퍼티임

2. 작성법
- Stateful Widget 작성: st > Stateful, Stateless에 대한 옵션을 얻을 수 있음
  (Stateless Widget을 Stateful Widget으로 변경) Stateless Widget에 마우스를 올리고 code action을 열면 Convert to Stateful Widget 있음
  *State의 데이터를 바꿀 때 UI가 새로고침되면서 최신 데이터를 보여줌
- State에 위젯의 UI 관련 코드 작성
- 위젯에 데이터 추가
- 데이터 수정 함수 작성
- setState 함수 작성 > State 클래스에게 데이터가 변경되었다고 알리는 함수

## React

## BuildContext
- 부모 요소 정보에 직접 접근하는 데에 사용
*위젯 트리: 앱을 어떻게 렌더링하는지 보여주는 그림
> context를 이용
- context: 모든 상위 요소들에 대한 정보를 포함, 위젯 트리에 대한 정보가 있음
- 위젯 트리에서 위젯의 위치를 제공하고 이를 통해 상위 요소 데이터에 접근할 수 있게 해줌

## Widget Lifecycle
-  Statefule Widget은 build 메소드 이외에 initState 메소드도 가지고 있음
- initState 메소드: 상태를 초기화 하기 위한 메소드
> 상태변수의 초기화가 가능하기 때문에 대부분의 경우에서 필요없음
> 부모 요소에 의존하는 데이터를 초기화해야 하는 경우 사용됨
  *initState는 build 메소드보다 먼저 호출되어야 하고 단 한 번만 호출됨
- dispose 메소드: 위젯이 스크린에서 제거될 때 호출되는 메소드
