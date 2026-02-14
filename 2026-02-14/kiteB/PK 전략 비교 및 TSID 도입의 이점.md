# 2026-02-14 스터디 내용

## 학습 자료

### 1. PK 전략 비교 및 TSID 도입의 이점
**작성자:** [@kiteB](https://github.com/kiteB)

[원문 보기](https://lacy-pirate-0e4.notion.site/TSID-30660934694c805eac26cc9bb5ff3c5d?source=copy_link)

**요약:**
- AUTO_INCREMENT와 SEQUENCE는 단일 DB 환경에 적합하지만 DB 의존성이 높고 분산 환경에 부적합합니다.
- UUID(v4)는 분산 환경에 적합하지만 무작위성으로 인해 인덱스 효율이 떨어집니다.
- TSID는 시간 기반으로 정렬 가능하며, 분산 환경에서도 고유성을 보장하는 64비트 정수형 식별자입니다.
- TSID는 DB 락 대기 시간을 줄여 데드락 및 Gap Lock을 완화하고, DB 의존성을 낮춰 다중 DBMS 환경에서 표준화 및 확장성을 높입니다.
- TSID는 라이브러리 추가 후 엔티티에 적용하여 애플리케이션에서 ID를 생성할 수 있습니다.

---

