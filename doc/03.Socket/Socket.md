# Socket
 - 양방향 데이터 통신을 위한 입구 역할을 한다.
 - 특정 Port와 묶여있다(bind)
 - 소켓은 정해진 통신 프로토콜에 맞게 만들어져야 하며, 보통 OSI 7계층 중 4계층 Transport 계층 상에서 동작하는 소켓을 사용합니다. 

클라이언트 Process에서 요청 -> 소켓 -> 포트 -> 전송 계층 ->  인터넷 계층 -> 인터넷망 -> 인터넷 계층 -> 전송 계층 -> 포트 -> 소켓 -> 서버의 Prcoess에 전달

![소켓 구조](https://github.com/johnson434/python-network-programming/assets/150678238/19c73069-a406-4eca-b239-1ffd1ead6a20)


# 파이썬에서 사용되는 Socket 명령어
 - socket.socket() : 소켓을 만듬.
 - s.bind(host, port) : 소켓과 호스트의 아이피와 port를 묶는다.
 - s.send() : 메시지를 상대에게 보낸다.
 - s.listen() : 상대방이 메시지를 보내는지 체크.
 - s.recv() : 상대방이 메시지를 받는다.
 - s.close() : 스켓을 닫는다.
