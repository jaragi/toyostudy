# 2026-01-31 스터디 내용

## 학습 자료

### 1. JPA 엔티티 기본 키(PK) 생성 전략
**작성자:** [@kiteB](https://github.com/kiteB)

[원문 보기](https://lacy-pirate-0e4.notion.site/JPA-ID-2f860934694c80b18187ee45e69f3248)

**요약:**
- JPA에서 엔티티의 기본 키(PK)는 직접 할당하거나 JPA를 통해 자동 생성할 수 있다.
- **직접 할당**: 애플리케이션에서 ID 값을 직접 생성하여 할당하며, 비즈니스적 의미가 있거나 외부 식별자를 유지해야 할 때 사용된다.
- **자동 생성**: `@GeneratedValue(strategy = GenerationType.XXX)`를 사용하여 JPA가 PK를 자동으로 생성하도록 위임한다.
- **IDENTITY**: DB에 PK 생성을 위임하며, INSERT 후 PK가 생성되어 쓰기 지연이 동작하지 않는다.
- **SEQUENCE**: DB 시퀀스를 이용하며, DB에 가지 않고 번호를 먼저 받아와 쓰기 지연이 가능하다.
- **TABLE**: 키 생성을 위한 별도 테이블을 사용하며, 모든 DB에서 사용 가능하지만 성능상 불리할 수 있다.
- **AUTO**: DB 방언에 따라 `IDENTITY`, `SEQUENCE`, `TABLE` 중 하나를 자동 선택한다.
- **UUID (Hibernate 6+)**: 애플리케이션에서 UUID를 즉시 생성하며, DB에 의존하지 않지만 인덱스 성능에 상대적으로 불리할 수 있다.

---

