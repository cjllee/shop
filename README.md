# shop
## 프로젝트 환경설정
### 사용기술
- Spring Boot
- Gradle
- Thymeleaf
- JPA
- HIBERNATE
- Tomcat

## 요구사항 분석
### 기능목록

회원기능
- 회원 등록
- 회원 조회

상품 기능
- 상품 등록
- 상품 수정
- 상품 조회

주문 기능
- 상품 주문
- 주문 내역 조회
- 주문 취소

기타 요구사항
- 상품은 재고 관리가 필요하다
- 상품의 종류는 도서,음반,영화가 있다
- 상품을 카테고리로 구분할 수 있다.
- 상품 주문시 배송 정보를 입력할 수 있다


## 도메인 모델 설계
![](https://velog.velcdn.com/images/cjllee/post/7c775b87-65c0-423f-91e8-0a69f8de8c6b/image.png)

## 엔티티 설계
![](https://velog.velcdn.com/images/cjllee/post/cfbfa9b0-4038-436c-b505-f5ac6bb0e047/image.png)

## 테이블 설계
![](https://velog.velcdn.com/images/cjllee/post/d881a8a3-ea18-465f-880b-94bf2e76af1e/image.png)

## JPA로 엔티티와 테이블 ORM으로 매핑

## 어플리케이션 아키텍처 구성
![](https://velog.velcdn.com/images/cjllee/post/4d5446aa-b441-4bfe-b0e1-460a3324a5fd/image.png)
### 계층형 구조 사용
- controller,web:웹 계층
- service: 비즈니스 로직, 트렌잭션 처리
- repository: JPA를 직접 사용하는 계층, 엔티티 매니저 사용
- domain: 엔티티가 모여 있는 계층, 모든 계층에서 사용

### 패키지 구조
- domain
- exception
- repository
- service
- web

## 핵심 비즈니스 로직 개발
- 회원 상품 주문 도메인 개발
- 핵심 비즈니스 로직 개발

## 웹 계층 개발
