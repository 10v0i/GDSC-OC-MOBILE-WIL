# WIL4
## 박스 디자인
1. 박스에 여백주기
> 외부 여백
- margin: EdgeInsets.all()

> 내부 여백
- padding: EdgeInsets.all()

>> all이 아닌 fromLTRB( , , , )를 사용하면 상하좌우 개별적으로 여백을 설정할 수 있음.

2. 박스 테두리 만들기
> 박스의 스타일은 decoration: 안에 작성해야함.
- border: Border.all(color: Color.black)

3. 박스 정렬하기
- Center(): 가운데 정렬
- Align(alignment: Alignment.~): 정렬 위치 조정

4. 박스 꽉 채우기
- double.infinity
