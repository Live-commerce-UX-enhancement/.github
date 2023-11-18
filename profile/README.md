## Requirements

- 해당 프로젝트를 실행시키기 위해서, 아래의 지시사항을 순서대로 따라주세요.
- 2대의 서로다른 컴퓨터가 필요합니다.
    - 관리자용 : 라이브 커머스 관리자 보드 실행을 위한 컴퓨터
    - 시청자용 : Naver Live Commerce 및 시청자용 Chrome Extension 실행을 위한 컴퓨터
 
## Presentation Video + Demo
- https://www.youtube.com/watch?v=AcHoE-BJosg

---

### 1. 채팅 의도 분류 모델을 AWS 에 배포 후, API 를 생성합니다.

- [Chat-Intent-Classification Repository](https://github.com/Live-commerce-UX-enhancement/Chat-Intent-Classification) 를 참고하여 채팅 의도분류 모델에 대한 API 를 생성합니다.

### 2. 자동 답변 생성 프로젝트를 AWS 에 배포 합니다.

- [Auto-Answer-Generation Repository](https://github.com/Live-commerce-UX-enhancement/Auto-Answer-Generation) 를 참고하여 자동 답변 생성 프로젝트를 AWS 에 배포합니다.

### 3. 라이브 커머스 관리자 보드 서비스를 AWS에 배포합니다.

- [Live Shopping SellerBoard Repository](https://github.com/Live-commerce-UX-enhancement/Live-Shopping-Seller-Board) 를 참고하여 라이브 커머스 관리자보드를 AWS에 배포합니다.

### 4. 라이브 커머스 관리자 보드를 실행합니다.
- 3번 배포 시, 사용한 AWS 의 EC2 인스턴스의 Public IP 를 활용하여, 관리자용 컴퓨터로 라이브 커머스 관리자 보드에 접속합니다.
    - 접속 주소 : EC2 인스턴스의 Public IP + Port Number(3000)
1. 현재 보고 있는 네이버 쇼핑 라이브 url 입력 후, ‘admin program start’ 버튼을 클릭합니다.
    - 반드시 현재 라이브 중인 방송이어야 합니다.
2. 해당 방송에 등록되어 있는 제품 정보 및 방송 정보를 직접 입력 후, ‘상품 정보 등록’ 버튼을 클릭합니다.
3. 관리자 보드 접속 후, 답변 하고 싶은 질문 댓글을 선택합니다.
4. 답변 작성 후, ‘send’ 버튼을 클릭합니다. (시청자 구글 크롬 확장프로그램 실행 시, 라이브 방송 페이지 채팅창에서 질문 및 답변을 확인할 수 있습니다.)

### 5. 시청자용 크롬 확장 프로그램을 설치 및 실행합니다.

1. [Chrome-extension Repository](https://github.com/Live-commerce-UX-enhancement/Chrome-Extension) 를 참고하여 크롬 확장 프로그램 서비스를 시청자용 컴퓨터에 설치 및 실행합니다.
2. 현재 방송중인 네이버 쇼핑 라이브에 접속합니다. (반드시 현재 라이브 중인 방송이어야 합니다)
3. 쇼핑 라이브 접속 화면에서, 상단의 퍼즐 모양을 클릭합니다.
4. WebSocket Demo 크롬 확장 프로그램이 실행되면, 아래의 사진처럼 ‘WebSocket Demo’의 원이 빨간색으로 바뀝니다.
    <img width="294" alt="image" src="https://github.com/Live-commerce-UX-enhancement/.github/assets/64399505/5bfd99d9-993b-4583-911f-2e5b9b8b6e23">

    
5. 관리자 프로그램에서 답변을 전송할 시, 라이브 방송 페이지 채팅창에서 관리자가 보낸 답변과 그 답변에 해당하는 질문을 확인할 수 있습니다.
