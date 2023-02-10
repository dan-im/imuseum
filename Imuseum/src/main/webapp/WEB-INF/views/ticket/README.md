# TICKET
## :heavy_check_mark: 전시티켓 예매
![티켓선택](https://user-images.githubusercontent.com/112814104/218022046-9ce0d1c0-221f-4aaf-9d01-7b1c2e2a5a16.jpg)
- 상단 메뉴바에서 TICKET을 누르면 보여지는 화면입니다.
- 상단에서 티켓 예매 진행상황을 알 수 있으며, 그 아래 네비바를 통해 전시와 교육프로그램 두 가지 티켓 종류를 선택할 수 있습니다.
- **현재 예매할 수 있는 전시**를 보여주며 여러 건의 전시가 있는 경우 전시 시작일 기준 최신순과 오래된순으로 정렬할 수 있습니다.

![관람일선택](https://user-images.githubusercontent.com/112814104/218020939-d41481a6-135d-4525-90f5-5a434f1c9c74.jpg)
- 전시를 클릭하면 해당 전시의 정보를 확인할 수 있으며 관람일을 선택할 수 있는 페이지로 이동합니다.
- **우측 달력을 이용해서 관람일을 선택**할 수 있으며, **전시 기간이 아닐 경우에는 선택이 불가능**하도록 구현하였습니다.
- 권종별 관람인원을 선택할 수 있으며 티켓의 **예매갯수 합이 4매 이상일 경우 안내문구와 함께 카운트가 불가**하도록 구현하였습니다.
- **관람일과 관람인원 선택, 유의사항 동의**를 모두 마쳐야 예매하기 페이지로 이동합니다.
![전시티켓결제](https://user-images.githubusercontent.com/112814104/218024534-a94e5e33-4d83-410e-9bf2-47ebceff78dc.jpg)
- 이전 페이지에서 선택한 관람정보와 관람일, 관람인원을 받아옵니다.
- 회원우대로 30% 할인을 적용할 수 있으며, **권종별 가장 높은 티켓값을 기준으로 1매 적용**됩니다. 
- 결제정보에서 할인금액이 적용된 결제금액을 바로 확인할 수 있으며 필수 동의에 체크해야 결제하기가 가능합니다.
## :heavy_check_mark: 교육프로그램티켓 예매
![교육티켓선택](https://user-images.githubusercontent.com/112814104/218049287-ee810676-f496-4694-a2f2-899486f109f4.jpg)
- 티켓 메뉴바에서 LEARN을 누르면 보여지는 화면입니다.
- **현재 날짜 기준 예매할 수 있는 교육프로그램**을 보여주며 기본으로 모든 교육프로그램을 노출합니다.
- 원하는 교육대상을 선택해 조회가 가능합니다.
- 교육프로그램 예매는 **단체 교육과 1회성 교육(개인) 으로 나누어지며 상단 뱃지로 구분**해 확인할 수 있습니다.
![교육관람일선택](https://user-images.githubusercontent.com/112814104/218048692-01e47661-e4d1-42a3-a22d-07bce00c87f4.jpg)
- 1회성 교육 뱃지가 있는 프로그램을 클릭했을 때 이동하는 페이지입니다.
- 해당 교육프로그램의 정보를 확인할 수 있으며 교육일을 선택할 수 있습니다.
- **우측 달력을 이용해서 교육일을 선택**할 수 있으며, **교육 기간이 아닐 경우에는 선택이 불가능**하도록 구현하였습니다.
- **관리자가 등록한 정원 수에 맞게 예약가능 인원이 표시**되며, 날짜를 클릭하면 **빨간색으로 현재 예매 가능한 티켓 수를 확인**할 수 있습니다.
- 티켓의 **예매갯수 합이 4매 이상일 경우 안내문구와 함께 카운트가 불가**하도록 구현하였습니다.
- 교육일과 교육인원 선택, 유의사항 동의를 모두 마쳐야 예매하기 페이지로 이동합니다.
![교육티켓결제](https://user-images.githubusercontent.com/112814104/218050675-8d23ccf5-7889-4760-970c-fc7f71c93fbf.jpg)
- 이전 페이지에서 선택한 교육프로그램 정보와 교육일, 예매인원을 받아옵니다.
- 관리자가 등록한 참가비에 따라 결제금액이 결정됩니다.
- 필수 동의에 체크해야 결제하기가 가능하며 **무료교육일 경우 결제하기를 누르면 바로 예매완료 페이지로 이동**합니다.
## :heavy_check_mark: 티켓 결제
![아임포트](https://user-images.githubusercontent.com/112814104/218024904-251d6686-81c5-40a2-99d4-5560b322c081.jpg)
- 결제하기 버튼을 클릭하게 되면 **아임포트 결제 API로 이니시스 카드결제**가 가능합니다.
![결제성공](https://user-images.githubusercontent.com/112814104/218052668-de6c9bbe-2f8a-4eac-a998-20282527cad5.jpg)
- **예매에 성공**할 경우 예매 시간으로 생성된 예매번호가 등록되며 가입한 이메일로 예매정보를 발송합니다.
- 하단에서는 결제에 사용한 카드정보와 예매 정보를 확인할 수 있습니다.
![결제실패](https://user-images.githubusercontent.com/112814104/218052684-35544d93-0f8e-4790-a429-e60a0d099f90.jpg)
- 예매에 실패할 경우 '예매가 정상적으로 완료되지 않았습니다.' 라는 문구와 함께 아래에 결제 실패 사유를 표시합니다.
- 예매페이지로 가기 버튼을 클릭하면 처음 예매페이지로 돌아갑니다.

