1. 네트워크 정의
- [네트워크란](#네트워크란)
- [네트워크의 중요성](#네트워크의-중요성)
- [네트워크 형태](#네트워크의-형태)

2. 네트워크 구조
- [네트워크 구조](#네트워크의-구조)
- [홈 네트워크](#홈-네트워크)
- [기업용 네트워크](#기업용-네트워크)
- [클라우드 네트워크](#클라우드-네트워크)

3. OSI 7 Layer
- [OSI 7 Layer](#OSI-7-Layer)
- [OSI 7 Layer 모델](#OSI-7-Layer-모델)

4. TCP / IP
- [TCP/IP란](#TCP/IP란)
- [TCP/IP 모델](#TCP/IP-모델)
- [캡슐화](#캡슐화)

## 네트워크란
- 분산되어 있는 컴퓨터들이 자원을 공유할 수 있게 통신망으로 연결한 것

## 네트워크의 중요성
- 3차 산업혁명 : 디지털+인터넷 - 지식 정보화 사회
- 4차 산업혁명 : 정보통신 기술의 융합 - 빅데이터, 인공지능, 사물인터넷, 클라우드, 3D프린팅, 자율주행차, 지능형로봇
- On Network : 대부분의 요소 기술들은 네트워크 위에서 동작

## 네트워크의 형태
- LAN 근거리 통신망 : 사무실 또는 학교 등의 가까운 지역을 한데 묶은 네트워크
- WAN 장거리 통신망 : 각각 떨어진 LAN망을 연결, 규모가 큰 네트워크, ISP로 연결
- VPN 가상 사설망 : 공중망을 이용해 사설망을 사용할 수 있도록 하는 가상 사설망, 암호화되어 사용자에게 투명한 통신 서비스 제공

## 네트워크의 구조
- 통신 방식과 경로 : server & client, peer to peer
- 토폴로지 : 노드들과 연결된 회선들을 포함한 네트워크의 구성을 나타냄  

### Star : 각 노드는 중앙에 위치한 주 노드를 통하여 다른 노드들과 통신   
- 장점 - 장애 발견이 쉽고, 관리가 용이
- 단점 - 주 노드에 장애가 발생하면 전체 네트워크 사용이 불가능  
<img width=20% src=https://upload.wikimedia.org/wikipedia/commons/thumb/d/d0/StarNetwork.svg/1024px-StarNetwork.svg.png>

### Ring : 각 노드의 좌우의 인접한 노드와 연결되어 원형을 이루고 있는 형태
- 장점 - 단 방향 통신으로 신호 증폭이 가능하여 거리 제약이 적음
- 단점 - 노드의 추가 삭제가 용이하지 않음
<img width=20% src=https://upload.wikimedia.org/wikipedia/commons/d/db/NetworkTopology-Ring.png>

### Mesh : 모든 노드가 서로 일대일로 연결된 그물망 형태로 다수의 노드 쌍이 동시에 통신할 수 있음   
- 장점 - 특정 노드의 장애가 다른 노트에 영향을 주지 않고, 회선장애에 유연한 대처가 가능
- 단점 - 회선구축비용이 많이 들며, 새로운 노드 추가 시 비용부담이 발생   
<img width=20% src=https://upload.wikimedia.org/wikipedia/commons/thumb/3/3c/NetworkTopology-FullyConnected.png/440px-NetworkTopology-FullyConnected.png>

### Bus : 버스라는공통 배선에 각 노드가 연결된 형태로, 노드의 신호가 테이블 전체에 전달됨   
- 장점 - 노드의 추가 및 삭제가 용이하고, 특정 노드의 장애가 다른 노드에 영향을 주지 않음
- 단점 - 공통배선의 대역폭을 공유하기 때문에 노드 수가 증가하면 배선의 트래픽이 증가하여 네트워크 성능이 저하됨  
<img width=20% src=https://upload.wikimedia.org/wikipedia/commons/thumb/4/47/BusNetwork.svg/1024px-BusNetwork.svg.png>

### Tree : 트리 구조 형태로 망을 구성하여 정보 단말 장치를 추가하기 용이
- 장점 - 네트워크 관리가 쉽고 확장이 편리
- 단점 - 특정 노드에 트래픽이 집중화되면 네트워크 속도가 떨어짐  
<img width=20% src=https://fossbytes.com/wp-content/uploads/2016/03/tree-network-topology.jpg> 


### 홈 네트워크
- 인터넷 - ISP - 모뎀 - 공유기 - 컴퓨터

### 기업용 네트워크
- 인터넷 - ISP전용선 - 라우터 - 방화벽 - L3백본 - L2스위치 - 컴퓨터   
　　　　　　　　　　　　　　　　  - L4로드밸런서 - DMZ - 서버

### 클라우드 네트워크
- 인터넷 - Route53 - IGW - VPC - ELB - Auto Scaling - Security Group - EC2


## OSI 7 Layer
- 정의 - 네트워크 프로토콜과 통신을 7 계층으로 표현
- 목적 - 프로토콜을 기능별로 나누고 계층별로 구분, 벤더간 호환성을 위한 표준 필요 -> 쉬운 접근성으로 기술의 발전

## OSI 7 Layer 모델
- Application - 응용 서비스 HTTP(웹), SMTP(메일)
- Presentation - 인코딩, 암호화, 압축
- Session - TCP / IP 통신을 연결 수립, 유지, 중단
- Transport - TCP / UDP
- Network - IP 통신, 라우팅
- Data Link - 이더넷, 랜카드, Mac 통신, 에러검출, 재전송
- Physical - 네트워크 하드웨어 전송 기술

### 1계층 - Physical
- 장치와 통신 매체 사이의 비정형 데이터의 전송을 담당
- 디지털 bit(0 & 1)를 전기, 무선 또는 광 신호로 변환
- 전송되는 방법, 제어 신호, 기계적 속성 등을 정의
- 케이블, 인터페이스, 허브, 리피터 등이 이에 속함

### 2계층 - Data Link
- 동일 네트워크 내에서 데이터 전송, 링크를 통해서 연결을 설정하고 관리
- 물리계층에서 발생할 수 있는 오류를 감지하고 수정
- MAC, LLC
- 모뎀, 스위치

### 3계층 - Network
- 다른 네트워크로 데이터 전송, IP 주소로 통신
- 출발지 IP에서 목적지 IP로 데이터 통신 시 중간에서 라우팅 처리
- 데이터가 큰 경우 분할 및 전송 후 목적지에서 재조립하여 메시지 구현
- IP통신과 라우팅
- L3 스위치, 라우터

### 4계층 - Transport
- 호스트 간의 데이터(서비스) 전송
- 오류 복구 및 흐름 제어, 완벽한 데이터 전송을 보장
- TCP / UDP
- L4 계층을 특정 하드웨어로 구분하기가 모호
- Port를 제어한다는 의미로 L4 로드 밸런서가 있음

### 5계층 - Session
- 로컬 및 원격 애플리케이션 간의 IP / Port 연결을 관리
- Session Table (netstat -an)

### 6계층 - Presentation
- 사용자 프로그램과 네트워크 형식간에 데이터를 변환ㅇ하여 표현과 독립성을 제공
- 인코딩, 디코딩, 암호화, 압축
- ASCII, JPG, MPEG

### 7계층 - Application
- 사용자와 가장 밀접한 소프트웨어
- 이메일 서비스 SMTP, 또는 파일전송 FTP 등
 
## TCP/IP란
- 네트워크 프로토콜의 모음으로 패킷 통신 방식의 IP와 전송 조절 프로토콜인 TCP로 이루어져 있다

## TCP/IP 모델
- Application - 응용 프로그램간 표준화 된 데이터 교환
- Transport - TCP / UDP
- Network - 패킷을 처리하고 다른 네트워크로 연결
- Network Interface - 물리 계층으로 네트워크 노드들을 상호 연결

## 캡슐화
- 송신 데이터에 필요한 정보를 헤더에 붙여서 다음 계층으로 보내는 기술
