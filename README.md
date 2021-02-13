# 쿠버네티스

- 쿠버네티스는 컨테이너를 쉽고 빠르게 배포/확장하고 관리를 자동화 해주는 오픈소스 플랫폼.

- 도커 컴포즈나 기타 컨테이너 오케스트레이션 도구랑 비슷..하다

- 컨테이너 오케스트레이션이란
    - 여러개의 서버에 컨테이너를 배포하고 운영하면서
    - 서비스 디커버리 같은 기능을 이용하여
    - 서비스 간 연결을 쉽게 해주는 것.

## 쿠버네티스의 특징

- 생태계
    - 수많은 회사들이 참여하고 점점 확장해 나가고 있다.
- 다양한 배포 방식
    - 단순 웹/서버 배포 뿐 아니라 여러 배포형태를 지원한다.

- Ingress 설정
    - 다양한 웹 애플리케이션을 하나의 로드밸런스로 서비스 하기 위해 Ingress 기능을 지원한다.
    - 기존 프록시 서버 (Nginx, Apache에서 하던것들)의 역할을 쿠버네티스 Ingress가 자동화하면서, 기존 프록시 서버에서 사용하는 설정을 그대로 사용 가능하다 !!
- 클라우드지원 
    - 짱짱맨
- 네임스페이스/레이블
    - 하나의 클러스터를 논리적으로 구분해서 사용 가능하다.
- 오토스케일링 등..

## 단점
- 개복잡하다.