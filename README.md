<img src="https://capsule-render.vercel.app/api?type=waving&color=auto&height=200&section=header&text=Welcome!&fontSize=70" />

## Hi there 👋
문제를 정의하고 데이터를 기반으로 증명하고 소통하는 개발자, 김진현입니다.

- [진현의 노션 포트폴리오 바로가기! 클릭](https://useful-capri-975.notion.site/Jinhyeon-s-notion-134878dac63080b6ad33c62221fc0fb1)

<br>

<h3 align="left">🛠 Tech Stack 🛠</h3>

<div align="left">
  <img src="https://img.shields.io/badge/java-%23007396.svg?&style=for-the-badge&logo=java&logoColor=white" style="height:28px;">
  <img src="https://img.shields.io/badge/Spring%20Boot-6DB33F.svg?&style=for-the-badge&logo=springboot&logoColor=white" style="height:28px;">
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1.svg?&style=for-the-badge&logo=postgresql&logoColor=white" style="height:28px;">
  <img src="https://img.shields.io/badge/Redis-DC382D.svg?&style=for-the-badge&logo=redis&logoColor=white" style="height:28px;">
  <img src="https://img.shields.io/badge/Kafka-231F20.svg?&style=for-the-badge&logo=apachekafka&logoColor=white" style="height:28px;">
  <img src="https://img.shields.io/badge/Docker-2496ED.svg?&style=for-the-badge&logo=docker&logoColor=white" style="height:28px;">
</div>
<br>
<div align="left">
  <img alt="HTML5" src="https://img.shields.io/badge/HTML5-E34F26.svg?&style=flat-square&logo=HTML5&logoColor=white"/>
  <img alt="CSS" src="https://img.shields.io/badge/CSS-1572B6.svg?&style=flat-square&logo=CSS3&logoColor=white"/>
  <img alt="Vue.js" src="https://img.shields.io/badge/Vue.js-4FC08D.svg?&style=flat-square&logo=Vue.js&logoColor=white"/>
  <img alt="Next.js" src="https://img.shields.io/badge/Next.js-000000.svg?&style=flat-square&logo=next.js&logoColor=white"/> 
  <img alt="JavaScript" src="https://img.shields.io/badge/JavaScript-F7DF1E.svg?&style=flat-square&logo=JavaScript&logoColor=white"/>
  <img alt="TypeScript" src="https://img.shields.io/badge/Typescript-0058CC?style=flat-square&logo=TypeScript&logoColor=white">
</div>

<br>

### 🚀 Projects & My Contributions

#### 🏁 [1:1 (MSA 기반 스포츠 승률 예측 시스템)](https://github.com/11trillion/1-1)
> Game 도메인 아키텍처 설계 및 대규모 조회/수정 트래픽 병목 해결
- 동시성 제어 및 데이터 정합성 보장: 관리자 동시 업데이트 시 발생하는 Lost Update 문제를 해결하기 위해 JMeter로 부하 테스트(50~200 Threads) 진행. 금전적 정산 오류 차단이 최우선인 도메인 특성에 맞춰 비관적 락(Pessimistic Lock)을 채택하여 데이터 정합성 100% 보장.
- 대규모 트래픽 조회 성능 최적화: 트래픽 폭증 대비 CQRS 패턴 적용. 5만 건 부하 테스트 결과, 단건 조회 응답 시간을 45% 개선하고 꼬리 지연(P95)을 2.7배 감소시킴.

#### 🍀 [LuckyVicky Logistics (MSA 기반 B2B 물류 시스템)](https://github.com/LuckyVickyLogistics/backend-v1)
> Product / Order 핵심 도메인 설계 및 분산 환경 데이터 정합성 유지
- DDD 기반 설계: 상품 수량에 대한 불변식 검증 및 재고 변경 시 상태 전이 규칙을 적용하여 분산 환경에서의 안정적인 로직 처리 구현.
- 인가 처리 고도화: 역할(Role) 기반의 JPA 쿼리 레벨 조회 권한 필터링 적용.

#### 🍱 [곧감 Goat-Gam (음식 주문 배달 플랫폼 MVP)](http://github.com/orgs/1-6P/repositories)
> Restaurant 도메인 설계 및 API 보안/예외 처리 고도화
- 권한 및 소유권 검증: JWT 토큰 기반으로 식당 정보 수정/삭제 시 소유권(OwnerId)을 이중 검증하여 타인의 식당 정보 접근을 차단하는 로직 추가.
- 예외 처리: Custom AccessDeniedHandler를 구현하여 Spring Security 권한 제어(403) 시 명확한 에러 응답(JSON)을 반환하도록 개선.
