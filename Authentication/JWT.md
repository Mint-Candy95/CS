# JWT(Json Web Token)
===========

# 세션인증
------------

> 특징
 - MAP(Multiple Page Application)
 - 전통적
 - Server Side Rendering
 - 서버의 메모리, 클라이언트의 쿠키
 - 성능, 보안을 위해 대규모 시스템 구축에 전략적으로 사용
 - 전통적인 PHP, JSP, ASP 등

> 장점
 - 서버 측 사용자 인증 확인이 분명하고 쉬움
 - 서버 측에서 세션 정보를 관리
 - 클라이언트에 의한 변조가 어려움
 - 부가정보가 적어 Server.Client 송수신 데이터가 상대적으로 적음

> 단점
- 대규모 서비스로의 Scale-Up 시 메모리 성능 부하 문제
-  Redim, Memcached등 별도 메모리 관리 시스템 염두
-  쿠키는 단일 도메인 및 서브 도메인에서만 동작하므로, 여러 도메인 사용시 관리의 부담

# 토큰 인증
-------------

> 특징
- SPA(Single Page Application)
- 비교적 최신 트렌드 
- 사용자 경험이 중요한 복잡한 Front-end 구현의 적합
- Vue, React, Angular 등
- 웹 브라우저 외 모바일, IoT 등 다양한 플랫폼 및 디바이스의 클라이언트를 하나의 Back-end 서비스 API로 대응 가능

> 장점
- 멀티 플랫폼 서비스 대응에 유리
- 토큰 정보를 클라이언트가 보유
- 서버의 Scale-up 부담이 상대적으로 낮음
- 클라이언트 세션 관리에 대한 서버 메모리 부담 감소
- 다양한 도메인 대응 부담 감소

> 단점

- 클라이언트 토큰 정보 탈취로 보안적인 부분의 상대적 취약 가능성
- 토큰에 Signature와 같은 부가정보가 있어, 세션 기반 인증에 비해 Server-Client간 주고받는 데이터 양 증가
- 토큰 인증을 위한 Database 조회 발생으로, DB 성능 부하의 가능성 존재