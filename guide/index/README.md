## 기본 테스트

- 쿠버네티스(minikube) 설치
- kubectl 설치.

## minikube
- 모든 기능을 테스트 하긴 어렵지만... 기본 기능을 익히기엔 충분하다.

```sh
# minikube 상태확인
minikube status

# minikube 실행
minikube start

# 특정 k8s 버전 실행
minikube start --kubernetes-version=v1.20.0

# 특정 driver 실행
minikube start --driver=virtualbox --kubernetes-version=v1.20.0

# minikube ip 확인 (접속테스트시 필요)
minikube ip

# minikube 종료
minikube stop

# minikube 제거
minikube delete
```

### 워드프레스 배포

- 도커 컴포즈를 사용했었다면 다음과 같이 배포했을 것

```yml
version: "3"

services:
  wordpress:
    image: wordpress:5.5.3-apache
    environment:
      WORDPRESS_DB_HOST: mysql
      WORDPRESS_DB_PASSWORD: password
    ports:
      - "30000:80"

  mysql:
    image: mysql:5.6
    environment:
      MYSQL_ROOT_PASSWORD: password
```

- 다음은 쿠버네티스를 이용해 배포해보자 !

