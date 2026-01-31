# 2026-01-24 스터디 내용

## 학습 자료

### 1. JPA Auditing: 엔티티 변경 이력 자동 추적
**작성자:** [@choyoungwoo9](https://github.com/choyoungwoo9)

[원문 보기](https://www.notion.so/SpringData-JPA-Auditing-2f10e5be088a80c2b0acee92b44795ae)

**요약:**
- JPA Auditing은 엔티티 생성/수정 주체와 시점을 자동으로 추적하는 기능입니다.
- @CreatedBy, @LastModifiedBy로 주체를, @CreatedDate, @LastModifiedDate로 시점을 지정합니다.
- 적용 방법은 메인 애플리케이션에 @EnableJpaAuditing, 엔티티에 @EntityListeners(AuditingEntityListener.class)를 추가하고, 필요시 AuditorAware 구현체를 작성합니다.

---

