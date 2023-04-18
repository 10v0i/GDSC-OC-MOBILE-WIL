# WIL3
1. MaterialApp()
- MaterialApp() 위젯을 사용해 코드 작성
- 디자인과 여러 기능을 제공
- MaterialApp()은 구글 스타일 <-> Cupertino() Apple(ios) 스타일

2. Scaffold()
- 앱을 상중하로 나눠주는 위젯
> 상단: appbar() (AppBar() 위젯은 상단바를 생성해줌)
> 앱의 내용: body()
> 하단: BottomAppBar() 위젯

3. 여러 위젯 가로로 배치하는 법
- Row(children:[])
- Row의 mainAxis = 가로축
  Row의 crossAxis = 세로축

4. 여러 위젯 세로로 배치하는 법
- Column(children:[])
- Column의 mainAxis = 세로축
  Column의 crossAxis = 가로축
