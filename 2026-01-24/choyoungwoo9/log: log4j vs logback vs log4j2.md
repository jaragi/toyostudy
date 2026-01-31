# 2026-01-24 스터디 내용

## 학습 자료

### 1. Java 로깅 프레임워크: SLF4J, Log4j, Logback, Log4j2 비교
**작성자:** [@choyoungwoo9](https://github.com/choyoungwoo9)

[원문 보기](https://www.notion.so/log4j-vs-logback-vs-log4j2-2f20e5be088a8008aaa0c46c1d0be74a)

**요약:**
- SLF4J는 Java 로깅 API의 추상화 계층으로, Facade 패턴을 사용하여 로그 구현체 변경을 용이하게 함.
- Log4j는 과거 대표 로깅 프레임워크였으나 2015년 서비스 종료되었으며, SLF4J 기본 지원을 위해 추가 의존성이 필요함.
- Logback은 Log4j의 개선 버전으로 SLF4J 네이티브 지원, 성능 개선, 고급 필터링 및 자동 재로딩 기능을 제공하며 Spring Boot의 기본 로깅 구현체임.
- Log4j2는 최신 프레임워크로 Logback의 장점에 람다 기반 Lazy Logging, 비동기 로거, Garbage-free 모드 등 성능 및 효율성을 극대화하는 기능들을 추가함.

---

