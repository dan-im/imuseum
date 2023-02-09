# :art: 박물관 예매 플랫폼 'IMUSEUM'
![아이뮤지엄](https://user-images.githubusercontent.com/112814104/217779351-2d890be8-be9a-492a-9cd4-9429925ea217.png)

## :pushpin: 주제
![개발동기](https://user-images.githubusercontent.com/112814104/217780378-5c1017e3-c283-4bad-bfa4-7260baaecd69.jpg)
![주제](https://user-images.githubusercontent.com/112814104/217780382-c3d19a73-013c-48b1-a51a-ab240012c637.jpg)

## :pushpin: 메뉴구성
![메뉴구성](https://user-images.githubusercontent.com/112814104/217780885-9e0d111a-a919-4bd7-94fc-774aa45a403d.jpg)
- **회원관리:** 회원가입, 로그인, 아이디찾기, 비밀번호찾기, 회원정보수정, 회원탈퇴
- **전시:** 진행전시조회, 지난전시조회, 전시예약
- **교육프로그램:** 진행프로그램조회, 지난프로그램조회, 프로그램예약
- **스토어:** 상품조회, 리뷰/문의 조회, 장바구니, 주문/결제, 찜하기
- **관리자:** 상품관리, 판매내역조회, 전시등록/관리, 프로그램등록/관리, 문의답글등록, 예매티켓관리
- **마이페이지:** 예매목록조회, 주문내역조회, 작성글조회, 회원등급조회, 배송지관리

## :pushpin: 개발환경
- **개발기간:** 2022.11.16 ~ 2022.12.16 (4주)
- **개발 웹서버:** Apache Tomcat 9.0
- **개발 프레임워크:** Spring 4.3.16, MyBatis, Maven
- **개발 툴:** Eclipse IDE, Oracle SQL Developer
- **사용 언어:** Java(JDK 1.8), JSP & Servlet, HTML/CSS, JavaScript, Jquery, Ajax
- **사용 API:** (네이버, 카카오, 구글) 로그인 API, 아임포트 결제API, (카카오, 구글) 지도 API, 카카오 우편번호 API, (트위터, 카카오, 페이스북) 공유, EmailJS

## :pushpin: 역할분담
![역할분담](https://user-images.githubusercontent.com/112814104/217783767-c0f9992d-b030-4356-82f9-a142b85031af.jpg)
- **김동환(팀장):** 회원가입, 로그인/로그아웃, 소셜로그인, 아이디/비밀번호 찾기, QNA 게시판
- **김소연:** 스토어, 장바구니, 주문/결제, 주문확인, 상품리뷰, 찜하기
- **백은주:** 마이페이지, 예매 및 주문조회, 배송지등록, FAQ 게시판
- **서태우:** 교육프로그램 등록 및 관리, 교육프로그램 단체예매 등록 및 관리
- **이현준:** 판매상품 등록 및 관리, 배송관리, 상품문의
- **임다은:** 전시 등록 및 관리, 전시 예매, 교육프로그램 예매, 예매티켓 관리

## :pushpin: DB 설계
![DB설계](https://user-images.githubusercontent.com/112814104/217784709-ed393134-1865-43e2-be3e-31dcac5257ca.jpg)
해당 텍스트 클릭 시 DB 자세히 보기가 가능합니다.
<details>
<summary><b>유저, 공지사항, 교육프로그램</b></summary>

![유저,공지사항, 교육프로그램](https://user-images.githubusercontent.com/112814104/217785277-c4cb2dea-076b-41f2-9f87-5ad15ef2cec4.jpg)

</details>
<details>
<summary><b>교육프로그램 관리, 교육프로그램 단체예매</b></summary>

![교육프로그램 관리, 교육프로그램 단체예매](https://user-images.githubusercontent.com/112814104/217786135-099e3294-7455-4eb8-8da0-a35ad352af15.jpg)

</details>
<details>
<summary><b>전시 관리, 예약</b></summary>

![전시관리,예약](https://user-images.githubusercontent.com/112814104/217786432-fb4bd472-4c49-4d9e-94bc-083f852cbeeb.jpg)

</details>
<details>
<summary><b>QNA게시판</b></summary>

![QNA게시판](https://user-images.githubusercontent.com/112814104/217786434-3b7c1c0c-1e6d-4f9c-ac3b-7e39242415d6.jpg)

</details>
<details>
<summary><b>상품,상품문의</b></summary>

![상품,상품문의](https://user-images.githubusercontent.com/112814104/217786436-5173317a-312e-48d8-beb6-238c7a6a990a.jpg)

</details>
<details>
<summary><b>장바구니,주문배송</b></summary>

![장바구니,주문배송](https://user-images.githubusercontent.com/112814104/217786440-d77a379b-ca33-4860-87bf-70e6fdb7ec19.jpg)

</details>

## :raised_hand:맡은 기능 (해당 링크를 클릭 시 이동합니다)
* **[메인페이지](https://github.com/dan-im/imuseum/tree/main/Imuseum/src/main/webapp/WEB-INF/views#%ED%99%88%ED%99%94%EB%A9%B4)**
* **VISIT**
  * [미술관소개](https://github.com/dan-im/imuseum/tree/main/Imuseum/src/main/webapp/WEB-INF/views/visit#heavy_check_mark-%EB%AF%B8%EC%88%A0%EA%B4%80-%EC%86%8C%EA%B0%9C)
  * [오시는 길](https://github.com/dan-im/imuseum/tree/main/Imuseum/src/main/webapp/WEB-INF/views/visit#heavy_check_mark-%EC%98%A4%EC%8B%9C%EB%8A%94-%EA%B8%B8)
* **EXHIBITION**
  * [현재전시](https://github.com/dan-im/imuseum/tree/main/Imuseum/src/main/webapp/WEB-INF/views/exhibition#heavy_check_mark-%ED%98%84%EC%9E%AC%EC%A0%84%EC%8B%9C)
  * [지난전시](https://github.com/dan-im/imuseum/tree/main/Imuseum/src/main/webapp/WEB-INF/views/exhibition#heavy_check_mark-%EC%A7%80%EB%82%9C%EC%A0%84%EC%8B%9C)
  * [전시 상세보기](https://github.com/dan-im/imuseum/tree/main/Imuseum/src/main/webapp/WEB-INF/views/exhibition#heavy_check_mark-%EC%A0%84%EC%8B%9C-%EC%83%81%EC%84%B8%EB%B3%B4%EA%B8%B0)
  * [전시 및 교육프로그램 검색](https://github.com/dan-im/imuseum/tree/main/Imuseum/src/main/webapp/WEB-INF/views/exhibition#heavy_check_mark-%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%A8-%EA%B2%80%EC%83%89)
  * [프로그램 캘린더](https://github.com/dan-im/imuseum/tree/main/Imuseum/src/main/webapp/WEB-INF/views/exhibition#heavy_check_mark-%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%A8-%EA%B2%80%EC%83%89)
* **TICKET**
  * 전시티켓 예매
  * 교육프로그램티켓 예매
  * 티켓 결제
* **ADMIN**
  * 전시관리
  * 예매티켓 관리  
  
  

