# 2026-01-17 스터디 내용

## 학습 자료

### 1. 신뢰할 수 있고 확장 가능하며 유지보수하기 쉬운 애플리케이션
**작성자:** [@kiteB](https://github.com/kiteB)

[원문 보기](https://lacy-pirate-0e4.notion.site/2cc60934694c80518d0ac3c6acd02af6)

**요약:**
- 현대 애플리케이션은 데이터 중심(Data-Intensive) 시스템으로, 데이터의 양과 복잡도가 CPU 성능보다 중요
- 소프트웨어 설계 시 고려해야 할 3가지 원칙: 신뢰성(결함이 있어도 정상 동작), 확장성(부하 증가에 대응), 유지보수성(운용성, 단순성, 발전성)
- 트위터 팬 아웃 문제: 읽기 시점 계산 vs 쓰기 시점 계산의 트레이드오프 존재
- 트위터는 일반 사용자는 쓰기 시점 계산, 유명인은 읽기 시점 계산을 사용하는 혼합 모델 채택

---

### 2. Gradle
**작성자:** [@choyoungwoo9](https://github.com/choyoungwoo9)

[원문 보기](https://pleasant-rambutan-86b.notion.site/Gradle-2ea0e5be088a8034bc70d45990d2a0e5?source=copy_link)

**요약:**
- Gradle은 빌드/실행/테스트/패키징 작업을 일관되게 자동화하는 빌드 엔진으로, 프로젝트 실행 규칙을 코드로 고정
- 플러그인(확장 팩)을 통해 Task와 DSL을 추가하며, repositories에서 라이브러리 저장소를 지정
- dependencies에서 스코프(implementation, testImplementation 등)별로 의존성을 선언해 프로덕션과 테스트 환경을 분리
- Task는 프로젝트에서 수행 가능한 행동 단위로, Gradle이 의존 관계를 그래프로 관리하고 자동 실행
- java toolchain, kotlin compilerOptions, tasks 블록 등을 통해 환경 차이를 무시하고 일관된 빌드 규칙 적용

---

### 3. Claude Code를 활용한 병렬 작업 워크플로우
**작성자:** [@kimsj-git](https://github.com/kimsj-git)

[원문 보기](https://www.notion.so/2ea9ba488b1f807ab0d2f32ce866a0a9?source=copy_link)

**요약:**
- PRD 작성 → TaskMaster MCP로 태스크 분할 → Git Worktree로 환경 격리 → 병렬 실행 → PR 병합의 워크플로우
- Git Worktree를 사용해 각 태스크마다 독립된 작업 공간(../worktrees/<branch-name>)을 생성하여 코드 충돌 방지
- 각 터미널에서 별도의 Claude 인스턴스를 실행하여 동시에 여러 태스크를 병렬로 수행
- Custom Skill(.claude/commands/start-task.md)을 통해 워크트리 생성 및 환경 설정 절차 자동화
- 작업 완료 후 각 브랜치를 PR로 생성하여 코드 리뷰 및 병합 진행

---

## 참고사항

각 링크를 클릭하여 자세한 내용을 확인하세요.
