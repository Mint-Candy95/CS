## ORM(Object Relation Mapping)

# JPA(Java Persistance API)
> JPA는 Java에서 제공하는 API로 Java ORM 기술의 표준 명세를 제공. Spring Framework에서는 JAP와 JPA 구현체의 편리한 사용을 위해
> Spring Data JPA를 제공


- 장점 
  - 객체지향 개념 기반으로 데이터 관리
  - 비즈니스 로직 구현에 집중 가능
  - 테이블의 생성 및 관리 용이
  - Database Query 보다 객체에 집중
  - Database 제품 및 버전에 대한 종속성을 낮춰 개발의 효율성 증가
 
 - 단점
  - Query 중심의 DB처리에 비해 높은 복잡도
  - 복잡한 Query가 필요할 경우 성능 이슈 발생 확률 증가
  - 성능을 비롯한 여러가지 문제 해결 위한 높은 이해도 요구

# Hibernate
> Hibernate는 JPA의 구현체 역할을 하는 Java ORM 프레임워크이다. Hibernate 외에도 DAtaNucleus, EclipseLink 등의 JPA 구현체가 존재하며 Hibernate가 그중 가장 널리 사용되고 있다.

# QueryDSL
> Querydsl은 type-safe한 쿼리의 제작과 실행을 위해 사용하는 프레임워크이다. String으로 쿼리를 직접 작성할 때 발생할 수 있는 오타 혹은 잘못된 테이블의 참조, 낮은 가독성 등의 단점을 극복할 수 있게 도와준다. Querydsl을 사용하면 컴파일 시점에 선언한 Entity 클래스 기반으로 Q 클래스가 생성되므로, 더 안전한 DB 쿼리를 작성 할 수 있다.


