# AI Robotics 도메인 사전 조사 자료 (3개 영역)

> 기준일: 2026-04-18 | "최근 1년" = 2025-04 ~ 2026-04
> 본 문서는 팩트/출처 중심이며, 아이디어·의견은 포함하지 않습니다.

---

## A. 의료/수술/재활 로봇

### 1. 시장/도입 현황

- **세계 수술로봇 시장**: 2025년 약 **USD 11.33B**, 2035년 **USD 38.27B** 전망 (CAGR 12.95%, SNS Insider 2026-04-13). 별도 집계로 2025년 **USD 13.69B → 2030년 USD 27.14B** (MarketsandMarkets).
- **정형외과 수술로봇**: 2025년 **USD 7.87B → 2035년 USD 26.17B** (Market Research Future).
- **세계 의료로봇(소프트+하드) 시장**: 2029년 약 **45조 원** 전망 (바이오타임즈, GM Insights 인용).
- **한국 로봇보조 수술시스템 시장**: 2024년 **USD 81.35M → 2035년 USD 644M** (Spherical Insights, CAGR 20.69%).
- **국내 로봇수술 건수**: 2005년 17건 → 현재 연 **약 1만 건** (Forbes Korea).
- **da Vinci 설치 기반**: 2025-12-31 기준 **11,106대** (YoY +12%); 2025년 시술 **약 315.3만 건** (YoY +18%) — Intuitive Surgical 2025 연간 예비 실적(2026-01-22).
- **호스피털 로지스틱스/약제 로봇**: 2025년 **USD 5.44B → 2033년 USD 14.77B** (DataM Intelligence, CAGR 13.3%).
- **웨어러블 외골격 시장**: 2025년 **USD 24.9억 → 2034년 USD 642.3억** (CAGR 43.7%, Global Growth Insights).

### 2. 주요 플레이어 (표)

| 구분 | 기업 | 대표 제품/영역 | 최근 팩트 |
|---|---|---|---|
| 해외 | Intuitive Surgical (美) | da Vinci 5 | 2025 4Q 532대 선적, da Vinci 5 303대, 유럽 CE mark 2025-07 |
| 해외 | Medtronic (美/아일랜드) | Hugo RAS | 2025-12-03 FDA 비뇨기 수술 clearance, 30개국 판매 |
| 해외 | Stryker (美) | Mako SmartRobotics / Mako RPS | 전 세계 3,000대+ 설치, 2026-02-09 Mako RPS 한정 출시 (2025-08 FDA 510(k)) |
| 해외 | Diligent Robotics (美) | Moxi (병원 물류) | 25개+ 미국 병원, 100만+ 배송, 약국 배송 30만건, Moxi 2.0 2026 상반기 출고 |
| 해외 | Aethon (美) | TUG | 500개+ 병원 설치 |
| 국내 | 큐렉소 | 큐비스-조인트(인공관절), 큐비스-스파인(척추), 모닝워크(재활) | 2025 매출 **745억원** (YoY +34%), 영업이익 흑자전환; 2026 FDA 최종 승인 목표 |
| 국내 | 고영테크놀러지 | 지니언트 크래니얼(뇌수술) | 미국 FDA·일본 PMDA 인허가 획득 |
| 국내 | 엔젤로보틱스 | 엔젤렉스 M20, 엔젤슈트 H10 | 2025 상반기 H10 출시, 말레이시아 국립대병원 공식 출시 |
| 국내 | 코스모로보틱스 | 엑소아틀레트 EA | 2025 IPO 진행 |
| 국내 | 로엔서지컬 | 자메닉스(신장결석) | 2025 첫 병원 공급 |
| 국내 | 엘엔로보틱스 | 심혈관중재 로봇 | 식약처 제조인증, 보건신기술인증 |

### 3. 최근 1년 기술 트렌드 (2025–2026)

- **VLA(Vision-Language-Action) 의료 적용**: RoboNurse-VLA 등, 수술 보조·약제 분배·환자 모니터링에 대한 VLA 임상시험이 2026년 진입 예상 (arXiv 2505.04769).
- **힘 피드백/햅틱**: da Vinci 5가 **FDA 승인 최초의 integrated force feedback haptic** 기능 탑재 (2024-03 발표, 2025 확산).
- **핸드헬드 로봇**: Stryker Mako RPS로 정형외과 로봇이 **console → handheld**로 확장 (2026-02).
- **휴머노이드 간호 로봇**: Foxconn/NVIDIA **Nurabot**, 대만 병원 2025-04 테스트 → 2026 초 상용화, 간호 업무량 20–30% 절감.
- **원격수술(Telesurgery)**: 정형외과 원격수술 타당성 리뷰 다수 (Springer J. Robotic Surgery, 2025).
- **병원 물류 파트너십**: Swisslog × Diligent(2025-10), Cedars-Sinai TUG 확장(2024-07).

### 4. 공공연한 문제/한계

- **햅틱/tactile 결핍**: 현행 RAS는 임상 통합된 palpation/haptic이 부재 → 인지부하·훈련시간·조직 손상 위험 (IEEE Pulse, MDPI Sensors 2026).
- **자율수술 수준 낮음**: FDA 승인 자율수술 로봇 대부분 **Level 1**, Level 2는 4개, Level 3은 3개뿐 (PMC11956393).
- **국내 '겹규제'**: 식약처 허가(3–6개월) + 혁신의료기술심사(3–6개월)로 큐렉소 척추로봇 2022 허가→2027 완료 전망 (한국경제 2025-11-20).
- **보험수가 부재**: 건강보험 수가가 행위 중심이라 디지털기기·로봇 반영 곤란; 보행재활로봇은 뇌졸중 선별급여만 적용 (약사공론).
- **시장 독점**: Intuitive Surgical **60%+ 글로벌 점유**, 국내는 "미국 대형사가 점령한 시장" (Forbes Korea).

### 5. 현장 페인포인트 (2~4개)

1. **간호 인력난·단순업무 과부하** — WHO, 2030년 **의료인력 1,000만명 부족** 예측. Moxi 같은 약제·검체·린넨 배송 단순업무를 대체 (automate.org, CNN 2025-09-12).
2. **햅틱 부재로 인한 tissue injury 리스크** — 수술로봇 조작 시 촉각 정보 없음 (MDPI Sensors 2026).
3. **국내 수술로봇 상용화 지연** — 5년 심사 누적으로 기술 개발해도 출시 불가 (한국경제 2025-11-20).
4. **재활로봇 접근성** — 수가 미비로 환자 자비 부담, 복지부 재활의료기관 지정제 안에서만 제한적 보급 (보건복지부).

### 6. 기존 서비스/제품 맵핑 (표)

| 제품 | 기업 | 용도 | 현황 |
|---|---|---|---|
| da Vinci 5 | Intuitive Surgical | 복강경 수술 | 2025 풀런칭, 힘 피드백 |
| Hugo RAS | Medtronic | 비뇨/부인/일반외과 | 2025-12 FDA 비뇨기 clearance |
| Mako RPS | Stryker | 무릎 정형외과 (핸드헬드) | 2026-02 한정 출시 |
| Moxi 2.0 | Diligent | 병원 약제/물품 배송 | 2026 상반기 출고 |
| TUG | Aethon | 병원 자율 AMR | 500+ 병원 |
| 큐비스-조인트 | 큐렉소 | 인공관절 | 식약처 허가, 인도/동남아 수출 |
| 지니언트 크래니얼 | 고영테크 | 뇌수술 | FDA·PMDA 승인 |
| 엔젤슈트 H10 | 엔젤로보틱스 | 산업용 웨어러블 | 2025 상반기 출시 |
| Nurabot | Foxconn | 간호 보조 | 2026 상용화 |

### 7. 기술적 공백

- **지능형(Level 2+) 자율수술**을 안전하게 검증·허가 받는 파이프라인 부족.
- **소형·멸균 가능·고정밀 촉각 센서** (PMC 2701448, MDPI 26/4/1126).
- **의료 전용 VLA**를 위한 **병원 운영 데이터셋** (수술 영상+지시+기구 동작 결합) 공개 부재.
- **보행재활 홈케어** — 병원 밖 외골격 원격 모니터링/수가 모델 부재.
- **국내 인허가 심사 간소화와 실세계 증거(RWE) 연계** 제도 공백.

---

## B. 서비스/접객 로봇

### 1. 시장/도입 현황

- **IFR World Robotics 2025 (서비스로봇)**: 전문용 서비스로봇 2024년 **약 20만대** 판매 (YoY +9%); RaaS 대여모델 **+31%** (IFR 2025-10-07).
- **Hospitality(접객) 로봇**: 2024년 **42,000대+ 판매**로 2위, 단 YoY **–11%** (IFR).
- **커머셜 서비스 로보틱스 시장**: 2025 **USD 8.09B → 2034 USD 30.89B** (CAGR 21.3%, IntelMarket Research). 2025년 **호스피털리티가 42%** 차지.
- **중국 벤더 점유율**: 2024년 전 세계 커머셜 서비스로봇 출하의 **약 85%**가 중국 (People's Daily, 2025-12-08).

### 2. 주요 플레이어 (표)

| 구분 | 기업 | 대표 제품 | 최근 팩트 |
|---|---|---|---|
| 해외 | Pudu Robotics (中) | KettyBot Pro, BellaBot | 80개국+ 판매, KettyBot Pro 출시 |
| 해외 | Keenon (中) | DINERBOT, Butler | 60개국+, Embodied AI 확장 |
| 해외 | SoftBank Robotics (日/佛) | Pepper 계열 | 글로벌 상위 3사 |
| 국내 | 베어로보틱스 (본사 美, 코리아법인) | Servi, Servi Plus, Servi Mini | 20개국+ **2만대+** 공급; 2025-05 LG전자 지분 30%+ 추가 인수로 **LG 계열사 편입** |
| 국내 | LG전자 | CLOi ServeBot, GuideBot | 조선호텔앤리조트 협력, 인국공 NDA 체결, CES 2026 CLOiD 공개 |
| 국내 | KT | KT 서빙로봇 | 통신사 기반 대여 모델 |
| 국내 | 로보티즈 | 일개미(실외 배송), 집개미(실내 배송) | 로봇팔 탑재 실내 배송 |
| 국내 | 현대위아 | H-motion (물류) | CES 2026 첫 공개, 2028년 **4,000억원** 매출 목표 |

### 3. 최근 1년 기술 트렌드 (2025–2026)

- **LG전자의 서비스로봇 사업 본격화**: 2025-05 베어로보틱스 경영권 확보; 조선호텔앤리조트·인천국제공항공사와 협력 (LG Newsroom 2025-01, 2025-02).
- **생성형 AI 접목 대화형 가이드**: CLOi에 LLM 기반 대화 기능 탑재 확산 (innno.co.kr 2026-04).
- **조리 로봇과 연계**: Miso Robotics Flippy(치킨 튀김), Chipotle Hyphen Makeline(보울 350개/시간), Sodexo ART 파트너십 등으로 서빙-조리 연결 가속 (Fortune 2026-02-26).
- **RaaS 확산**: 구독형 로봇 렌탈 +31% 성장 (IFR 2025).
- **휴머노이드/모바일 매니퓰레이터**: 현대위아 H-motion, 로보티즈 집개미(로봇팔 장착).

### 4. 공공연한 문제/한계

- **Hospitality 로봇 2024년 판매량 감소(-11%)** — 단순 서빙의 ROI 포화 (IFR 2025).
- **국내 식당 체감 효용 낮음**: 바쁜 피크타임에 사람 감지 시 정지, 테이블번호 입력 오히려 지연 (뉴시스, 그린포스트코리아).
- **물리적 제약**: 문턱·경사로·다층 구조·엘리베이터 탑승 난제 (나무위키, 사이드뷰).
- **배터리 화재 사례**: 서울 노원구 서빙로봇 충전 중 화재 (500만원 피해) — 안전 이슈 부각.
- **중국산 덤핑 구조**: 글로벌 85% 중국 벤더 점유로 국내 제조사 가격 경쟁 압박.

### 5. 현장 페인포인트 (2~4개)

1. **피크타임 병목** — 좁은 통로에서 정지·회피로 사람 서빙보다 느려짐 (뉴시스).
2. **건물 인프라 제약** — 다층 식당/호텔에서 엘리베이터 연동·문턱 통과 실패.
3. **주문→탑재→테이블번호 입력 수작업** 자체가 새로운 노동 (그린포스트코리아).
4. **배터리/안전** — 충전 중 화재, 리튬 배터리 교체·관리 부담.

### 6. 기존 서비스/제품 맵핑 (표)

| 제품 | 기업 | 유형 | 용도 |
|---|---|---|---|
| Servi / Servi Plus / Servi Mini | 베어로보틱스 | 서빙/버싱 | 식당, 호텔 |
| CLOi ServeBot | LG전자 | 서빙 (트레이형) | 호텔/식당 |
| KettyBot Pro | Pudu | 서빙+접객(AD 디스플레이) | 식당 |
| BellaBot | Pudu | 서빙 | 식당 |
| DINERBOT T8/T10 | Keenon | 서빙 | 식당 |
| 집개미 | 로보티즈 | 실내 배송 (로봇팔) | 호텔·고층빌딩 |
| 일개미 | 로보티즈 | 실외 배송 | 도심·아파트 |
| H-motion (AMR/코봇/Stretch) | 현대위아 | 물류 | 창고·B2B |
| Flippy | Miso Robotics | 조리 | QSR(치킨/감자) |

### 7. 기술적 공백

- **엘리베이터·문·보안게이트** API 표준 부재 (멀티 벤더 연동).
- **피크타임 군집 내비게이션** — 사람 밀집 시 사회적 내비게이션(SAN) 부족.
- **VLA 기반 주문 이해·자연 대화 결합**한 일체형 서빙 에이전트 미성숙.
- **주방-홀 엔드투엔드 자동화** (주문→조리→픽업→서빙→버싱→세척) 통합 플랫폼 공백.
- **안전 표준**: 서빙로봇의 배터리·충전·화재 안전 KC/KS 별도 인증 체계 부재.

---

## C. 농업 로봇

### 1. 시장/도입 현황

- **세계 자율주행 트랙터 시장**: 2025 **USD 8.37B → 2035 USD 68.88B** (CAGR 23.46%, Roots Analysis).
- **세계 자율주행 트랙터(Mordor Intelligence 기준)**: 2025년 **약 1.7조 원 → 2029년 5.5조 원** (Bloter 인용).
- **세계 과일수확 로봇**: 2025년 **USD 247M** (Coherent Market Insights).
- **딸기 수확 로봇**: 2026년 **USD 123.1M → 2033년 USD 191.4M** (Verified Market Reports).
- **DJI 농업드론**: 2024년 말 기준 100여 개국 **약 40만 대** 운용, 2020년 대비 +90%+ (디지털투데이).
- **국내 보급(농촌진흥청)**: 2024년 운반로봇 10대, 2025년 운반로봇 13대+방제로봇 10대, **수확로봇은 2026 중 보급 예정** (정책브리핑/전자신문 2025-10-09).
- **국내 생산성 실증**: 자율트랙터·이식로봇·드론 조합으로 **작업시간 18%~80% 단축**, 사과·복숭아 농장 **생산성 13–15%↑** (AgTech Navigator 2025-11-19).

### 2. 주요 플레이어 (표)

| 구분 | 기업 | 대표 제품 | 최근 팩트 |
|---|---|---|---|
| 해외 | John Deere (美) | Autonomous 9RX, 2nd-gen Autonomy Kit | CES 2025 공개, 16-camera 360° 어레이, 2026 풀릴리즈 |
| 해외 | CNH Industrial / New Holland | R4 Autonomous Robot (전동·하이브리드) | Agritechnica 2025 공개, **2027 상반기 한정생산**, CO2 최대 100% 감축 |
| 해외 | Lely (네덜란드) | Astronaut A5 Next, Astronaut Max, Lely Hub | 2025-08 공개, **2026 페이즈드 롤아웃**, 누적 **50,000대+** |
| 해외 | Octinion (벨기에) | Rubion Gen2 (딸기) | **95% 정확도**, 손상률 <0.8%, 첫해 3,800대 |
| 해외 | Harvest CROO Robotics (美) | 딸기 수확 | 2025-04 필드트라이얼 상용화 수준 달성 |
| 해외 | DailyRobotics | 딸기 수확 로봇 | 2026 캘리포니아 상용화 예정 |
| 해외 | DJI Agriculture (中) | Agras T40/T50 | 글로벌 40만대+ |
| 해외 | XAG (中) | 농업드론 | 글로벌 경쟁사 |
| 국내 | 대동 (Daedong) | HX·AI 트랙터, 운반로봇, 콤바인 | 업계 최초 자율 4단계 온디바이스 AI 트랙터 공개, **2026 상용화 목표**; 농진청 신기술 농업기계 인증 |
| 국내 | TYM | 자율 3단계 대형 트랙터 | 2025-05부터 국내외 판매 |
| 국내 | LS엠트론 | 트랙터 | (기존 3사 중 하나) |
| 국내 | 에스피아그리 | 스마트팜 딸기 수확 | 야간 8시간 무인 수확, **인건비 40–50% 절감** |

### 3. 최근 1년 기술 트렌드 (2025–2026)

- **온디바이스 AI 트랙터**: 대동 2025-11 공개, 클라우드 의존 없이 기기에서 경로·장애물·작업 제어 실시간 수행 (헤럴드경제 2026-04-09).
- **멀티작업 통합 플랫폼**: New Holland **R4** — 제초·경운·방제를 한 플랫폼에서, 한 명이 원격으로 최대 **5대** 조작.
- **농업로봇 통합관리 프로그램**: 농촌진흥청, 방제·운반·모니터링 로봇 통합 SW (2025-10 시연, 월화수목금토마토농장).
- **Green-on-Green 타겟 방제**: 제초제 최대 **80% 절감**(CNH, 2027 북미 런칭).
- **딸기 소프트터치**: Octinion Rubion Gen2가 **사람 수준 bruising률 매칭**.
- **축산 자동화 확장**: Lely Astronaut Max로 **500–1,100두 대규모 농장** 지원.

### 4. 공공연한 문제/한계

- **가격·투자 회수**: John Deere 8R 자율트랙터 **USD 50–60만**, 리트로핏킷 USD 5–7만 — 소규모 농가 접근성 낮음 (Farmonaut).
- **한국 농촌 고령화·소규모 필지**: 농촌 인력난+필지 소형화로 대형 자율기계 도입 난이도.
- **수확 로봇 상용화 지연**: 부드러운 과실(딸기·토마토) 손상·인식 정확도·속도 문제 — 국내 수확 로봇 보급은 2026부터 시작.
- **계절근로자 제도 엇박자**: 외국인 계절근로 확대(8→10개월, 2026–2030 기본계획) 병행 필요 (축산신문, 법무부).
- **작물별 특화** — 한 플랫폼이 여러 작물에 적용되기 어려움 (R4는 특화작물용).

### 5. 현장 페인포인트 (2~4개)

1. **농촌 고령화·인력난** — 국내 농가 고령화로 농약 살포·수확 노동력 부족 (농진청, 굿모닝경제).
2. **방제 시 농약 피폭** — 드론/로봇 방제로 농업인 직접 노출 회피 필요 (농진청).
3. **수확기 노동 집중** — 딸기·토마토 같은 고부가 작물에서 수확 시간 집중이 병목, 에스피아그리는 야간 무인 수확으로 대응.
4. **대자본 집중·소농 배제** — 고가 자율기계는 대농 중심, 소농을 위한 공동이용/RaaS 모델 필요.

### 6. 기존 서비스/제품 맵핑 (표)

| 제품 | 기업 | 용도 | 현황 |
|---|---|---|---|
| Autonomous 9RX | John Deere | 대형 경운 자율트랙터 | 2026 풀릴리즈 |
| R4 Electric/Hybrid | New Holland | 과수원·포도밭 멀티작업 | 2027 한정 생산 |
| Astronaut A5 Next/Max | Lely | 착유 로봇 | 2026 페이즈드 롤아웃 |
| Rubion Gen2 | Octinion | 딸기 수확 | 상용 배치 중 |
| Agras T40/T50 | DJI | 방제/파종 드론 | 글로벌 40만대 |
| 대동 AI 트랙터 | Daedong | 자율 4단계 | 2026 상용화 목표 |
| TYM 자율 트랙터 | TYM | 자율 3단계 | 2025-05 판매 |
| 스마트팜 딸기 수확 | 에스피아그리 | 시설 딸기 | 야간 8시간 무인 |
| 농진청 통합 관리 | RDA | 방제·운반·모니터링 통합 | 2025-10 시연 |

### 7. 기술적 공백

- **부드러운 과실의 범용 파지** — 품종·형태 다양성을 커버하는 범용 gripper와 VLA 기반 인식.
- **노지(오픈필드) 작물용** 저가형 수확 로봇 — 현재 고부가 시설작물 중심.
- **한국형 소필지·다품종**에 맞는 경량·저가 자율 플랫폼 (John Deere·New Holland는 대필지 타깃).
- **축산 분야 스마트 헬스케어 로봇** — 착유 외 질병 조기진단·행동모니터링 로봇 부재.
- **농업 RaaS/공동이용 플랫폼** — 소농 대상 구독형 로봇 운용 모델 미성숙.
- **농약 살포 드론 안전·무인비행 규제** — 국내 야간 방제·장거리 자율비행 규제 공백.

---

## 통합 출처 목록

### A. 의료/수술/재활 로봇

1. SNS Insider, "Surgical Robots Market Size", 2026-04-13 — https://orthospinenews.com/2026/04/13/surgical-robots-market-size-is-projected-to-attain-usd-38-27-billion-by-2035-sns-insider/
2. Intuitive Surgical, "Preliminary Q4 & FY 2025 Results", 2026-01-13 — https://isrg.intuitive.com/news-releases/news-release-details/intuitive-announces-preliminary-fourth-quarter-and-full-year-5
3. Intuitive Surgical 2024 Annual Report — https://isrg.intuitive.com/static-files/500ff989-ad91-4b32-a59e-f94a34d75997
4. Medtronic, "FDA clearance of Hugo™ for urologic procedures", 2025-12-03 — https://news.medtronic.com/2025-12-03-Medtronic-announces-FDA-clearance-of-Hugo-TM-robotic-assisted-surgery-system-for-urologic-surgical-procedures
5. Stryker, "Mako Handheld Robotics with Mako RPS", 2026-02-09 — https://www.stryker.com/us/en/about/news/2026/stryker-introduces-mako-handheld-robotics-mako-rps.html
6. The Robot Report, "Diligent Robotics 300,000 pharmacy deliveries" — https://www.therobotreport.com/diligent-robotics-completes-300000-pharmacy-deliveries-with-moxi/
7. The Robot Report, "Moxi 2.0 mobile manipulator" — https://www.therobotreport.com/diligent-robotics-moxi-2-0-mobile-manipulator-built-for-ai/
8. 로봇신문, "큐렉소, 2025년 매출 745억원…역대 최대 실적", 2026-02 — https://www.irobotnews.com/news/articleView.html?idxno=44779
9. 한국경제, "세계 최초 기술 개발하면 뭐하나…심사 기간만 10년", 2025-11-20 — https://www.hankyung.com/article/2025112063341
10. 이투데이, "고영테크, 지니언트 크래니얼 日 PMDA" — https://www.etoday.co.kr/news/view/2547329
11. 헤럴드경제, "엔젤로보틱스 IPO 인터뷰" — https://biz.heraldcorp.com/article/3336124
12. Forbes Korea, "美 대형사가 잠식한 시장, 국내 수술 로봇의 돌파구" — https://www.forbeskorea.co.kr/news/articleView.html?idxno=400499
13. CNN Business, "AI nursing robots Nurabot Foxconn NVIDIA", 2025-09-12 — https://www.cnn.com/2025/09/12/tech/taiwan-nursing-robots-nurabot-foxconn-nvidia-hnk-spc
14. IEEE Pulse, "Robotic Surgery With Haptic Feedback" — https://www.embs.org/pulse/articles/feel-the-precision-next-gen-robotic-surgery-with-haptic-feedback/
15. PMC, "Autonomous surgery challenges" (PMC11956393) — https://pmc.ncbi.nlm.nih.gov/articles/PMC11956393/
16. arXiv 2505.04769, "Vision-Language-Action Models: Concepts, Progress, Applications and Challenges" — https://arxiv.org/html/2505.04769v1
17. 청년의사, "삼성서울병원 SMC 병동로봇" — http://www.docdocdoc.co.kr/news/articleView.html?idxno=3006451
18. 세브란스 뉴스, "지능형 의료서비스로봇 도입" — https://sev.severance.healthcare/news/press/report.do?mode=view&articleNo=116661
19. DataM Intelligence, "Hospital Robotics (Logistics & Pharmacy) Market 2026–2033" — https://www.datamintelligence.com/research-report/hospital-robotics-logistics-and-pharmacy-market
20. Global Growth Insights, "Soft Exoskeleton (Exosuits) and Wearable Robots Market" — https://www.globalgrowthinsights.com/market-reports/soft-exoskeleton-exosuits-and-wearable-robots-market-100266

### B. 서비스/접객 로봇

1. IFR, "World Robotics 2025 – Service Robots", 2025-10-07 — https://ifr.org/ifr-press-releases/news/service-robots-see-global-growth-boom
2. IFR, "World Robotics 2025 Statistics, Sources & Methods" — https://ifr.org/img/worldrobotics/Sources___Methods_WR_2025_Service_Robots.pdf
3. IntelMarket Research, "Commercial Service Robotics 2026-2034" — https://www.intelmarketresearch.com/global-commercial-service-robotics-forecast-market-26549
4. People's Daily, "Chinese-made robotics show strength on world stage", 2025-12-08 — https://en.people.cn/n3/2025/1208/c90000-20399637.html
5. LG Newsroom, "LG전자, 베어로보틱스 경영권 확보", 2025-01 — https://live.lge.co.kr/2501-lg-bear-robotics/
6. LG전자, "LG 클로이 서브봇 제품 페이지" — https://www.lge.co.kr/service-robot/ldlim21
7. LG, "홈로봇 CLOiD CES 2026 공개 예고" — https://www.lg.co.kr/media/release/29723
8. 헤럴드경제, "현대위아, 2028년 무인 물류로 매출 4000억원 목표 [CES 2026]" — https://biz.heraldcorp.com/article/10651129
9. 서울경제, "현대위아 CES 첫 참가, H-모션 공개" — https://www.sedaily.com/NewsView/2K773V8PRL
10. 현대닷컴, "CES 2026 AI 로보틱스" — https://www.hyundai.com/kr/ko/brand/brandstory/campaigns/ces-2026-robotics-exhibition
11. 로보티즈 실내 배송로봇 '집개미' — https://www.robotis.com/sub/business_zip.php
12. 로보티즈 실외 자율주행로봇 — https://www.robotis.com/sub/business_012.php
13. 뉴시스, "바쁜 피크타임엔 못써요 서빙로봇 현장", 2023-02 — https://www.newsis.com/view/NISX20230220_0002198993
14. 그린포스트코리아, "국내 외식업계, 서빙로봇 도입에만 급급" — http://www.greenpostkorea.co.kr/news/articleView.html?idxno=114074
15. 나무위키, "서빙로봇 (배터리 화재 사례 포함)" — https://namu.wiki/w/서빙로봇
16. Fortune, "$28 billion race to disrupt fast food", 2026-02-26 — https://fortune.com/2026/02/26/robot-disruption-fast-food-short-order-cook-flippy-labor-shortage/
17. Pudu Robotics KettyBot — https://www.pudurobotics.com/ads/kettybot/en
18. The Robot Report, "Pudu CEO predicts service robot market" — https://www.therobotreport.com/pudu-ceo-predicts-service-robot-market-to-expand/

### C. 농업 로봇

1. John Deere, "New Autonomous Machines at CES 2025" — https://www.deere.com/en/news/all-news/autonomous-9RX/
2. PRNewswire, "John Deere CES 2025" — https://www.prnewswire.com/news-releases/john-deere-reveals-new-autonomous-machines--technology-at-ces-2025-302342436.html
3. CNH Industrial, "2025 Tech Day: AI, Autonomy, Robotics", 2025-11-11 — https://www.globenewswire.com/news-release/2025/11/11/3185279/0/en/CNH-2025-Tech-Day-showcasing-customer-centric-farming-innovations-across-AI-Autonomy-Robotics-and-Automation.html
4. New Holland, "Autonomous R4 Robot Series" — https://agriculture.newholland.com/en-gb/europe/new-holland-world/news/2025/new-holland-autonomous-r4-robot-series
5. Lely, "Three new robotic systems for milking", 2025-08-05 — https://roboticsandautomationnews.com/2025/08/05/lely-launches-three-new-robots-for-milking-cows/93499/
6. Roots Analysis, "Autonomous Tractor Market 2035" — https://www.rootsanalysis.com/autonomous-tractor-market
7. 전자신문, "토마토밭 누비는 로봇…스마트팜", 2025-10-09 — https://www.etnews.com/20251009000070
8. 농촌진흥청, "로봇과 AI로 토마토 수확시기 예측" — https://www.rda.go.kr/board/board.do?boardId=farmprmninfo&prgId=day_farmprmninfoEntry&dataNo=100000771411
9. 정책브리핑, "이젠 로봇도 체계적으로…농업로봇 확산" — https://www.korea.kr/news/policyNewsView.do?newsId=156685775
10. 헤럴드경제, "운전대서 손 뗀 트랙터, 대동 AI 농업로봇", 2026-04-09 — https://biz.heraldcorp.com/article/10713353
11. Bloter, "농슬라 대동·TYM, 자율주행 농기계로 재도약" — https://www.bloter.net/news/articleView.html?idxno=623705
12. AgTech Navigator, "South Korea autonomous machinery ageing farm population", 2025-11-19 — https://www.agtechnavigator.com/Article/2025/11/19/south-korea-turns-to-autonomous-machinery-as-ageing-farm-population-deepens-labour-shortage/
13. 이투데이, "에스피아그리, AI 로봇 사계절 딸기 수확" — https://www.etoday.co.kr/news/view/2515342
14. AgFunder News, "DailyRobotics strawberry harvester 2026 commercial launch" — https://agfundernews.com/dailyrobotics-gears-up-for-commercial-launch-in-california-in-2026-with-robotic-strawberry-harvester
15. Octinion Rubion — http://octinion.com/products/agricultural-robotics/rubion
16. 디지털투데이, "글로벌 농업 드론 40만대 시대…DJI" — https://www.digitaltoday.co.kr/news/articleView.html?idxno=564963
17. DJI, "농업 연례 보고서 2025" — https://www.dji.com/kr/newsroom/news/dji-agricultural-annual-report-2025
18. Expert Market Research, "South Korea Agriculture Drone Market" — https://www.expertmarketresearch.com/reports/south-korea-agriculture-drone-market
19. 축산신문, "외국인 계절근로자 제도 엇박자" — https://www.chuksannews.co.kr/news/article.html?no=270412
20. Coherent Market Insights, "Fruit Picking Robots Market 2026-2033" — https://www.coherentmarketinsights.com/market-insight/fruit-picking-robots-market-4531
