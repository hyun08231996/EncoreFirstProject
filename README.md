# EncoreFirstProject

4.21 



## MileStone

1. Project 착수 단계
   - 작업기간
   - 사용할 기술 셋 
   - 사용할 software (그림이 가독성이 좋고 직관적이다)
   - 주제 선정
2. 프로젝트 계획

   - 구축할 아키텍쳐 구조
   - SRS 작성
   - usecase Diagram 작성
3. 사용자적 관점에서 System 활용도 파악
4. 





메뉴, 마이미피(개인정보) 2개의 메뉴만 사용?!

![image-20210421114420946](C:\Users\sehon\AppData\Roaming\Typora\typora-user-images\image-20210421114420946.png)


![image](https://user-images.githubusercontent.com/46814964/115526425-fb692e80-a2ca-11eb-877d-57cab71cc4bc.png)



메뉴 

피자, 샐러드&사이드, 나만의피자 3개의 카테고리를 설정

각각의 카테고리를 클릭하면 해당 Category에 속하는 menu들을 보여줌.

메뉴 버튼을 눌렀으면,

아래의 기능이 있어야한다.

1. 피자, 샐러드/사이드, 나만의피자 를 선택할수있는 버튼(토글)
2. 피자 사진을 누르면 피자 상세정보로 이동
3. 장바구니로 이동

![image-20210421114526634](C:\Users\sehon\AppData\Roaming\Typora\typora-user-images\image-20210421114526634.png)







![image-20210421120351404](C:\Users\sehon\AppData\Roaming\Typora\typora-user-images\image-20210421120351404.png)



나만의 피자 화면

피자 도우 그림

....... 토핑들 (가격순 또는 이름순으로 정렬)



![image-20210421114927393](C:\Users\sehon\AppData\Roaming\Typora\typora-user-images\image-20210421114927393.png)



![image-20210421120531591](C:\Users\sehon\AppData\Roaming\Typora\typora-user-images\image-20210421120531591.png)



![image-20210421121018716](C:\Users\sehon\AppData\Roaming\Typora\typora-user-images\image-20210421121018716.png)

![image-20210421121059842](C:\Users\sehon\AppData\Roaming\Typora\typora-user-images\image-20210421121059842.png)

프론트(화면)

메인화면 -> 오형석님, 프론트영역 총괄 

- 로그인화면
- 아이디/비밀번호 찾기
- 회원가입화면
- 개인정보수정

메뉴화면 -> 권예람님

- 피자 메뉴 화면
- 사이드/샐러드 메뉴 화면
- 나만의 피자 만들기 화면

- 피자상세정보화면

주문 -> 남승현님

- 장바구니 화면
- 주문 유형 선택 화면
- 주소/매장 선택 화면
- 결제화면





## 간트 차트
![image](https://user-images.githubusercontent.com/46814964/115572495-e7d5bc00-a2fa-11eb-9c2a-894987a824f3.png)




## 요구사항 명세표
작성자 : 임세홍
작성일 : 2021-04-21

| ID   | 화면명(클래스명) | 요구사항내용                                                 | 우선순위 | 담당자 |
| ---- | ---------------- |  ------------------------------------------------------------ | -------- | ------ |
| 1    | 메인화면         |  Home, 메뉴, Mypage 3개로 구성한다.  |          | 오형석 |
| MI-02    | 메인   | [인트로] 화면을 구성한다.  -예시 : https://www.mrpizza.co.kr/ |        | 오형석       |
| 2    | 로그인      |  화면 구성, 퀵 메뉴 2가지로 구성한다. ID, PW를 입력 받는다. |          | 오형석 |
| 2    | 로그아웃   |  화면 구성 없이, 퀵 메뉴로 만든다. |          | 오형석 |
| 3    | 회원가입   |  화면 구성 후, 회원 정보 입력 받아 회원등록 한다. |          | 오형석 |
| 4    | 개인정보수정   |  마이페이지에 회원 정보 수정 사이드메뉴로 구성한다.  |          | 오형석 |
| 5    | 피자메뉴 화면  |   메뉴바 구현                                                             |          |        |
| 6    | 피자상세정보 화면 | 피자의 상세정보를 보여주고 하단에 주문하기로 주문하거나 장바구니에 담을 수 있음|          |        |
| 7    | 사이드/샐러드 상세정보 화면 |                                                              |          |        |
| 8    |                  |                                                   |          |        |
| 9    | 장바구니         |  왼쪽 영역 (장바구니)<br />- 이전 화면에서 장바구니에 추가한 모든 피자정보 (이미지, 이름, 가격 등)의 List를 DB로부터 받아와서 장바구니(Table)에 담는다.<br />- 수량을 조절할 수 있게 한다. (이때 minimum 수량은 1개)<br />- 특정 피자를 선택(Select)할 수 있게 하고 (복수선택 가능), 삭제(Button)를 누르면 선택된 피자를 삭제할 수 있게 한다.<br />오른쪽 영역 (계산)<br />- 장바구니에 있는 모든 피자들의 가격을 더한  총 결제예정금액을 표시한다.<br />- ''결제하러가기'' Button을 표시한다. |          | 남승현 |
| 10   | 주문 유형 선택   |  - 이전 화면에서 ''결제하러가기'' Button을 클릭하면 주문 유형을 선택할 수 있는 화면으로 넘어온다.<br />- 주문 유형은 2개 -> 배달주문 or 방문포장 (Button식으로 하나만 선택 가능하게) |          | 남승현 |
| 11   | 주소/매장 선택   | 배달주문<br />- 새로운 배달 주소를 입력할 수 있게 하고, 이 주소를 DB에 저장해서 다음 번에 주문할 때 이 주소를 사용할 수 있게 한다.<br />- 저장된 모든 주소를 '내 배달주소' 리스트에 담고, 하나만 선택할 수 있게 한다.<br />방문포장<br />- DB에 저장되어 있는 모든 매장 주소들을 가져와서, 주소 하나만 선택할 수 있게 한다.<br />화면 하단에 '결제하기'와 '취소' 버튼을 표시한다. |          | 남승현 |
| 12   | 결제             | - 최종 결제 금액을 표시한다.<br/>- 결제하기를 클릭하면 회원의 총 결제금액에서 최종 결제 금액이 추가되는 방식으로 구현한다.<br/>- 결제완료 페이지로 가게 한다. |          | 남승현 |
| 13   | DB 설계          | 명세사항에 맞는 table 작성                                   |          | 변준영 |
| 14   | DB 설계          | 작성한 table에 부합되는 VO class 작성                        |          | 변준영 |
| 15   | DAO interface    |1. 회원가입 method, 2. 로그인 method, 3. 개인정보 수정 method, 4. 피자 정보 불러오는 method, 6. 매장정보 출력 method, 4. |          | 임세홍 |
| 16   | DAO class        | class 작성각 Controller들에서 요구되어지는 method들을 완성한다. |          | 임세홍 |
| 17   | 로그인           |  아이디, 비밀번호 확인 후 로그인                                  |          | 조은비 |
| 18   | 회원가입         | 이름, 주소, 생년월일, 전화번호 입력 후 가입                  |          | 조은비 |
| 19   | 개인정보 수정    |  로그인 후 이름, 주소 등 개인정보 수정            |          | 조은비 |
| 20   | 금액 결제        | 결제 버튼 클릭하면 결제가 완료              |          | 조은비 |
| 21   | 아이디/ 비밀번호 찾기  | 개인정보 대조 후 아이디/ 비밀번호 알려줌    |          |        |
| 22   | PizzaMenuController | 피자 메뉴 선택시 상세페이지로 이동     |          |        |
| 23   |                  | 사이드, 샐러드 선택시 상세페이지로 이동   |          |        |
| 24   |                  | 토핑, 도우 선택, 이미지 보이기   |          |        |
| 25   |                  | 매장의 주소 검색 및 선택   |          |        |



백엔드 

1. 디비 설계, VO class (회원정보 <- 주문내역, 토핑정보, 피자, 사이드/샐러드, 매장정보) : 1명 -> 변준영 
2. DAO Class <- DAO interface(interface 설계는 같이!) : 1명 -> 임세홍
3. MainServlet, Controllers(Controller interface를 implements한 것들), HandlerMapping : 2명 -> 오영수님, 조은비님

각자 화면에 대한 Controller :

조은비님

- 로그인에 대한 Controller 
- 회원가입에 대한 Controller 
- 아이디/비밀번호 찾기에 대한 Controller 
- 개인정보 수정에 대한 Controller 
- 금액 결제 화면에 대한 Controller 

오영수님

- 메뉴화면에서 피자 객체 정보들을 넘겨주는 Controller 
- 샐러드/사이드화면에 대한 Controller 
- 나만의 피자 화면에서 토핑과 도우에 대한 정보를 다루는 Controller 
- 주소/매장 선택 화면에 대한 Controller 



1명이 DAO class 작성 -> reference작성(method명, return type, 이 method가 어떤 작업을 하는지, method에 필요한 parameter들)

Controller class를 구현하는 사람은 DAO class의 method의 내부구조를 몰라도 reference만 보면 DB와 소통 할 수있다.



| 테이블명 | Column                                                       |
| -------- | ------------------------------------------------------------ |
| 회원정보 | id(PK), 이름, 비밀번호, 주소, 이메일주소, 총 주문금액        |
| 주문내역 | 주문번호(PK), 고객id(FK), 매장id(FK), 피자명, 주문유형, 결제금액 |
| 피자     | 피자이름, 가격                                               |
| 매장     | 매장id, 매장주소, 매장 전화번호, 매장 총 매출                |
| 사이드   | id, 사이드이름, 가격                                         |




MileStone 단계 정하기

1. Project 설계
   - 작업기간, 사용할 기술 셋, 사용할 softwware, 주제 선정

분석을 바탕으로 설계가 있어야함

1. 각자 자신이 맡은 파트를 로컬에서 완성하고 제대로 돌아가는지 테스를 완료
   - 매일 (주기적으로) 서로의 진행상황에 대해 피드백
   - 백엔드 파트가 먼저 윤곽이 잡혀야 프론트에서 동적 페이지 구성을 원활하게 작성 가능합니당.
2. 각자 로컬에 완성한것을 하나의 프로젝트로 합병
   - 
3. 프로그램이 전체적으로 잘 돌아가는지 확인  그리고 구현한 내용에 대해 피드백 진행





![image-20210421165347908](C:\Users\sehon\AppData\Roaming\Typora\typora-user-images\image-20210421165347908.png)



![image-20210421165546425](C:\Users\sehon\AppData\Roaming\Typora\typora-user-images\image-20210421165546425.png)



피드백 : 요구사항 명세서 ID를 분류에 따라 구분할수있게 바꿔주자. 요구사항 명칭이 ID에 녹아들어야함.  ex : P-1, M-1

기능 설명에 집중하자. ~~한 값을 가지고 회원 가입을 한다.(사용자적인 기능)

비기능적인 면도 들어갈 수 있다.

우선순위도 필요
