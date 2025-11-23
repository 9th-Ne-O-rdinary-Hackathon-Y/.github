# 커핏 Career-Fit
<img width="1920" height="1080" alt="표지" src="https://github.com/user-attachments/assets/730f830f-fe00-4bcb-88e6-5ed7e5346afd" />
일하는 방식 기반 성향 테스트로, 나에게 맞는 직업을 찾아주는 **행동 데이터 기반 커리어 내비게이션 서비스**

### 🧡 팀원을 소개합니다
<div align=center><table>
  <tr>
        <td align="center"><a href="https://github.com/gs0428"><img src="https://avatars.githubusercontent.com/u/114225974?v=4" width="100px;" alt=""/><br /><b>gs0428</b></a><p>레니</p></td>
          <td align="center"><a href="https://github.com/hyun907"><img src="https://avatars.githubusercontent.com/u/159671505?v=4" width="100px;" alt=""/><br /><b>hyun907</b></a><p>현이</p></td>
          <td align="center"><a href="https://github.com/51taek"><img src="https://github.com/51taek.png" width="100px;" alt=""/><br /><b>51taek</b></a><p>앨런</p></td>
          <td align="center"><a href="https://github.com/YoonchulChung"><img src="https://github.com/YoonchulChung.png" width="100px;" alt=""/><br /><b>YoonchulChung</b></a><p>알렉스</p></td>
          <td align="center"><a href="https://github.com/gyeonseo"><img src="https://github.com/gyeonseo.png" width="100px;" alt=""/><br /><b>gyeonseo</b></a><p>견서</p></td>
      



   </tr>
</table></div>
<br>

## 🔍 핵심 문제 및 솔루션

### 1. 핵심 문제

20대는 **직업 정보 부족**이 아니라 **나에 대한 정보 부족** 때문에 진로에서 헤맵니다.
* 기준 없이 진로를 선택 → 적성·환경 불일치 → 잦은 재탐색 루프

### 2. 솔루션

커핏은 설문이 아닌 **“행동 데이터”로 성향을 측정**합니다.

* 세 가지 미니게임을 통해 **반응 속도, 정확도, 우선순위, 판단 방식, 위험 감수 성향, 협업 성향**을 수집
* 고민보다 **직관적 반응**이 나오도록 설계
* 수집된 행동 데이터를 바탕으로
  * 업무 스타일(일하는 방식) 분석
  * 8개 직무군에 대한 알고리즘 기반 **적합도 점수 계산**
  * 상위 직무 2개를 추천하고, 즉시 관련 정보·영상·교육으로 연결

---

## 🧩 주요 기능

<img width="1920" height="1080" alt="13" src="https://github.com/user-attachments/assets/18f5b21c-aca6-4637-a08a-77f4f22b56f7" />


### 1. 미니게임 기반 성향 측정

1. 별 맞추기 게임 (정확도 + 의사결정 속도)
* 화면을 움직이는 별을 중앙에 맞추고 STOP을 누르는 게임
* 중심과의 거리 → **정확도 추구 정도**
* STOP까지의 시간 → **의사결정 속도**

2. 작업 스타일 선택 (추론/협업/리스크/우선순위)
* 5개의 상황형 질문에 대해 A/B 선택
* 문항별 **5~12초 시간 제한**으로 자기보고 편향을 줄이고 **즉각적 성향**을 측정

3. 업무 우선순위 선택 (실제 상황 기반 의사결정)
* 3가지 업무 요청 중 무엇을 먼저 처리할지 선택
* 12초 이내 선택, 초과 시 타임아웃
* 실제 업무 상황을 가정해 **우선순위·판단 방식**을 복합적으로 측정

### 2. 성향 분석 및 결과 리포트
* 위험 감수 성향, 추론 성향, 의사결정 방식 등을 종합해 **업무 스타일 카드 제공**
* 6가지 핵심 지표로 정량화:
  * 정확도 vs 속도
  * 리스크 감수 성향
  * 추론/논리 중심 vs 직관 중심
  * 협업 성향
  * 우선순위 판단 방식 등

### 3. 직무 매칭 및 정보 제공
* 8개 직무군에 대해 **성향 적합도 점수** 계산
* 상위 2개 직무를 카드 형태로 노출
* 각 직무 카드에서:
  * 직무 설명
  * 관련 영상
  * 부트캠프/교육 링크 등
    → **성향 기반 직무 탐색 → 학습/준비 단계**까지 자연스럽게 이어지는 구조
    
---

## 프로젝트 아키텍처
<img width="617" height="442" alt="career-fit-infra" src="https://github.com/user-attachments/assets/de8d4099-286b-4b71-84de-a2efa7c127c1" />

---

## 🛠 프론트 기술 스택

* **Framework & Language**

  * React 19.2.0
  * TypeScript 5.9.3
  * Vite 7.2.4

* **Routing & 상태 관리**

  * React Router DOM 7.9.6
  * Zustand 5.0.8 (전역 상태 관리 – 게임 결과 등)
  * TanStack Query 5.90.10 (서버 상태 캐싱)

* **폼 & 검증**

  * React Hook Form 7.66.1
  * Zod 4.1.12 (스키마 기반 타입 검증)

* **스타일 & 유틸**

  * Tailwind CSS 4.1.17
  * Ky 1.14.0 (HTTP 클라이언트)
 
## 🛠 백엔드 기술 스택

  * Java 21

    - 최신 문법(패턴 매칭, 레코드, 가상 스레드 등)을 지원해 가독성과 유지보수성이 향상됩니다.  
    - 성능 최적화가 크게 개선되어 대규모 애플리케이션에서도 안정적으로 동작합니다.  
    - 장기 지원(LTS) 버전으로 안정적인 운영이 가능합니다.
    
  * Spring Boot 3.4.9

    - 스프링 생태계와 완벽하게 호환되며 최신 기능 및 보안 패치가 포함되어 있습니다.  
    - 자동 설정(Auto Configuration) 기반으로 빠르게 애플리케이션을 구성할 수 있습니다.  
    - REST API, 데이터 액세스, 시큐리티 등이 통합되어 있어 비즈니스 로직 개발에 집중할 수 있습니다.
    
  * Spring Data JPA

    - 반복적이고 보일러플레이트가 많은 데이터 액세스 코드를 간소화합니다.  
    - 명확한 도메인 모델 중심 개발이 가능하며, QueryDSL 등과 조합해 강력한 쿼리 작성이 가능합니다.
    
  * PostgreSQL

    - ACID 트랜잭션을 충실히 준수하는 안정적인 오픈소스 RDBMS입니다.  
    - JSONB 등 고급 기능을 제공해 유연한 구조 관리가 가능합니다.  
    - 대규모 트래픽 환경에서도 성능과 확장성이 뛰어나며, Spring Data JPA와 매우 잘 어울립니다.

---

## 🚀 시작하기

### 1. 설치

```bash
pnpm install
```

### 2. 개발 서버 실행

```bash
pnpm dev
```

브라우저에서 아래 주소로 접속:

```text
http://localhost:5173
```

### 3. 빌드 및 프리뷰

```bash
pnpm build
pnpm preview  # 빌드 결과 미리보기
```

### 4. 코드 품질 관리

```bash
pnpm lint     # 린트 검사
pnpm format   # 코드 포맷팅
```
