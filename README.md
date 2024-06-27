# android-contacts
***
사용자가 간단한 인터페이스/입력폼을 통해 연락처를 등록/조회할 수 있는 애플리케이션
***
## STEP1 연락처_정보_폼 
연락처를 추가하기 위한 UI 구성 
- 필수구현 (미입력시, 토스트메시지)
  - 이름 (TextView)
  - 전화번호 (TextView)
- 선택구현
  - 메일 (TextView)
  * 더보기 (Button)
  - 생일 (Calender)
  - 성별 (Radio)
  - 메모 (TextView)
- 하단 뷰 (클릭시, 토스트메시지 + 연락처_목록_화면으로 전환)
  - 취소_버튼 (Button)
  - 저장_버튼 (Button)

***

## STEP2 연락처_목록_기능

+ 연락처_목록_보기
  - 연락처 목록 (RecyclerView + 객체)
  - 특정 연락처 클릭 이벤트시, 특정인물_정보_보기 화면으로 전환
+ 특정인물_정보_보기
  - 특정인물의 이름/전화번호 기록되어있음
+ 추가기능
  - 뒤로가기 버튼을 누를 시 확인팝업창
  - 추가된 연락처는 앱이 다시 실행시 유지되지 않음

## 실행화면


## 코드 개요
#### MainActivity.kt
+ 버튼을 눌러 새로운 연락처를 추가할 수 있음
+ 연락처_목록을 표시함 
#### RegisterContact.kt
+ 연락처_등록_폼을 처리함
#### ViewContact.kt
+ 클릭한 연락처의 Info 표시
#### Person.kt
+ 한 연락처(객체)를 나타내는 데이터 클래스
#### PersonAdapter.kt
+ 연락처_목록을 표시하는 RecyclerView 어댑터
