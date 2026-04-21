# AI Robotics — 의료/돌봄 도메인 리서치 (간병 로봇 기획서용)

> **기준일**: 2026-04-18 | **"최근 1년"** = 2025-04 ~ 2026-04
> 본 문서는 채택 아이디어 **"로봇 간병인 서비스"** 기획서 작성을 위한 의료·돌봄 영역 발췌본이다.
> 원본: [archive/RESEARCH.md](archive/RESEARCH.md) — 14개 영역 전체 리서치 중 의료/수술/재활(A-4), 서비스/접객(A-5), 가정/케어(A-7) 영역과 cross-cutting 기술 트렌드(VLA, FM, Embodied AI, Sim-to-Real)만 추출.
> 상세 출처 드래프트: [research-drafts/group2-medical-service-agri.md](research-drafts/group2-medical-service-agri.md)

## 목차

- [공통 매크로 지표](#공통-매크로-지표-참조)
- [Part 1. 영역 지도](#part-1-영역-지도)
  - [A-4. 의료/수술/재활 로봇](#a-4-의료수술재활-로봇)
  - [A-5. 서비스/접객 로봇](#a-5-서비스접객-로봇)
  - [A-7. 가정/케어 로봇](#a-7-가정케어-로봇)
- [Part 2. 영역별 페인포인트 & 기존 서비스](#part-2-영역별-페인포인트--기존-서비스)
- [Part 3. 주목 기술 트렌드 (Cross-cutting)](#part-3-주목-기술-트렌드-cross-cutting)
- [Part 4. 출처 (의료/돌봄 발췌)](#part-4-출처-의료돌봄-발췌)

---

## 공통 매크로 지표 (참조)

| 지표 | 수치 | 출처 |
|---|---|---|
| 산업용 로봇 신규 설치 2024 | **542,000대** (4년 연속 50만 돌파) | IFR World Robotics 2025 (2025-09) |
| 2025 전망 | 575,000대 (+6%) | IFR 2025 |
| 협동로봇(cobot) 설치 2024 | **64,500대** (비중 2.8%→11.9% since 2017) | IFR 2025 |
| 한국 로봇 밀도 | 제조업 1만 명당 **1,012~1,220대** (세계 1위) | IFR 2024/2025 |
| 서비스로봇(전문용) 2024 판매 | **약 20만대**(+9%), RaaS +31% | IFR 2025-10-07 |
| Hospitality 로봇 2024 | **42,000대+** (YoY −11%) | IFR 2025 |
| 한국 정부 정책 | 제4차 지능형로봇 기본계획: 2030년까지 3조원, 100만대 보급 | 산업부 |
| K-휴머노이드 연합 | 2025-04-10 출범, 1조원+ 투자, 2028 상용(60kg 이하·20kg 페이로드·50 DoF·2.5m/s) | 정책브리핑 |

---

## Part 1. 영역 지도

### A-4. 의료/수술/재활 로봇

- **What**: 수술보조 로봇, 재활 외골격, 병원 물류·간호 보조. 세계 수술로봇 **2025 US$ 11.33B → 2035 US$ 38.27B** CAGR 12.95%(SNS Insider 2026-04-13) / 2025 US$ 13.69B → 2030 US$ 27.14B(MarketsandMarkets). 세계 의료로봇 2029년 약 **45조원**(GM Insights). **da Vinci** 설치 11,106대(2025-12-31, YoY +12%), 2025년 시술 315만 건(+18%). 한국 로봇 수술 **연 약 1만 건**.
- **주요 플레이어**: 해외 — Intuitive Surgical(da Vinci 5, 2025-07 CE, 2025 4Q 532대 선적), Medtronic(Hugo RAS, 2025-12-03 FDA 비뇨기), Stryker(Mako RPS 2026-02 핸드헬드), Diligent Robotics(Moxi 30만+ 약제 배송, Moxi 2.0 2026 상반기), Aethon TUG(500+ 병원). 국내 — **큐렉소**(2025 매출 **745억원** +34%, 2026 FDA 목표), 고영테크(지니언트 FDA·PMDA), 엔젤로보틱스(엔젤슈트 H10 2025 출시), 로엔서지컬(자메닉스), 엘엔로보틱스.
- **최근 1년 트렌드**:
  - **VLA 의료 적용**: RoboNurse-VLA, 2026 임상 진입 예상.
  - da Vinci 5가 FDA 승인 최초 integrated force feedback haptic(2024-03 → 2025 확산).
  - **Mako RPS로 console → handheld** 전환(2026-02).
  - **Foxconn/NVIDIA Nurabot** — 대만 병원 2025-04 테스트 → 2026 초 상용, 간호 업무 20–30% 절감.
  - 원격수술 타당성 리뷰 다수(Springer 2025).
  - 병원 물류 파트너십(Swisslog×Diligent 2025-10).

### A-5. 서비스/접객 로봇

- **What**: 호텔·식당·공항·매장 안내·서빙 로봇. 2024 전문용 서비스로봇 20만대+(+9%), Hospitality 42,000대+(YoY −11%) — **수요 포화 신호**. 커머셜 서비스로봇 2025 US$ 8.09B → 2034 US$ 30.89B CAGR 21.3%(IntelMarket). 글로벌 85% 중국 벤더(People's Daily 2025-12-08).
- **주요 플레이어**: 해외 — Pudu Robotics(KettyBot Pro, 80국+), Keenon(60국+), SoftBank Robotics(Pepper). 국내 — **베어로보틱스**(Servi 20국+ 2만대+, **2025-05 LG 계열사 편입**), LG전자(CLOi, 조선호텔·인국공, CES 2026 CLOiD), KT, 로보티즈(일개미/집개미), **현대위아 H-motion**(CES 2026 첫 공개, 2028년 4,000억원 매출 목표).
- **최근 1년 트렌드**:
  - **LG전자 서비스로봇 본격화**(베어로보틱스 경영권 2025-05, 조선호텔·인국공).
  - 생성형 AI 접목 대화형 가이드(CLOi LLM 탑재).
  - 조리 로봇 연계(Miso Flippy, Chipotle Hyphen Makeline 350 bowl/hr, Sodexo ART, Fortune 2026-02-26).
  - RaaS +31% 성장(IFR 2025).
  - 휴머노이드/모바일 매니퓰레이터(현대위아 H-motion, 로보티즈 집개미 로봇팔).

### A-7. 가정/케어 로봇

- **What**: 청소 로봇, 노인돌봄/실버, 컴패니언/펫 로봇. 로봇청소기 2025 **약 320억 달러** CAGR 27.6%(Research Nester). 국내 상반기 **Roborock 46%**(1위), 삼성 22%(+6%p), 에코백스 14%→4% 급락. 초고령사회 — **2025 65세+ 1,084만 명**(20%+), 2072년 47.7%(서울신문 2026-01-04). AI 돌봄 '다솜' 누적 2만명, 대화 8,555만 건.
- **주요 플레이어**: 로봇청소기 — Roborock(中), 삼성 Bespoke AI, LG, Ecovacs(中). 돌봄 — 효돌(MS Azure), 원더풀플랫폼 다솜. 컴패니언 — Sony Aibo($3,000+), CASIO Moflin($400), KEYi Loona(ChatGPT-4o). **홈 AI** — 삼성 Ballie(Gemini, 2026 타깃, 3회 지연), LG Q9(MS Azure OpenAI, 2025 말). 웨어러블 — 삼성 봇핏 EX1.
- **최근 1년 트렌드**:
  - 생성형 AI/LLM 내장화(Ballie=Gemini, Q9=Azure OpenAI+Bing).
  - LG Q9 2025-03 베타 → 2025 말 정식, Q9 SDK 선공개.
  - **Ballie 출시 3회 지연**, 2025 미출시 → 2026 타깃.
  - 돌봄 로봇 다모달 관찰(다솜 카메라로 먼저 말 걸기).

---

## Part 2. 영역별 페인포인트 & 기존 서비스

### A-4. 의료/수술/재활 로봇

**현장 페인포인트**
1. 간호 인력난·단순업무 과부하 — WHO 2030 1,000만 명 부족. Moxi 약제·검체 배송으로 대체.
2. 햅틱 부재로 tissue injury 리스크(MDPI Sensors 2026).
3. 국내 수술로봇 상용화 지연 — 식약처 + 혁신의료기술심사 **5년 누적**(한국경제 2025-11).
4. 재활로봇 접근성 — 수가 미비로 자비 부담.

**기존 서비스/제품**

| 제품 | 기업 | 용도 | 현황 |
|---|---|---|---|
| da Vinci 5 | Intuitive Surgical | 복강경 수술 | 2025 풀런칭, 힘 피드백 |
| Hugo RAS | Medtronic | 비뇨/부인/일반외과 | 2025-12 FDA 비뇨기 |
| Mako RPS | Stryker | 무릎 정형외과 핸드헬드 | 2026-02 한정 출시 |
| Moxi 2.0 | Diligent | 병원 약제/물품 배송 | 2026 상반기 |
| TUG | Aethon | 병원 AMR | 500+ 병원 |
| 큐비스-조인트 | 큐렉소 | 인공관절 | 식약처 허가, 동남아 수출 |
| 지니언트 크래니얼 | 고영테크 | 뇌수술 | FDA·PMDA 승인 |
| 엔젤슈트 H10 | 엔젤로보틱스 | 산업용 웨어러블 | 2025 상반기 출시 |
| Nurabot | Foxconn | 간호 보조 | 2026 상용화 |

**기술적 공백**
- Level 2+ 자율수술 검증·허가 파이프라인.
- 소형·멸균·고정밀 촉각 센서.
- 의료 전용 VLA용 공개 병원 데이터셋.
- 보행재활 홈케어(원격 모니터링·수가 모델).
- 국내 인허가 심사 + RWE 연계 제도.

### A-5. 서비스/접객 로봇

**현장 페인포인트**
1. 피크타임 병목 — 좁은 통로 정지·회피로 사람보다 느려짐(뉴시스).
2. 건물 인프라 제약 — 다층 식당/호텔 엘리베이터 연동·문턱 실패.
3. 주문→탑재→테이블번호 입력 수작업(그린포스트).
4. 배터리/안전 — 서울 노원구 서빙로봇 충전 화재.

**기존 서비스/제품**

| 제품 | 기업 | 유형 | 용도 |
|---|---|---|---|
| Servi / Servi Plus / Servi Mini | 베어로보틱스 | 서빙 | 식당/호텔 |
| CLOi ServeBot | LG전자 | 서빙 트레이 | 호텔/식당 |
| KettyBot Pro | Pudu | 서빙+AD | 식당 |
| BellaBot | Pudu | 서빙 | 식당 |
| DINERBOT T8/T10 | Keenon | 서빙 | 식당 |
| 집개미 | 로보티즈 | 실내 배송 로봇팔 | 호텔·고층 |
| 일개미 | 로보티즈 | 실외 배송 | 도심·아파트 |
| H-motion | 현대위아 | 물류 | 창고·B2B |
| Flippy | Miso Robotics | 조리 | QSR |

**기술적 공백**
- 엘리베이터·문·보안게이트 API 표준.
- 피크타임 사회적 내비게이션(SAN).
- VLA 기반 주문 이해·자연 대화 일체형 서빙.
- 주방-홀 엔드투엔드 자동화.
- 서빙로봇 배터리·화재 안전 KC/KS 인증.

### A-7. 가정/케어 로봇

**현장 페인포인트**
1. 독거노인 응급 감지 지연(유니콘팩토리 2025-05).
2. 치매·인지저하 예방의 비접촉성(다솜·효돌 시장 증명).
3. 가정 내 다기기 제어 분산 → 통합 '집사' 수요.
4. 로봇청소기 '마무리'(먼지봉투·세제·구석) 공백.

**기존 서비스/제품**

| 제품 | 카테고리 | 주 기능 | 상태 |
|---|---|---|---|
| Roborock S 시리즈 | 청소 | 흡입+물걸레+AI 회피 | 국내 1위 |
| 삼성 Bespoke AI 스팀 | 청소 | 고온 스팀 물걸레 | 2024-2025 |
| 삼성 Ballie | 홈 AI 볼 | Gemini 대화·프로젝터 | 2026 예정(3회 지연) |
| LG Q9 클로이 | AI 에이전트 | 가전 제어·대화 | 2025 말 |
| 삼성 봇핏 EX1 | 웨어러블 | 보행보조 | 출시 준비 |
| 효돌 | 돌봄 인형 | 정서·복약·응급 | 판매 |
| 다솜 M/B/K | 돌봄 로봇 | 쌍방향 대화·치매예방 | 판매 |
| Sony Aibo | 펫 | 감정 표현 | $3,000+ |
| CASIO Moflin | 펫 | 성격 학습 | ~$400 |
| KEYi Loona | 펫 | ChatGPT-4o | 중가 |

**기술적 공백**
- 가정 자율 이동 이족/다족 케어 휴머노이드 상용 미성숙.
- 비접촉 의료 모니터링(호흡·심박 레이더) + 로봇 액추에이션 통합.
- 노인 발화·방언 특화 STT + 가정용 VLA 저전력 온디바이스.

---

## Part 3. 주목 기술 트렌드 (Cross-cutting)

> 간병 로봇 기획서의 "AI 기술 적용 방안" 항목 작성 시 참고. 자세한 내용은 [archive/RESEARCH.md](archive/RESEARCH.md) Part 3 참조.

### 3-1. Vision-Language-Action (VLA)

- **정의**: VLM 위에 로봇 **액션** 출력 헤드를 얹은 단일 정책 아키텍처.
- **왜 지금**:
  - 인터넷 스케일 VLM 사전학습 지식을 로봇 정책에 이식할 유일 경로.
  - 하나의 모델로 다중 embodiment·다중 task "generalist policy" 현실화.
  - 2025 오픈·상용 모델 대량 공개로 평가·파인튜닝 생태계 형성.
- **대표 성과 (최근 1년)**:
  - PI **π0.5** (2025-04, arXiv 2504.16054) — 처음 보는 가정 10~15분 청소
  - DeepMind **Gemini Robotics 1.5 + ER 1.5** (2025-09, arXiv 2510.03342) — 15 ER 벤치 SOTA
  - NVIDIA **GR00T N1.6** (CoRL 2025) — 32-layer DiT + Cosmos Reason
  - **RoboNurse-VLA** — 의료 전용 VLA, 2026 임상 진입 예상
- **한계**: 추론 지연(수백 ms), 온보드 GPU 요구, 액션 스키마 불통일, hallucination.

### 3-2. Foundation Models for Robotics

- **정의**: 인터넷+로봇 데이터로 사전학습한 대형 모델 → 로봇별 파인튜닝 패러다임.
- **왜 지금**:
  - 데이터 희소성 극복(한 번 훈련 → 여러 로봇 파인튜닝).
  - 대형 + 스타트업 동시 참전(NVIDIA, DeepMind, PI, TRI, Skild, Figure, HF).
  - FM + 시뮬 + 합성 + 벤치 통합 패키지화.
- **대표 성과**:
  - NVIDIA **Cosmos + GR00T-Dreams + GR00T N1.5/N1.6** 풀스택 (2025-05~09).
  - **Skild AI** omni-bodied, Series C $1.4B / $14B 밸류 (2026-01).
  - TRI + Boston Dynamics **LBM** Atlas 탑재 (2025-08-20).
- **한계**: 안전성 검증, cloud 의존, fine-tune 표준화 부재.

### 3-3. Embodied AI

- **정의**: 물리적 신체 에이전트의 지각-추론-행동 루프 AI. NVIDIA가 "Physical AI"로 확장.
- **왜 지금**: NVIDIA/Meta/DeepMind가 "AI의 다음 물결" 선언(CES 2025). 제조·물류·가사 경제 임팩트.
- **대표 성과**:
  - Gemini Robotics-ER 1.5/1.6 — embodied reasoning 벤치 SOTA.
  - Jensen Huang CES 2025 "The next frontier is physical AI".
  - **EmbodiedBench** (2025, arXiv 2502.09560) MLLM embodied agent 평가.
- **한계**: 과대 마케팅 용어화; embodied reasoning 벤치 ↔ 실 로봇 성능 상관 불명확.

### 3-4. Sim-to-Real

- **정의**: 시뮬레이터 학습 정책 → 실 로봇 전이(도메인 랜덤화, 디지털 트윈, real-is-sim).
- **왜 지금**: 실 데이터 희소 → 시뮬 의존 재상승. Newton·MJX로 수백만 에피소드 훈련.
- **대표 성과**:
  - **NVIDIA Newton**(DeepMind+Disney 공동, 2025) Isaac Lab 통합.
  - **Real-is-Sim**(2025-04, arXiv 2504.03597).
  - **"Reality Gap in Robotics" Survey**(UZH RPG, 2025-10, arXiv 2510.20808).
- **한계**: Dexterous manipulation은 시뮬 여전히 취약. 컨택트·마찰·variance 부정확.

---

## Part 4. 출처 (의료/돌봄 발췌)

> 전체 200+ 출처 목록은 [archive/RESEARCH.md](archive/RESEARCH.md) Part 4 참조. 본 섹션은 의료/돌봄 직접 관련 출처만 추렸다.

### 시장 / 통계

- [SNS Insider — Surgical Robots 2035](https://orthospinenews.com/2026/04/13/surgical-robots-market-size-is-projected-to-attain-usd-38-27-billion-by-2035-sns-insider/)
- [DataM Intelligence — Hospital Robotics Logistics & Pharmacy](https://www.datamintelligence.com/research-report/hospital-robotics-logistics-and-pharmacy-market)
- [Global Growth Insights — Soft Exoskeleton](https://www.globalgrowthinsights.com/market-reports/soft-exoskeleton-exosuits-and-wearable-robots-market-100266)
- [IntelMarket Research — Commercial Service Robotics 2026-2034](https://www.intelmarketresearch.com/global-commercial-service-robotics-forecast-market-26549)
- [Research Nester — Robotic Vacuum](https://www.researchnester.com/reports/robotic-vacuum-cleaner-market/8208)
- [Spherical Insights — Korea Surgery Robot](https://www.sphericalinsights.com/)
- [IFR Service Robots 2025](https://ifr.org/ifr-press-releases/news/service-robots-see-global-growth-boom) — 2025-10-07
- [IFR Global Robotics Race: Korea leads](https://ifr.org/ifr-press-releases/news/global-robotics-race-korea-singapore-and-germany-in-the-lead)

### 한국 — 인구·정책·기업·언론

- [서울신문 — 초고령사회](https://www.seoul.co.kr/news/newsView.php?id=20260104500049)
- [Korea Herald — 20% Koreans 65+](https://www.koreaherald.com/article/10648363)
- [한국경제 — 수술로봇 심사 10년](https://www.hankyung.com/article/2025112063341)
- [Forbes Korea — 국내 수술 로봇](https://www.forbeskorea.co.kr/news/articleView.html?idxno=400499)
- [로봇신문 — 큐렉소 2025 매출 745억](https://www.irobotnews.com/news/articleView.html?idxno=44779)
- [LG Newsroom — LG전자 베어로보틱스](https://live.lge.co.kr/2501-lg-bear-robotics/)
- [LG Newsroom — CLOiD CES 2026](https://www.lg.co.kr/media/release/29723)
- [LG Newsroom — Q9 AI 에이전트](https://live.lge.co.kr/2403-ai-agent-q9/)
- [The bell — LG 로봇사업 점검](https://www.thebell.co.kr/free/content/ArticleView.asp?key=202503251554382040103261)
- [디지털데일리 — 로봇청소기 2025 H1](https://m.ddaily.co.kr/page/view/2025102015385605157)

### 해외 — 의료/간병/돌봄 제품·뉴스

- [CNN — Nurabot Foxconn NVIDIA](https://www.cnn.com/2025/09/12/tech/taiwan-nursing-robots-nurabot-foxconn-nvidia-hnk-spc)
- [The Robot Report — Diligent 300k pharmacy](https://www.therobotreport.com/diligent-robotics-completes-300000-pharmacy-deliveries-with-moxi/)
- [The Robot Report — Moxi 2.0](https://www.therobotreport.com/diligent-robotics-moxi-2-0-mobile-manipulator-built-for-ai/)
- [Intuitive Surgical — Q4 FY 2025](https://isrg.intuitive.com/news-releases/news-release-details/intuitive-announces-preliminary-fourth-quarter-and-full-year-5)
- [Medtronic — Hugo FDA urologic](https://news.medtronic.com/2025-12-03-Medtronic-announces-FDA-clearance-of-Hugo-TM-robotic-assisted-surgery-system-for-urologic-surgical-procedures)
- [Stryker — Mako RPS handheld](https://www.stryker.com/us/en/about/news/2026/stryker-introduces-mako-handheld-robotics-mako-rps.html)
- [TechCrunch — Ballie 2025 launch](https://techcrunch.com/2025/01/06/samsung-says-its-home-robot-ballie-will-roll-out-this-year/)
- [TechCrunch — 1X NEO Gamma test](https://techcrunch.com/2025/03/21/1x-will-test-humanoid-robots-in-a-few-hundred-homes-in-2025/)
- [Business Wire — 1X NEO launch](https://www.businesswire.com/news/home/20251027434628/en/1X-Launches-NEO-The-Robot-Redefining-Life-at-Home)

### VLA / Foundation Models — 핵심 논문

- [PI π0.5 arXiv 2504.16054](https://arxiv.org/abs/2504.16054)
- [Gemini Robotics 1.5 — arXiv 2510.03342](https://arxiv.org/abs/2510.03342)
- [GR00T N1 — arXiv 2503.14734](https://arxiv.org/abs/2503.14734)
- [VLA Survey — arXiv 2505.04769](https://arxiv.org/html/2505.04769v1)
- [EmbodiedBench — arXiv 2502.09560](https://arxiv.org/html/2502.09560v1)
- [Real-is-Sim — arXiv 2504.03597](https://arxiv.org/html/2504.03597v1)
- [Reality Gap Survey — arXiv 2510.20808](https://arxiv.org/abs/2510.20808)

---

## 부록. 사용 시 주의

- 시장 규모는 리서치펌별 편차 2배 이상 — IFR 공식 지표가 가장 신뢰도 높음.
- VLA·FM 일부(π0.5, GR00T N1, Helix 등)는 **연구·오픈소스 시연** 단계이며 실 운용 KPI 미공개. "이미 상용화됨"으로 오기재 금지.
- Ballie는 2024 이후 3회 출시 지연, 2025 미출시. "예고 시점"과 "실제 출시"를 구분.
- 의료로봇(A-4)은 Healthcare 도메인과 중첩. 본 문서는 **로봇 개체의 인지·의사결정·행동** 관점.
