# AI Robotics 도메인 리서치

> **기준일**: 2026-04-18 | **"최근 1년"** = 2025-04 ~ 2026-04
> 본 문서는 팀 프로젝트의 **아이디어 후보 선정 직전 단계** 팩트 자료이며, 제안/의견 없이 출처 중심으로 작성되었습니다. 서비스·기술·수치는 모두 발행일·발행처·링크와 함께 기록되어 있습니다.

## 목차

- [Part 1. 하위 영역 지도 (What / 플레이어 / 최근 트렌드)](#part-1-하위-영역-지도)
  - [(A) 응용 도메인 9개](#a-응용-도메인)
  - [(B) 개발 플랫폼/인프라 5개](#b-개발-플랫폼인프라)
- [Part 2. 영역별 페인포인트 & 기존 서비스 (Pain)](#part-2-영역별-페인포인트--기존-서비스)
- [Part 3. 주목 기술 트렌드 (Trend, Cross-cutting)](#part-3-주목-기술-트렌드-cross-cutting)
- [Part 4. 통합 출처 목록](#part-4-통합-출처-목록)
- [부록. 조사 한계 & 주의사항](#부록-조사-한계--주의사항)

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
| 로지스틱스 로봇 2025 판매 | **450,000대+** (2019 대비 +500%) | Cyzerg 2025 |
| Amazon 로봇 보유 | **100만 대+** (2025-07) | Automate.org |
| 한국 정부 정책 | 제4차 지능형로봇 기본계획: 2030년까지 3조원, 100만대 보급 | 산업부 |
| K-휴머노이드 연합 | 2025-04-10 출범, 1조원+ 투자, 2028 상용(60kg 이하·20kg 페이로드·50 DoF·2.5m/s) | 정책브리핑 |

---

## Part 1. 하위 영역 지도

> **하위 영역 구조**: (A) 응용 도메인 9개 + (B) 개발 플랫폼/인프라 5개 = **총 14 영역**
>
> (B)는 로봇 AI를 "만드는 개발자를 돕는 SaaS·툴 레이어"입니다. 한국 기획자들이 자주 놓치는 영역이지만 2024–2026 스타트업 투자가 활발한 기회 공간이므로 비중 있게 다룹니다.

### (A) 응용 도메인

#### A-1. 산업용/협동 로봇 (Cobots)

- **What**: 조립·용접·피킹 등 사람 곁에서 동작하는 협동로봇. 2024년 64,500대 설치(+12% YoY), 자동차 산업이 최대 수요(45%). 글로벌 시장 2025 **US$ 3.06B~4.18B**(보고서 편차), 2035년 US$ 85.93B(Precedence Research). 국내 시장 약 3.6억 달러(인더스트리뉴스 2025).
- **국내/해외 온도차**: 해외 UR/FANUC/ABB가 AI-cobot 공격 출시. 국내 두산·한화·레인보우·HD현대로보틱스는 중국 저가 공세로 재무 부진 → 두산로보틱스 **2026 흑자전환 목표**.
- **주요 플레이어**: 국내 — 두산로보틱스(CES 2026 Scan & Go, NVIDIA Physical AI 협업), HD현대로보틱스(AI 제어기 Hi7, 2025-10), 레인보우로보틱스(삼성 계열사), 한화로보틱스. 해외 — Universal Robots(UR20/UR30 25~35kg), FANUC, ABB, KUKA, Yaskawa, Physical Intelligence(π0/π0.5).
- **최근 1년 트렌드**:
  - **VLA 파운데이션 모델 상용화 초입** — π0/π0.5(PI), NVIDIA **GR00T N1**(2025-03, 합성 780k trajectory), Gemini Robotics, OpenVLA(7B), SmolVLA(450M).
  - **ISO 10218-2:2025 + ISO/TS 15066 통합**: cobot을 "로봇 응용"으로 재정의.
  - **AI 비전 bin picking 성숙**: Inbolt 온-암 AI(2025-12, pick <1s + 95% 성공).
  - 한국: 이동식 협동로봇 산업표준(KSB ISO 10218-2), 대구 규제자유특구, 2025 AI 규제합리화 로드맵.
  - RaaS(Rapid Robotics, Vention)으로 SMB 진입장벽 완화.

#### A-2. 물류/창고 로봇 (AMR, 자동 피킹)

- **What**: AMR(Autonomous Mobile Robot), 자동 분류·피킹 시스템, 창고 자동화. 글로벌 AMR 2026 **US$ 2.75B~6.18B**(M&M/BRI 편차), 2032 US$ 7.07B CAGR 14.4%. **AI 피킹로봇**은 2024 $2.3B → 2034 $240B(10배↑, 로봇신문/IDC).
- **대형 레퍼런스**: Amazon **100만 대+**(2025-07 돌파), DHL **Stretch 1,000+대 MOU**(2025-05), Geek+ **세계 최초 AMR 상장**(2025).
- **국내**: 쿠팡 대구 FC(아시아 최대) THiRAbot·소팅봇 — 자동화 인력 330(2024-01) → 750(2025-10). **CJ대한통운** 군포 FC 국내 최초 AI 휴머노이드 실증, Icheon 허브 **5G 프라이빗망 + 500대 로봇 sub-10ms**.
- **주요 플레이어**: 국내 — 쿠팡, CJ대한통운, 티엑스알로보틱스, 씨메스(3D 비전+AI 피킹). 해외 — Amazon Robotics(Sequoia +75%, Proteus, Sparrow, Digit 테스트), Boston Dynamics Stretch(700 case/hr), Locus Robotics(DHL 누적 **5억 건** 피킹), GreyOrange(Series D $135M + Google Cloud DeepNav 2025-08), Agility Robotics Digit.
- **최근 1년 트렌드**:
  - 휴머노이드의 창고 진입(Digit-Amazon, CJ 휴머노이드).
  - 오케스트레이션 + Gen AI: **GreyMatter DeepNav**(Google Gemini 기반, 2025-08).
  - 대규모 VLA/FM 접목(CJ + Physical AI, NVIDIA Isaac GR00T 기반 RFM).
  - 5G 프라이빗 네트워크 상용 시작.
  - DHL 1,000+ Stretch MOU(2025-05), Otto Group 20+ 시설.

#### A-3. 배달/라스트마일 로봇

- **What**: 자율배송봇, 배송 드론, 실내/실외 라스트마일. 글로벌 2025 **US$ 0.80B**(M&M), 2026 자율 라스트마일 **US$ 1.6B**(Fortune BI), 2030 US$ 3.24B CAGR 32.4%. 국내 2021 $2.71M → 2026 **$14.65M**(연 40%, 세계 최고 성장률, KISTI).
- **Starship 누적**: 900만 건, 1,900만 km, 2,700대, 270 사이트, 7개국. 2027 12,000대 목표.
- **주요 플레이어**: 국내 — **뉴빌리티**(2025-12 Series B 251억, 누적 550억원, 재주문율 80%, 142 사이트, 젠슨 황 언급), 우아한형제들 **딜리**(실내 월 90만원 렌탈, 2년), 로보티즈(실외 '개미'). 해외 — Starship, Serve Robotics(Uber Eats 2,000대 + DoorDash 다년, $80M 2025-01), Nuro($6B 가치, Uber·Lucid 2031 20,000 robotaxi), **Coco Robotics**($80M Series B 2025-06 누적 $120M+), Kiwibot(30+ 미국 대학).
- **최근 1년 트렌드**:
  - 대형 플랫폼-로봇 제휴 본격화(Uber/DoorDash/Starship).
  - 자금 유입: Coco $80M, Starship $50M, Serve $80M, 뉴빌리티 251억.
  - 전천후 주행(Waymo all-weather 2025-10, Avride 눈길).
  - 한국 규제 완화: 2023 지능형로봇법 개정(500kg·15km/h 이하 보도 허용 + 의무보험). 2025 로드맵 심사항목 16→8개, 기간 60→30일.
  - 순찰·보안 겸업(뉴빌리티 북미·사우디).

#### A-4. 의료/수술/재활 로봇

- **What**: 수술보조 로봇, 재활 외골격, 병원 물류·간호 보조. 세계 수술로봇 **2025 US$ 11.33B → 2035 US$ 38.27B** CAGR 12.95%(SNS Insider 2026-04-13) / 2025 US$ 13.69B → 2030 US$ 27.14B(MarketsandMarkets). 세계 의료로봇 2029년 약 **45조원**(GM Insights). **da Vinci** 설치 11,106대(2025-12-31, YoY +12%), 2025년 시술 315만 건(+18%). 한국 로봇 수술 **연 약 1만 건**.
- **주요 플레이어**: 해외 — Intuitive Surgical(da Vinci 5, 2025-07 CE, 2025 4Q 532대 선적), Medtronic(Hugo RAS, 2025-12-03 FDA 비뇨기), Stryker(Mako RPS 2026-02 핸드헬드), Diligent Robotics(Moxi 30만+ 약제 배송, Moxi 2.0 2026 상반기), Aethon TUG(500+ 병원). 국내 — **큐렉소**(2025 매출 **745억원** +34%, 2026 FDA 목표), 고영테크(지니언트 FDA·PMDA), 엔젤로보틱스(엔젤슈트 H10 2025 출시), 로엔서지컬(자메닉스), 엘엔로보틱스.
- **최근 1년 트렌드**:
  - **VLA 의료 적용**: RoboNurse-VLA, 2026 임상 진입 예상.
  - da Vinci 5가 FDA 승인 최초 integrated force feedback haptic(2024-03 → 2025 확산).
  - **Mako RPS로 console → handheld** 전환(2026-02).
  - **Foxconn/NVIDIA Nurabot** — 대만 병원 2025-04 테스트 → 2026 초 상용, 간호 업무 20–30% 절감.
  - 원격수술 타당성 리뷰 다수(Springer 2025).
  - 병원 물류 파트너십(Swisslog×Diligent 2025-10).

#### A-5. 서비스/접객 로봇

- **What**: 호텔·식당·공항·매장 안내·서빙 로봇. 2024 전문용 서비스로봇 20만대+(+9%), Hospitality 42,000대+(YoY −11%) — **수요 포화 신호**. 커머셜 서비스로봇 2025 US$ 8.09B → 2034 US$ 30.89B CAGR 21.3%(IntelMarket). 글로벌 85% 중국 벤더(People's Daily 2025-12-08).
- **주요 플레이어**: 해외 — Pudu Robotics(KettyBot Pro, 80국+), Keenon(60국+), SoftBank Robotics(Pepper). 국내 — **베어로보틱스**(Servi 20국+ 2만대+, **2025-05 LG 계열사 편입**), LG전자(CLOi, 조선호텔·인국공, CES 2026 CLOiD), KT, 로보티즈(일개미/집개미), **현대위아 H-motion**(CES 2026 첫 공개, 2028년 4,000억원 매출 목표).
- **최근 1년 트렌드**:
  - **LG전자 서비스로봇 본격화**(베어로보틱스 경영권 2025-05, 조선호텔·인국공).
  - 생성형 AI 접목 대화형 가이드(CLOi LLM 탑재).
  - 조리 로봇 연계(Miso Flippy, Chipotle Hyphen Makeline 350 bowl/hr, Sodexo ART, Fortune 2026-02-26).
  - RaaS +31% 성장(IFR 2025).
  - 휴머노이드/모바일 매니퓰레이터(현대위아 H-motion, 로보티즈 집개미 로봇팔).

#### A-6. 농업 로봇

- **What**: 수확, 방제, 축산, 스마트팜 로봇. 세계 자율주행 트랙터 2025 **US$ 8.37B → 2035 US$ 68.88B** CAGR 23.46%(Roots Analysis). 세계 과일수확 로봇 2025 US$ 247M(Coherent). DJI 농업드론 **글로벌 40만대+** 운용(2024말 기준, 100국+).
- **한국**: 농진청 2024 운반로봇 10대 → 2025 13대+방제로봇 10대. **수확로봇 2026 보급 예정**. 자율트랙터·이식로봇·드론 조합으로 **작업시간 18~80% 단축**, 사과·복숭아 생산성 13~15%↑(AgTech Navigator 2025-11).
- **주요 플레이어**: 해외 — John Deere(Autonomous 9RX CES 2025, 16-camera 360°), CNH New Holland(**R4** Agritechnica 2025, 2027 한정생산, 1인당 원격 5대), Lely(Astronaut A5 Next/Max 2025-08, 누적 50,000대+), Octinion(Rubion Gen2 딸기, 95% 정확도 손상률 <0.8%), DJI Agras T40/T50. 국내 — **대동**(자율 4단계 온디바이스 AI 트랙터, 2026 상용화 목표), TYM(자율 3단계 2025-05 판매), LS엠트론, 에스피아그리(딸기 야간 무인, 인건비 40–50%↓).
- **최근 1년 트렌드**:
  - **온디바이스 AI 트랙터**(대동 2025-11, 헤럴드 2026-04-09).
  - 멀티작업 통합 플랫폼(R4 제초·경운·방제).
  - 농진청 통합관리 SW(2025-10 시연).
  - Green-on-Green 타겟 방제(CNH, 제초제 −80%, 2027 북미).
  - Lely Astronaut Max로 500–1,100두 대규모 농장 지원.

#### A-7. 가정/케어 로봇

- **What**: 청소 로봇, 노인돌봄/실버, 컴패니언/펫 로봇. 로봇청소기 2025 **약 320억 달러** CAGR 27.6%(Research Nester). 국내 상반기 **Roborock 46%**(1위), 삼성 22%(+6%p), 에코백스 14%→4% 급락. 초고령사회 — **2025 65세+ 1,084만 명**(20%+), 2072년 47.7%(서울신문 2026-01-04). AI 돌봄 '다솜' 누적 2만명, 대화 8,555만 건.
- **주요 플레이어**: 로봇청소기 — Roborock(中), 삼성 Bespoke AI, LG, Ecovacs(中). 돌봄 — 효돌(MS Azure), 원더풀플랫폼 다솜. 컴패니언 — Sony Aibo($3,000+), CASIO Moflin($400), KEYi Loona(ChatGPT-4o). **홈 AI** — 삼성 Ballie(Gemini, 2026 타깃, 3회 지연), LG Q9(MS Azure OpenAI, 2025 말). 웨어러블 — 삼성 봇핏 EX1.
- **최근 1년 트렌드**:
  - 생성형 AI/LLM 내장화(Ballie=Gemini, Q9=Azure OpenAI+Bing).
  - LG Q9 2025-03 베타 → 2025 말 정식, Q9 SDK 선공개.
  - **Ballie 출시 3회 지연**, 2025 미출시 → 2026 타깃.
  - 돌봄 로봇 다모달 관찰(다솜 카메라로 먼저 말 걸기).

#### A-8. 건설/위험작업 로봇

- **What**: 철거·점검·시설 유지보수·재난 대응·극한환경 로봇. 글로벌 건설로봇 2025 **약 14.6억 달러** CAGR 15.3%. 외벽 청소 로봇 2025 10.4억 달러 → 2033 150.9억 달러 CAGR 39.7%(GGI). 한국 건설 사망 2024 276명, 2025 Q3 210명(+3.4%) — OECD 최상위 10개국 평균의 **2배**, 영국의 **6.6배**(Korea Times 2025-11-27).
- **주요 플레이어**: 해외 — **Boston Dynamics Spot**(Sellafield 핵시설·후쿠시마 배치, 현대 자회사), **Atlas 전기식**(2026 Hyundai Georgia RMAC 투입), ANYbotics ANYmal(Onkalo 핵폐기장), Hilti Jaibot(천장 드릴링), Dusty FieldPrinter(현장 레이아웃), Rosatom Spider(원자로 용접 검사 2025-10), MHI A-UT(원자로 초음파). 국내 — CSCAM EDELSTRO(외벽 청소), RP 로보프린트(외벽 도장·청소), K-휴머노이드 연합 조선·가전·건설 현장 실증 로드맵.
- **최근 1년 트렌드**:
  - AI 기반 자율 점검 상용(Spot 핵시설 방사선 매핑).
  - **Rosatom Spider 원자로 용접 검사**(ANS Newswire 2025-10-28).
  - 3D 프린팅·벽돌쌓기 +24%, 철거 로봇 31% 점유(BRI 2025).
  - 외벽 청소 로봇 AI — 사람 대비 3배 고속.
  - K-휴머노이드 연합 조선 실증 로드맵.

#### A-9. 휴머노이드/범용 로봇

- **What**: 범용 이족 휴머노이드. 시장 2025 **48.9억 → 2026 62.4억**, CAGR 35-45%. Morgan Stanley 2050년 **5조 달러**, Goldman 2035 380억. **2025 중국 출하 90%** 점유, 리더 Unitree(~5,500), AgiBot(5,168), UBTech(~1,000). AgiBot 누적 **1만대 돌파**(2026-03, 5k→10k 3개월로 가속).
- **주요 플레이어**:
  - **Figure AI** — Figure 03(168cm 60kg 44DoF, <$20k 타깃, 2025-10 공개, 2026 말 파트너 가정 배치).
  - **1X** — NEO(30kg, $20,000 또는 월 $499, 2026 美 배송).
  - **Tesla Optimus V3** — 173cm 57kg, Tesla AI5 + Grok, 2026 여름 생산, 2027 양산 수만 대.
  - **Agility Digit** — GXO Flowery Branch **10만+ 토트 이동**(2025-11), Mercado Libre·Amazon 파일럿.
  - **Boston Dynamics Atlas 전기식** — CES 2026 상용 공개, Hyundai Georgia/Google DeepMind 2026 배치, **HMGMA 2028 30,000대/년**.
  - **NVIDIA GR00T N1** — 2025-03-18 GTC 오픈 VLA.
  - **Unitree** G1($16k~$73.9k) / H1($90-150k), 2026-03 상해 $610M IPO 신청, 2025 매출 ¥17.08억(+335%).
  - **UBTech** Walker S, 2026 생산 1만대.
  - **XPeng IRON** — 22 DoF 핸드, 인공근육·피부, 2026 말 대량생산 목표.
  - **AgiBot** — 2025 세계 1위 5,168대, 2026-03 1만대.
  - 한국 — **레인보우로보틱스 RB-Y1**(삼성 35% 자회사, 시총 13조, 2025 170-200대, 2026 확대), **에이로봇 앨리스 M1**(시리즈A 100억, NVIDIA CES 2026 기조, MWC 2026 LGU+), 현대차그룹(Atlas+Spot Georgia, 美 $26B 4년 투자).
- **최근 1년 트렌드**:
  - NVIDIA **GR00T N1**(2025-03) 오픈 VLA + GR00T-Dreams(합성 데이터 780k).
  - **Figure Helix**(2025-02, 풀상체 200Hz 온보드 GPU).
  - **Physical Intelligence π0.5/π0.6**(2025-04/11) — 처음 보는 가정에서 10-15분 청소 + RL 자기개선.
  - Google **Gemini Robotics 1.0/1.5/ER 1.6**(2025-03/09, 저지연 온디바이스).
  - HF **SmolVLA**(2025-06, 450M로 π0 급).
  - Figure 03 — 3g 촉각, 무선 유도충전 2kW, 16시간 배터리.
  - 1X NEO 'Expert Mode'(인간 원격조작으로 데이터 재학습).
  - 상용 마일스톤: Digit GXO 10만 토트, AgiBot 1만대, Optimus 1,000+ 테슬라 공장.
  - 한국: 레인보우로보틱스 삼성 자회사 편입, 에이로봇 NVIDIA 기조.

### (B) 개발 플랫폼/인프라

#### B-1. 시뮬레이션/가상환경

- **What**: 로봇 AI 학습·평가용 시뮬레이터. 글로벌 로보틱 시뮬레이터 시장 2025 **US$ 820M → 2035 US$ 3.09B** CAGR 14.20%(Precedence). 전체 로보틱스 스타트업 펀딩 2025 **~US$ 14B**(2024 $8.2B에서 급증).
- **주요 플레이어/제품**:
  - **NVIDIA Isaac Sim 5.0 / Isaac Lab 2.2** — SIGGRAPH 2025 GA, Neural reconstruction, OmniSensor USD schema.
  - **MuJoCo 3 / MJX / Playground** — Google DeepMind, MJX TPU v5 **2.7M steps/s**, Playground 2025-02.
  - **Newton** — NVIDIA + DeepMind + Disney Research 공동, GTC 2025, 2025-09-29 Linux Foundation 이관. NVIDIA Warp 기반, **differentiable physics**. RL 워크로드 **70x+** 가속.
  - **Genesis** — 20+ 연구실 컨소시엄, 2024-12 오픈소스, RTX 4090 단일 GPU에서 43M FPS 주장(제한조건; 재현 시 과장 논란).
  - **Gazebo** — Classic 2025-01 EOL, gz-sim으로 이주.
  - **ManiSkill3** — Hillbot/UCSD, RSS 2025, 30,000+ FPS, VLA 호환.
  - **Antioch** — 스타트업, 완전 SW-only 테스트(pre-seed).
- **투자 하이라이트**:
  - **Skild AI** Series C **US$ 1.4B**, 밸류 **US$ 14B+**(2026-01-14, SoftBank·NVentures·Bezos Expeditions). 7개월 만에 $4.5B → $14B로 3배.
  - **Physical Intelligence** US$ 600M, 밸류 **US$ 5.6B**(CapitalG).
  - **Flexion** Series A US$ 50M(2025-11, DST Global).
- **최근 1년 트렌드**:
  - GPU 병렬 시뮬레이터 표준화(Isaac Lab 4,096env 82-94K FPS).
  - Differentiable/Unified 물리 엔진(Newton).
  - **WFM을 시뮬 대체재로**: GR00T-Dreams로 GR00T N1.5 학습 **3개월 → 36시간**.
  - SIGGRAPH 2025 Isaac Sim 5.0 + Lab 2.2 GA.

#### B-2. 합성 데이터/디지털 트윈

- **What**: 3D 씬·도메인 랜덤화·Sim2Real 파이프라인. 합성 데이터 시장 2025 ~US$ 2B → 2033 ~US$ 10B CAGR ~25%. 다른 추정 $410M(2024) → $4.71B(2032) CAGR **35.8%**(SkyQuestt).
- **주요 플레이어**:
  - **NVIDIA Cosmos + GR00T-Dreams** — 2025-01 CES 출시, Predict-2.5 업데이트. Uber CES 2025 최초 도입 선언.
  - **Bifrost AI**(싱가폴) — 2024-10 Series A US$ 8M, 누적 $13.7M.
  - Parallel Domain, SKY ENGINE AI, Sightwise, Lightwheel(Isaac Lab 정책 평가 공동개발), Generalist AI, **1X World Model**(1XWM, NEO 정책 통합).
- **디지털 트윈 도입**:
  - **BMW** Omniverse FactoryExplorer → 생산계획 비용 **30% 절감** 전망.
  - **Foxconn** FODT 휴스턴 242,287 ft² AI 인프라 팩토리, Cadence 열시뮬 **150x** 가속.
  - Omniverse 누적 300,000+ 다운로드, 252+ 엔터프라이즈 배포.
- **최근 1년 트렌드**:
  - **WFM 기반 합성 데이터**(Cosmos, 1XWM, Humanoid World Models arXiv 2506.01182).
  - **Gaussian Splatting 학습 자산화** — InteriorGS(1,000 실내 씬 554K 오브젝트), EmbodiedSplat(ICCV 2025), arXiv 2512.13411.
  - **Real-to-Sim 자산 생성** — Scalable Real2Sim(CVPR 2025 Real2Sim Workshop 신설).
  - 도메인 랜덤화 재평가(2025 RAL — quadrotor에서 DR이 SysID 대비 suboptimal).
  - OpenUSD/OmniSensor 확산.

#### B-3. 로봇 파운데이션 모델 / 정책 학습

- **What**: 시연 데이터로 학습된 범용 VLA 정책. 2024~2025년 오픈/상용 VLA 대량 공개, "dual-system(S1 빠른 행동 + S2 느린 추론)" 아키텍처가 주류화. 상용화는 여전히 **연구 데모 + 제한 파일럿** 단계.
- **주요 플레이어/모델**:
  - **NVIDIA**: GR00T N1/N1.5/N1.6 + Cosmos + Isaac Lab (Apache 2.0)
  - **Google DeepMind**: RT-1/2, RT-X, ALOHA 2/Unleashed, **Gemini Robotics 1.0/1.5/ER 1.5/1.6**, Genie 2/3
  - **Physical Intelligence**: π0, π0.5, π0.6, π*0.6(RECAP), FAST tokenizer, openpi(Apache 2.0)
  - **Figure AI**: Helix(35-DoF·200Hz 온디바이스, 폐쇄)
  - **Hugging Face**: LeRobot, SmolVLA(450M, MacBook 구동)
  - **Skild AI**: Skild Brain ("omni-bodied"), $14B 밸류
  - **TRI**: Large Behavior Model(Atlas 공동)
  - **Stanford/UCB**: OpenVLA(7B Apache 2.0), Octo, RDT-1B(THU)
  - **AgiBot + OpenDriveLab**: AgiBot World Colosseo(1M+ trajectory)
  - **네이버랩스 유럽**: Navigation Foundation Model, 3D FM
- **2025 주요 릴리스 연표**:
  - 01 Cosmos / FAST / Figure Helix(02)
  - 03 GR00T N1(GTC), Gemini Robotics 1.0(117 저자), OpenVLA 업데이트
  - 04 π0.5 (open-world generalization)
  - 05 GR00T N1.5 + GR00T-Dreams (Cosmos 기반)
  - 06 SmolVLA(450M), RoboArena
  - 08 TRI LBM + Atlas
  - 09 Gemini Robotics 1.5 + ER 1.5 (15개 embodied reasoning 벤치 SOTA)
  - 10 Cosmos Predict 2.5 / Transfer 2.5
  - 11 π0.6 / π*0.6 RECAP (RL 자기 시연)
  - 12 Skild AI $14B 밸류
  - CoRL 2025 GR00T N1.6(32-layer DiT)

#### B-4. 데이터 수집·원격조작 (Teleop)

- **What**: 시연 데이터 수집 리그, VR 텔레옵, 대규모 데이터셋.
- **표준화 진행**:
  - **Stanford ALOHA**(~$20k) → Mobile ALOHA($32k, 2024) → **ALOHA 2**(DeepMind 2024-05) → ALOHA Unleashed(2024-09, 26k 시연).
  - **UMI**(Stanford, RSS 2024) — GoPro 핸드헬드 그리퍼로 in-the-wild 수집.
  - **SO-ARM100/101**(HF+RobotStudio) — 6-DoF 3D 프린팅 **$220~$240**. LeRobot 즉시 학습.
- **데이터셋 스케일**:
  - **Open X-Embodiment**(21기관, 1M+ trajectory, 22 embodiments, 527 skills)
  - **DROID**(13기관, 76k trajectory, 350h, 564 scene, 86 task)
  - **AgiBot World Colosseo**(1M+ trajectory, 2,976h, 217 task, IROS 2025 Best Paper Finalist)
  - **LeRobot 커뮤니티**(487 datasets, 10M frames)
  - **Humanoid Everyday**(USC 2025-10, 260 task, RGB+depth+LiDAR+tactile+IMU)
- **산업 서비스**:
  - micro1, Sensei(YC), Lumos FastUMI Pro(10,000대 2026 배포 계획).
  - 텔레옵 단가 **$340/h → $136/h**(2024초 → 2025 4Q).
  - **1X NEO** 2025-10 공식 출시($20k), human-in-the-loop 원격조작으로 대규모 가정 데이터 수집 전략.

#### B-5. 평가/벤치마크

- **What**: 로봇 정책 평가 환경/리더보드. 2024–2025 CoRL/RSS/ICLR 공감대: "robot policy evaluation is a persistent, unscalable challenge". NVIDIA + Lightwheel 오픈소스 평가 프레임워크 공동개발(2025).
- **주요 벤치마크**:
  - **RoboArena**(7기관, arXiv 2506.18123, 2025-06; NVIDIA Research 2025-09, 600+ pairwise)
  - **RobotArena ∞**(arXiv 2510.23571)
  - **RoboChallenge**(arXiv 2510.17950)
  - **PolaRiS**(arXiv 2512.16881)
  - **REALM**(arXiv 2512.19562)
  - **AutoEval**(arXiv 2503.24278)
  - **SimplerEnv**(UCSD, CoRL 2024, 25 tasks)
  - **ManiSkill3**(12 도메인 30K FPS VLA 평가, RSS 2025)
  - **LIBERO / LIBERO-PRO / LIBERO-Plus**(2023 / 2025-10 확장)
  - **HumanoidBench**(UCB, 27 whole-body)
  - **VLABench**(ICCV 2025)
  - **DROID / Open X-Embodiment / LeRobotDataset v3**
- **최근 1년 트렌드**:
  - 분산·크라우드소스 평가 전환.
  - Real2Sim 평가 주류화(RobotArena ∞, PolaRiS, REALM, Real-is-Sim).
  - **VLA robustness crisis**: LIBERO-Plus — 최신 VLA가 perturbation 하에 **95%→30% 이하 붕괴**, 언어 지시 사실상 무시 현상(arXiv 2510.13626).
  - LeRobotDataset v3 표준 멀티모달 시계열 포맷.
  - π0/π0-FAST/π0.5 오픈소스화(2025-02/09).

---

## Part 2. 영역별 페인포인트 & 기존 서비스

### A-1. 산업용/협동 로봇

**현장 페인포인트**
1. 프로그래밍·재설정 부담 — 다품종 소량 생산 때마다 티칭 재작업 (Standard Bots, Ebots 2025).
2. 안전영역 전략 부재 — 일괄 저속화로 생산성 하락 (기계신문 2025-07).
3. Bin picking 실패 — 겹침·반사·포즈 추정 오류 (ScienceDirect 2025).
4. SMB 자본 부담 — 셀 전체 $50k–$150k+, ROI 12–18개월.
5. (한국) 중국 저가 유입, 규제 해석 혼란.

**기존 서비스/제품**

| 제품 | 기능 | AI 적용 | 알려진 한계 |
|---|---|---|---|
| UR20/UR30 + AI Accelerator | 25–35kg, PolyScope X | NVIDIA Isaac 통합 | AI Accelerator 별도 옵션, 앱 생태계 초기 |
| 두산 Scan & Go | cobot+AMR 통합, 도면 없이 작업 | Physical AI(VLA), 3D 비전 | 상용 초기, 레퍼런스 부족 |
| HD Hi7 | 산업 로봇 AI 제어기 | 위험 예측 | 협동용보다 산업용 |
| PI π0.5 | 모바일 매니퓰레이터 범용 | VLA, 이종 데이터 공동학습 | 실환경 일반화 초기 |
| GR00T N1 | 휴머노이드 FM | 멀티모달 VLA | HW 보급 전 |
| Inbolt 온-암 | 랜덤빈 피킹 | 온-암 AI 비전 | 신규, 장기 레퍼런스 부족 |

**기술적 공백**
- 실시간 안전영역 어댑티브 세이프티(작업자 위치/자세 기반 동적 토크/속도 조정).
- 자연어 재티칭 — 한두 번 시연/말로 새 공정 학습(VLA 성과는 있으나 공장 배포 X).
- SME용 제로샷 비전 피킹.
- 국내 cobot 제조사 자체 FM 부재.

### A-2. 물류/창고 로봇

**현장 페인포인트**
1. 피킹 정확도 vs 다품종 — 99.5%+ 달성하나 이형·변형·손상 SKU 급락 (TGW 2025).
2. 성수기 인력 충원 불가능성 — MHI 2025 45~52% "매우 어렵다".
3. 로봇 간 트래픽 / AMR-사람 협착.
4. SW 통합 복잡도(WMS-로봇 OS-AMR, CJ 5G 프라이빗망 구축 사례).

**기존 서비스/제품**

| 제품 | 기능 | AI 적용 | 한계 |
|---|---|---|---|
| Amazon Sequoia | 컨테이너 피킹 통합, Proteus AMR | 비전·모션플래닝 | 품목 형상 제약 |
| Amazon Digit(Agility) | 이족, 토트 재활용 | locomotion+manip | 속도·적재 제한, 파일럿 |
| BD Stretch | 컨테이너/트럭 언로딩 700 case/hr | 비전+딥러닝 파지 | 케이스박스 위주, 이형 화물 취약 |
| Locus Robotics AMR | 피킹 어시스트 | 경로·주문 AI | 사람이 파지 |
| GreyMatter DeepNav | 동적 오케스트레이션 | Google Gemini LLM | 신규, 레퍼런스 초기 |
| Geek+ | Goods-to-person AMR | 경로 AI | 고정 선반 의존 |
| 쿠팡 THiRAbot+소팅봇 | 반송·분류 | 비전·스케줄 | 내부 전용 |
| CJ 휴머노이드 PoC | 포장·분류 | RFM + Gen AI | 초기 PoC |

**기술적 공백**
- 완전 이형·깨지기 쉬운 SKU 제로샷 피킹.
- 로봇+사람 혼재 실시간 동선 예측.
- 휴머노이드 FC 운영 KPI(pick/hr, 가동률) 공개 부재.
- 국내 중견·중소 3PL용 RaaS 모델 확산 미흡.

### A-3. 배달/라스트마일 로봇

**현장 페인포인트**
1. 보행자·접근성 약자 충돌/차단 — Chicago·West Hollywood 민원 폭증(2025).
2. 계단·경사·엘리베이터 — 실내외 경계 통과 실패.
3. 도난·장난 — 로봇 카메라·적재물 훼손.
4. 운영비 대비 건당 수익성 — 15km/h·소형 페이로드, 기상 중단 고려 시 난이도.

**기존 서비스/제품**

| 제품 | 기능 | AI 적용 | 한계 |
|---|---|---|---|
| Starship | 보도 자율 1.5~2km | 비전·LiDAR 자율주행 | 소형, 폭설 중단 |
| Serve Gen3 | 보도 자율 4시간+ | Jetson 컴퓨터 비전 | mobility scooter 충돌 |
| Nuro R3 | 운전대 없는 공공도로 물류 | end-to-end 자율 | B2C → 라이선싱 피벗 |
| Coco | 보도 하이브리드(원격+자율) | 비전 + 텔레옵 | 버스 쉘터 충돌 |
| 뉴빌리티 뉴비 | 실외 배송·순찰 겸업 | 저가 카메라 SLAM | 15km/h 보도법, 엘리베이터 |
| 우아한 딜리 | 실내 서빙 | 실내 SLAM | 테이블번호 수동 |
| Kiwibot | 대학 캠퍼스 | 비전·LiDAR | 학내 한정 |

**기술적 공백**
- 실내↔실외 연속 배송(공동현관·엘리베이터 자동 연동).
- 이형 지형(눈·연석) 안정 주행.
- 보행자 의도 예측 + 접근성 인지 특화 모델.
- 소량·초소형(의약품·문서) 도심 배송.
- 한국 실외 B2C 단가 모델(딜리 월 90만원 외 불투명).

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

### A-6. 농업 로봇

**현장 페인포인트**
1. 농촌 고령화·인력난(농진청, 굿모닝경제).
2. 방제 시 농약 피폭 회피.
3. 수확기 노동 집중(딸기·토마토 병목).
4. 대자본 집중·소농 배제(소규모 농가용 공동이용 필요).

**기존 서비스/제품**

| 제품 | 기업 | 용도 | 현황 |
|---|---|---|---|
| Autonomous 9RX | John Deere | 대형 경운 | 2026 풀릴리즈 |
| R4 Electric/Hybrid | New Holland | 과수원·포도 | 2027 한정 생산 |
| Astronaut A5 Next/Max | Lely | 착유 | 2026 페이즈드 롤아웃 |
| Rubion Gen2 | Octinion | 딸기 수확 | 상용 배치 |
| Agras T40/T50 | DJI | 방제 드론 | 글로벌 40만대 |
| 대동 AI 트랙터 | Daedong | 자율 4단계 | 2026 상용 목표 |
| TYM 자율 트랙터 | TYM | 자율 3단계 | 2025-05 판매 |
| 에스피아그리 | 에스피아그리 | 시설 딸기 야간 무인 | 판매 |
| 농진청 통합 관리 | RDA | 방제·운반·모니터링 | 2025-10 시연 |

**기술적 공백**
- 부드러운 과실의 범용 파지(VLA 기반).
- 노지(오픈필드) 저가형 수확 로봇.
- 한국형 소필지·다품종 경량 자율 플랫폼.
- 축산 스마트 헬스케어(질병 조기진단).
- 농업 RaaS/공동이용 플랫폼.
- 야간 방제·장거리 자율비행 규제.

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

### A-8. 건설/위험작업 로봇

**현장 페인포인트**
1. 소규모 현장 추락·감전 사망 — 2025 Q3 10.4%↑, 안전관리자 부재(Korea Times 2025-11).
2. 고층 외벽 청소·도장 위험(곤돌라 100% 수작업, 마천루 3개월).
3. 핵시설·재난 인간 접근 불가(후쿠시마·Sellafield).
4. 노후 인프라 점검 누락(교량·터널).

**기존 서비스/제품**

| 제품 | 영역 | 상태 |
|---|---|---|
| Boston Dynamics Spot | 시설 점검 | 상용(핵시설·건설) |
| ANYbotics ANYmal | 발전·화학 점검 | 상용(Onkalo) |
| Hilti Jaibot | 천장 드릴링 | 상용 |
| Dusty FieldPrinter | 현장 레이아웃 | 상용 |
| Built Robotics RoboDozer | 불도저 자율화 | 파일럿·상용 |
| Canvas(Drywall) | 내벽 마감 | 상용 |
| Vega Robot | 핵 해체 정찰 | 연구→실증 |
| CSCAM EDELSTRO | 외벽 청소 | 한국 상용 |
| RP 외벽 로봇 | 도장·청소 | 한국 상용 |
| Rosatom Spider | 원자로 용접검사 | 2025 배치 |

**기술적 공백**
- 소규모 현장용 저가(1억 이하) 안전관찰 로봇.
- 고소·외벽 작업 완전 자율화(바람·전선·난간).
- 비정형 폐기물(철거) 분류·선별 자동화.
- 재난 현장 이종(휴머노이드+드론+4족) 군집 제어.

### A-9. 휴머노이드/범용 로봇

**현장 페인포인트**
1. 로지스틱스 3D 업무 인력난(GXO·Mercado·Amazon Digit 도입).
2. 자동차 공장 반복/위험 공정(Hyundai HMGMA Atlas 2028).
3. 가정 일상 노동(Figure 03 수건개기·식기세척기·빨래·테이블정리).
4. 돌봄/재활 시설 인력난(Fourier GR-3 CES 2026).

**기존 서비스/제품**

| 세그먼트 | 대표 제품 | 실사용 상태 |
|---|---|---|
| 물류/창고 | Agility Digit | GXO 상시, 10만+ 토트 |
| 완성차 공장 | BD Atlas | Hyundai Georgia 실증, 2028 양산 |
| 완성차 공장 | Tesla Optimus | 테슬라 공장 내부, 외부 2026 말 |
| 홈 | Figure 03 | 파트너 가정 2026 |
| 홈 | 1X NEO | 2026 美 배송 |
| 연구/교육 | Unitree G1 | $16k~ 판매 |
| 산업/연구 | Unitree H1 | $90-150k |
| 돌봄 | Fourier GR-3 | CES 2026 공개 |
| 조선·제조 | 에이로봇 Alice M1 | 파일럿 |
| 한국 이족 | Rainbow RB-Y1 | 2025 시제품, 2026 확대 |
| FM | NVIDIA GR00T N1 / Gemini Robotics / π0 / Helix | 오픈/상용 |

**기술적 공백**
- Long-horizon 과업 신뢰도(오류 누적, 자가 복구).
- 범용 dexterous 손 조작(옷감·액체·가변 형상).
- 실시간 안전 보장(가정·공공장소 충돌·힘 제어 표준).
- 에너지 효율(16h 배터리는 상위권, 다수 2-4h).
- 온디바이스 VLA(Helix·Gemini On-Device 등장에도 다수 클라우드 의존).
- 한국 자체 FM 부재(GR00T·Helix·π0 전량 해외, K-휴머노이드 FM 2026 착수).

### B-1. 시뮬레이션

**개발자 페인포인트**
1. 환경 세팅/호환성 — Isaac Sim Linux+RTX 전제, 빌드 종속 강함.
2. 자산 포맷 변환(URDF·USD·MJCF 왕복).
3. 훈련 성능 튜닝 — GPU/CPU 병목 진단 어려움(Isaac Lab Issue #3043).
4. Sim2Real 검증 루프의 수동성(논문·릴리스마다 재현 불가, RoboArena 2506.18123).

**기존 툴**

| 계층 | 예시 | 비고 |
|---|---|---|
| 물리 엔진 | MuJoCo 3, PhysX 5, Newton(Warp), Genesis, Bullet, ODE | Newton이 GPU·differentiable 표준 시도 |
| 환경/런타임 | Isaac Sim 5.0, Gazebo(gz-sim), Webots, CoppeliaSim, SAPIEN | Isaac Sim은 Omniverse 결합 |
| RL 학습 | Isaac Lab 2.2, MuJoCo Playground, ManiSkill3, RoboSuite | GPU parallel env 표준 |
| 합성 데이터 | Replicator(Isaac), Cosmos+GR00T-Dreams, Bifrost, SKY ENGINE AI, Parallel Domain | WFM 기반 새 축 |
| MLOps | W&B(CoreWeave 인수 2025-05 $1.7B), MLflow, TensorBoard | 로보틱스 특화는 공백 |

**기술적 공백**
- 멀티 시뮬레이터 자산 포터빌리티 표준(OpenUSD도 물리 semantics 미포괄).
- RL GPU 활용도 실시간 자동튜닝.
- WFM vs 전통 물리 sim 공식 성능/정확도 벤치.
- Windows/macOS GPU parallel RL(Genesis 외 부재).

### B-2. 합성 데이터/디지털 트윈

**개발자 페인포인트**
1. 리얼리티 갭 정량화 불가 — "얼마나 리얼해야 충분한가" 지표 부재.
2. 파이프라인 통합 비용(스키마·포맷 정리 수작업).
3. 라벨 검증/품질 관리(자동 annotation 오라벨 필터 부족).
4. 하드웨어-디지털 트윈 동기화 툴체인 파편화.

**기존 툴**

| 분류 | 플레이어 | 특징 |
|---|---|---|
| 엔드투엔드 | NVIDIA Omniverse Replicator + Cosmos + OSMO | GR00T-Dreams/N1.5 공급 |
| 독립 SaaS | Bifrost AI, Parallel Domain, SKY ENGINE | 센서별 도메인 특화 |
| Gaussian Splatting | InteriorGS, EmbodiedSplat, Scalable Real2Sim | 씬 자동화 |
| 세계 모델 | Cosmos Predict, 1XWM, GAIA-2(Wayve) | video→action |
| 디지털 트윈 | BMW FactoryExplorer, Foxconn FODT | OpenUSD |

**기술적 공백**
- 합성 품질 → 실 로봇 성공률 자동 피드백 루프.
- 연성물·유체·가변 마찰 합성.
- Gaussian Splat 자산 물리 속성(질량·마찰·관성) 자동 부여.
- CAD/PLM ↔ USD 디지털 트윈 live sync 상용.

### B-3. 로봇 파운데이션 모델 / 정책 학습

**개발자/연구자 페인포인트**
1. 체크포인트 많지만 자기 로봇·태스크 파인튜닝 절차가 난해(액션 공간·카메라·주파수 상이, 래퍼 반복 노동).
2. 실제 로봇 없이 평가 불가(RoboArena 분산 시도 초기).
3. 데이터 수집이 여전히 인력 집약($340/h → $136/h로 하락).
4. GPU/메모리 요구(OpenVLA 7B, RDT 1.2B 온보드 어려움 → SmolVLA 450M 수요).

**기존 모델 맵핑**

| 모델 | 발표 | 공개 | 구조 | 성능/한계 |
|---|---|---|---|---|
| RT-2 | DeepMind 2023 | 비공개 | PaLI-X/PaLM-E VLA | 55B 폐쇄 |
| Octo | Berkeley, RSS 2024 | 오픈 | Transformer diffusion 800k OXE | 9 로봇 재현, 소규모 |
| OpenVLA | Stanford/UCB CoRL 2024 | 오픈(Apache 2.0) | Llama2 7B + DINOv2+SigLIP | RT-2-X 대비 +16.5%/7× 작음 |
| π0 | PI 2024-10 | 오픈(openpi) | VLM + flow matching 50Hz | 7 플랫폼 68 태스크 SOTA |
| RDT-1B | Tsinghua, ICLR 2025 | 오픈 | 1.2B diffusion transformer | 46 데이터셋, bimanual |
| π0.5 | PI 2025-04 | 일부 오픈 | 계층적(서브태스크+액션) | 미본 가정 청소 10-15분 |
| π0.6 / π*0.6 RECAP | PI 2025-11 | 모델 카드 | RL 자기 시연 | 세탁·에스프레소 장시간 |
| GR00T N1/N1.5/N1.6 | NVIDIA | 오픈(HF) | Dual system VLA | N1 13.1→N1.5 38.3% |
| Gemini Robotics 1.0/1.5 | DeepMind | 모델 API | Gemini 2.0/2.5 + 액션, thinking | 15 ER 벤치 SOTA |
| Helix | Figure AI 2025-02 | 비공개 | S1/S2 VLA 35-DoF 200Hz | 2 로봇 동시 제어 |
| SmolVLA | HF 2025-06 | 오픈 | 450M, 1,000만 프레임 | SO100 78.3% |
| LBM | TRI 2025 | 비공개 | 전신 단일 정책 | Atlas 시연 |
| Skild Brain | Skild AI 2025-07 | 비공개 | omni-bodied | 수치 비공개 |

**기술적 공백**
- 정책 모델 + 연속학습/RL 표준화.
- 액션 공간·제어 주파수 통일(Unified Action Space).
- VLA 실행 런타임(엣지 TensorRT/ONNX 표준).
- 벤치마크 합의(RoboArena, RoboChallenge, Isaac Lab-Arena, EmbodiedBench 난립).

### B-4. 데이터 수집·원격조작

**개발자/연구자 페인포인트**
1. 텔레옵 셋업 복잡도(Meta Quest/Vive + 리더-팔로워 + ROS 동기화 재구현).
2. 데이터 라벨링/정제(언어 주석·세그먼테이션·실패 demo 제거 수작업).
3. 재현 불가능한 하드웨어(ALOHA 부품 단종 이슈, SO-ARM101 3D 프린팅화가 대응).
4. 개인정보/홈 데이터(1X NEO 가정 데모, 얼굴·사적 공간 규정 모호).

**기존 툴/데이터셋**

| 도구/데이터셋 | 발표 | 공개 | 특징 |
|---|---|---|---|
| ALOHA | Stanford 2023 | 오픈 HW+code | 리더-팔로워 양손 $20k |
| Mobile ALOHA | Stanford 2024-01 | 오픈 | 전신+이동 $32k |
| ALOHA 2 | DeepMind 2024-05 | 오픈 | ALOHA 개선, MuJoCo 모델 |
| ALOHA Unleashed | DeepMind 2024-10 | 논문+일부 코드 | Transformer + diffusion, 26k demo |
| UMI | Stanford RSS 2024 | 오픈 | GoPro 핸드헬드 그리퍼 |
| DROID | 13기관 2024-03 | 오픈 | 76k·350h Franka |
| Open X-Embodiment | 21기관 2023-10 | 오픈 | 1M+·22 embodiments |
| AgiBot World | AgiBot+OpenDriveLab 2025-03 | 오픈 | 1M+·2,976h·217 task, IROS 2025 Best Paper Finalist |
| SO-ARM100/101 | RobotStudio+HF 2024-2025 | 오픈 3D 프린팅 | 6-DoF $220~$240 |
| Humanoid Everyday | USC 2025-10 | 오픈 | 260 task, 다모달 |
| Isaac Lab + GR00T-Dreams | NVIDIA 2025 | 오픈 | 시뮬+Quest+Cosmos 합성, GR00T N1.5 3개월→36h |
| LeRobot | HF 2024~ | 오픈 | end-to-end OSS |

**기술적 공백**
- UMI-style 포터블 + ALOHA 고정밀 통합 프레임워크.
- 실패 demo 자동 필터링(인간 demo 품질 스코어링).
- 프라이버시-세이프 홈 데이터 파이프라인(얼굴 마스킹·익명화).
- 멀티모달(촉각·힘·오디오) 표준 포맷.

### B-5. 평가/벤치마크

**개발자/연구자 페인포인트**
1. "누구 게 실제로 더 잘 하나?" 답 불가 — 논문별 커스텀 셋업.
2. VLA 평가 재현 실패 — 카메라 각도·조도·초기상태에 편차 극심.
3. 벤치마크 인프라 분산 — SimplerEnv·ManiSkill·LIBERO·Humanoid·CALVIN·RLBench 통합 리더보드 없음.
4. 실 로봇 평가 로지스틱스(DROID 없으면 RoboArena 참여 불가).

**기존 툴**

| 계층 | 대표 툴 | 비고 |
|---|---|---|
| 실 데이터셋 | Open X-Embodiment, DROID, LeRobot 컬렉션 | OXE 22 로봇, DROID 76K |
| Sim 벤치(manipulation) | SimplerEnv, ManiSkill3, RLBench, LIBERO(+PRO/Plus), CALVIN | 포맷·리더보드 분산 |
| Sim 벤치(humanoid) | HumanoidBench, Isaac Lab locomotion | MuJoCo/Isaac |
| Real-world | RoboArena, RoboChallenge, AutoEval | 하드웨어 의존 |
| Real-to-Sim | RobotArena ∞, PolaRiS, REALM, Real-is-Sim, SuReSim | 2025 하반기 집중 |
| MLOps(일반) | W&B, MLflow, Neptune | 로봇 전용 X |
| VLA 베이스라인 | π0/π0-FAST/π0.5, OpenVLA, RT-X, GR00T, Octo | 다수 오픈 |

**기술적 공백**
- 통합 리더보드/스탠다드 포맷(OXE+LeRobot+SimplerEnv 관통).
- VLA robustness testing-as-a-service(LIBERO-Plus 자동 perturbation).
- 실 로봇 rollout 분산 인프라 상용 API.
- W&B 급 로보틱스 전용 실험 추적/리더보드 SaaS.
- 평가→트레이닝 데이터 선택 폐루프(AutoEval 초기).

---

## Part 3. 주목 기술 트렌드 (Cross-cutting)

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

### 3-5. Imitation Learning

- **정의**: 전문가 시연으로부터 정책 학습(BC, DAgger, Inverse RL).
- **왜 지금**: 현 VLA 대부분이 BC 기반. 텔레옵 데이터 대량 확보로 scaling. Interactive IL로 contact-rich 작업 가능.
- **대표 성과**:
  - **ALOHA Unleashed**(DeepMind 2024-10, arXiv 2410.13126) — 26k demo만으로 신발끈·셔츠.
  - Interactive IL for Dexterous Manipulation Survey(Frontiers 2025).
  - A Survey on IL for Contact-Rich Tasks(Tsuji 2025-06, arXiv 2506.13498).
- **한계**: 인간 demo 노이즈 전이, distribution shift, 실패 회복 부족.

### 3-6. Diffusion Policy

- **정의**: 로봇 정책을 조건부 denoising diffusion으로 표현 — 다중모드 액션 분포 처리.
- **왜 지금**: 2023 Cheng Chi 이후 BC 계열 SOTA backbone. ALOHA Unleashed·Octo·RDT-1B·π0 계열 내재화. Flow matching·SE(3)-equivariant·3D 포인트클라우드 파생.
- **대표 성과**:
  - **Spherical Diffusion Policy (SDP)** — ICML 2025, SE(3)-equivariant spherical Fourier(arXiv 2507.01723).
  - Diffusion Policy 저널(IJRR 2024-09 정식 게재).
  - Diffusion Models for Robotic Manipulation Survey(Frontiers 2025).
- **한계**: 샘플링 스텝 inference 지연; 고주파 dexterous는 autoregressive tokenizer(FAST) 경쟁.

### 3-7. World Models (Cosmos 등)

- **정의**: 비디오/물리 시뮬 생성·예측 모델 — 상상 속 롤아웃 학습 또는 합성 데이터 생성.
- **왜 지금**: 2024-2025 Genie 2/3, Cosmos Predict/Transfer, Dreamer가 robot training loop에 실투입. 실 + 시뮬 + WFM 3각 체제 정착. Cosmos 3M+ downloads, 1X/Figure/Skild 채택.
- **대표 성과**:
  - **NVIDIA Cosmos** 런치(CES 2025-01-06) + Predict 2.5 / Transfer 2.5(2025-10).
  - **DeepMind Genie 3** — 텍스트→실시간 720p/24fps 인터랙티브 3D 월드, 수분간 object permanence(2025-08).
  - **NVIDIA GR00T-Dreams** — Cosmos Predict 기반 trajectory 추출, N1.5 학습 **3개월→36시간**.
- **한계**: 장기 consistency(Genie 3 수분 한계), 물리 정확도(접촉·변형체 약함), 합성 품질 보증 프로토콜 부재.

---

## Part 4. 통합 출처 목록

> 발행처·발행일 형식 `[제목](URL)` — 유형별로 그룹화. 상세 인용은 `docs/research-drafts/` 개별 초안 파일 참조.

### 공식 보고서 / 정부·협회

- [IFR World Robotics 2025 — Industrial](https://ifr.org/ifr-press-releases/news/global-robot-demand-in-factories-doubles-over-10-years) — IFR, 2025-09
- [IFR World Robotics 2025 Executive Summary PDF](https://ifr.org/img/worldrobotics/Executive_Summary_WR_2025_Industrial_Robots.pdf)
- [IFR Service Robots 2025](https://ifr.org/ifr-press-releases/news/service-robots-see-global-growth-boom) — 2025-10-07
- [IFR Global Robotics Race: Korea leads](https://ifr.org/ifr-press-releases/news/global-robotics-race-korea-singapore-and-germany-in-the-lead)
- [정책브리핑 K-휴머노이드 연합 출범](https://www.korea.kr/briefing/pressReleaseView.do?newsId=156683522)
- [정책브리핑 농업로봇 확산](https://www.korea.kr/news/policyNewsView.do?newsId=156685775)
- [한국AI·로봇산업협회](https://www.korearobot.or.kr/)
- [한국로봇산업진흥원 KIRIA](https://www.kiria.org/)
- [K-Humanoid Alliance Wikipedia](https://en.wikipedia.org/wiki/K-Humanoid_Alliance)

### 시장 조사

- [Fortune Business Insights — Collaborative Robots](https://www.fortunebusinessinsights.com/industry-reports/collaborative-robots-market-101692)
- [MarketsandMarkets — Collaborative Robot](https://www.marketsandmarkets.com/Market-Reports/collaborative-robot-market-194541294.html)
- [Precedence Research — Collaborative Robots](https://www.precedenceresearch.com/collaborative-robots-market)
- [Precedence Research — Robotic Simulator Market 2035](https://www.precedenceresearch.com/robotic-simulator-market)
- [MarketsandMarkets — AMR](https://www.marketsandmarkets.com/PressReleases/autonomous-mobile-robots.asp)
- [Grand View Research — AMR](https://www.grandviewresearch.com/industry-analysis/autonomous-mobile-robots-market)
- [MarketsandMarkets — Delivery Robots](https://www.marketsandmarkets.com/Market-Reports/delivery-robot-market-263997316.html)
- [Fortune BI — US Autonomous Last Mile](https://www.fortunebusinessinsights.com/us-autonomous-last-mile-delivery-market-115056)
- [SNS Insider — Surgical Robots 2035](https://orthospinenews.com/2026/04/13/surgical-robots-market-size-is-projected-to-attain-usd-38-27-billion-by-2035-sns-insider/)
- [DataM Intelligence — Hospital Robotics Logistics & Pharmacy](https://www.datamintelligence.com/research-report/hospital-robotics-logistics-and-pharmacy-market)
- [Global Growth Insights — Soft Exoskeleton](https://www.globalgrowthinsights.com/market-reports/soft-exoskeleton-exosuits-and-wearable-robots-market-100266)
- [IntelMarket Research — Commercial Service Robotics 2026-2034](https://www.intelmarketresearch.com/global-commercial-service-robotics-forecast-market-26549)
- [Roots Analysis — Autonomous Tractor Market 2035](https://www.rootsanalysis.com/autonomous-tractor-market)
- [Coherent Market Insights — Fruit Picking Robots](https://www.coherentmarketinsights.com/market-insight/fruit-picking-robots-market-4531)
- [Research Nester — Robotic Vacuum](https://www.researchnester.com/reports/robotic-vacuum-cleaner-market/8208)
- [Research Nester — Construction Robots](https://www.researchnester.com/reports/construction-robots-market/5225)
- [Global Growth Insights — Facade Cleaning Robot](https://www.globalgrowthinsights.com/market-reports/facade-cleaning-robot-market-111553)
- [Morgan Stanley — Humanoid $5T by 2050](https://www.morganstanley.com/insights/articles/humanoid-robot-market-5-trillion-by-2050)
- [Spherical Insights — Korea Surgery Robot](https://www.sphericalinsights.com/)

### 한국 기업 / 언론

- [로봇신문 — 2025 국내 10대 뉴스](https://www.irobotnews.com/news/articleView.html?idxno=44124)
- [로봇신문 — 큐렉소 2025 매출 745억](https://www.irobotnews.com/news/articleView.html?idxno=44779)
- [로봇신문 — 에이로봇 NVIDIA 기조](https://www.irobotnews.com/news/articleView.html?idxno=44237)
- [로봇신문 — 에이로봇 LGU+ MWC 2026](https://www.irobotnews.com/news/articleView.html?idxno=45185)
- [로봇신문 — 에이로봇 AWS 유니콘데이](https://www.irobotnews.com/news/articleView.html?idxno=45394)
- [로봇신문 — HD현대 조선 용접 휴머노이드](https://www.irobotnews.com/news/articleView.html?idxno=45489)
- [로봇신문 — AI 피킹로봇 시장](https://www.irobotnews.com/news/articleView.html?idxno=44198)
- [로봇신문 — 쿠팡 물류센터](https://www.irobotnews.com/news/articleView.html?idxno=29492)
- [한국경제 — 수술로봇 심사 10년](https://www.hankyung.com/article/2025112063341)
- [한국일보 — HD Hi7](https://www.hankookilbo.com/News/Read/A2025100113260005391)
- [이코노믹리뷰 — 두산로보틱스 2026 AI 재설계](https://www.econovill.com/news/articleView.html?idxno=726696)
- [두산로보틱스 2024 사업보고서 PDF](https://www.doosanrobotics.com/pdf/bereport_2024.pdf)
- [전자신문 — 토마토밭 스마트팜](https://www.etnews.com/20251009000070)
- [전자신문 — 뉴빌리티 251억](https://www.etnews.com/20251210000332)
- [와우테일 — 뉴빌리티 251억](https://wowtale.net/2025/12/10/251683/)
- [머니투데이 — 젠슨황 뉴빌리티](https://www.mt.co.kr/future/2025/12/11/2025121020264396675)
- [헤럴드경제 — 현대위아 CES 2026](https://biz.heraldcorp.com/article/10651129)
- [헤럴드경제 — 대동 AI 트랙터](https://biz.heraldcorp.com/article/10713353)
- [Bloter — 농슬라 대동 TYM](https://www.bloter.net/news/articleView.html?idxno=623705)
- [Bloter — 우아한형제들 딜리](http://www.bloter.net/archives/361340)
- [CJ뉴스룸 — 에이전틱 AI 휴머노이드](https://cjnews.cj.net/cj대한통운-에이전틱-ai와-휴머노이드로-물류의-미/)
- [LG Newsroom — LG전자 베어로보틱스](https://live.lge.co.kr/2501-lg-bear-robotics/)
- [LG Newsroom — CLOiD CES 2026](https://www.lg.co.kr/media/release/29723)
- [LG Newsroom — Q9 AI 에이전트](https://live.lge.co.kr/2403-ai-agent-q9/)
- [The bell — LG 로봇사업 점검](https://www.thebell.co.kr/free/content/ArticleView.asp?key=202503251554382040103261)
- [Forbes Korea — 국내 수술 로봇](https://www.forbeskorea.co.kr/news/articleView.html?idxno=400499)
- [인더스트리뉴스 — 협동로봇 시장](https://www.industrynews.co.kr/news/articleView.html?idxno=50550)
- [인더스트리뉴스 — 협동로봇 안전](https://www.industrynews.co.kr/news/articleView.html?idxno=51611)
- [디지털데일리 — 로봇청소기 2025 H1](https://m.ddaily.co.kr/page/view/2025102015385605157)
- [축산신문 — 외국인 계절근로자](https://www.chuksannews.co.kr/news/article.html?no=270412)
- [Korea Times — Workplace fatalities](https://www.koreatimes.co.kr/southkorea/society/20251127/why-do-workplace-fatalities-in-korea-keep-rising-despite-govt-crackdown)
- [Korea Herald — 20% Koreans 65+](https://www.koreaherald.com/article/10648363)
- [서울신문 — 초고령사회](https://www.seoul.co.kr/news/newsView.php?id=20260104500049)
- [CNN — Nurabot Foxconn NVIDIA](https://www.cnn.com/2025/09/12/tech/taiwan-nursing-robots-nurabot-foxconn-nvidia-hnk-spc)

### 해외 기업/기술 뉴스

- [The Robot Report — VLA next leap](https://www.therobotreport.com/vision-language-action-models-are-the-next-leap-in-autonomous-robotics/)
- [The Robot Report — Diligent 300k pharmacy](https://www.therobotreport.com/diligent-robotics-completes-300000-pharmacy-deliveries-with-moxi/)
- [The Robot Report — Moxi 2.0](https://www.therobotreport.com/diligent-robotics-moxi-2-0-mobile-manipulator-built-for-ai/)
- [The Robot Report — Starship Series C](https://www.therobotreport.com/starship-technologies-obtains-series-c-funding-for-autonomous-deliveries/)
- [The Robot Report — Coco $80M](https://www.therobotreport.com/coco-robotics-raises-80m-to-scale-sidewalk-delivery-robots/)
- [The Robot Report — Pi0 open-source](https://www.therobotreport.com/physical-intelligence-open-sources-pi0-robotics-foundation-model/)
- [The Robot Report — Atlas Hyundai Georgia](https://www.therobotreport.com/boston-dynamics-shows-atlas-humanoid-working-georgia-hyundai-plant/)
- [The Robot Report — AgiBot 10k](https://www.therobotreport.com/agibot-rolls-out-10000th-humanoid-robot/)
- [The Robot Report — Antioch pre-seed](https://www.therobotreport.com/antioch-raises-pre-seed-funding-accelerate-ai-robotics-testing/)
- [The Robot Report — DHL Stretch](https://www.therobotreport.com/dhl-buying-1000-stretch-robots-from-boston-dynamics/)
- [TechCrunch — Skild AI $14B](https://techcrunch.com/2025/12/08/softbank-and-nvidia-reportedly-in-talks-to-fund-skildai-at-14b-nearly-tripling-its-value/)
- [TechCrunch — GR00T N1](https://techcrunch.com/2025/03/18/nvidia-debuts-groot-n1-a-foundation-model-for-humanoid-robotics/)
- [TechCrunch — Ballie 2025 launch](https://techcrunch.com/2025/01/06/samsung-says-its-home-robot-ballie-will-roll-out-this-year/)
- [TechCrunch — Bifrost 3D](https://techcrunch.com/2024/10/30/bifrost-ai-raises-8m-for-its-3d-and-ai-data-generation-platform/)
- [TechCrunch — 1X NEO Gamma test](https://techcrunch.com/2025/03/21/1x-will-test-humanoid-robots-in-a-few-hundred-homes-in-2025/)
- [Business Wire — Skild AI $1.4B](https://www.businesswire.com/news/home/20260114335623/en/Skild-AI-Raises-$1.4B-Now-Valued-Over-$14B)
- [Business Wire — 1X NEO launch](https://www.businesswire.com/news/home/20251027434628/en/1X-Launches-NEO-The-Robot-Redefining-Life-at-Home)
- [Business Wire — Skild Brain 첫 공개](https://www.businesswire.com/news/home/20250729431330/en/Skild-AI-Provides-First-Look-at-Its-General-Purpose-Robotic-Brain)
- [GlobeNewswire — GreyOrange Google Cloud](https://www.globenewswire.com/news-release/2025/08/12/3131636/0/en/GreyOrange-Teams-With-Google-Cloud-on-Breakthrough-Warehouse-AI.html)
- [GlobeNewswire — CNH Tech Day](https://www.globenewswire.com/news-release/2025/11/11/3185279/0/en/CNH-2025-Tech-Day-showcasing-customer-centric-farming-innovations-across-AI-Autonomy-Robotics-and-Automation.html)
- [The AI Insider — Flexion $50M](https://theaiinsider.tech/2025/11/20/flexion-raises-50m-in-series-a-funding-to-build-the-brain-of-humanoid-robots/)
- [Crunchbase News — Skild triples valuation](https://news.crunchbase.com/venture/robotics-startup-skild-ai-triples-valuation/)
- [Restaurant Dive — Starship $50M](https://www.restaurantdive.com/news/starship-technologies-raises-50-million-us-robotics-delivery/802863/)
- [Fortune — Robot fast food $28B](https://fortune.com/2026/02/26/robot-disruption-fast-food-short-order-cook-flippy-labor-shortage/)
- [WebProNews — Serve mobility scooter](https://www.webpronews.com/delivery-robot-collides-with-mobility-scooter-sparking-accessibility-outrage/)
- [Block Club Chicago — Delivery robot petition](https://blockclubchicago.org/2025/12/08/delivery-robots-take-over-chicago-sidewalks-sparking-debate-and-a-petition-to-hit-pause/)
- [Supply Chain Dive — Delivery robot regulation](https://www.supplychaindive.com/news/delivery-robot-bills-laws-proliferate-state-legislatures/648303/)
- [Waymo — All-weather Driver](https://waymo.com/blog/2025/10/creating-an-all-weather-driver/)
- [Avride — Snow handling](https://medium.com/avride/how-avrides-four-wheeled-delivery-robots-handle-snow-5e5650ec6bf8)
- [Fox Business/DataM — Hospital robot](https://www.datamintelligence.com/research-report/hospital-robotics-logistics-and-pharmacy-market)
- [ANS Newswire — Rosatom Spider](https://www.ans.org/news/2025-10-28/article-7497/rosatom-deploys-robotic-spider-for-reactor-weld-inspections/)
- [AgFunder — DailyRobotics strawberry](https://agfundernews.com/dailyrobotics-gears-up-for-commercial-launch-in-california-in-2026-with-robotic-strawberry-harvester)
- [Intuitive Surgical — Q4 FY 2025](https://isrg.intuitive.com/news-releases/news-release-details/intuitive-announces-preliminary-fourth-quarter-and-full-year-5)
- [Medtronic — Hugo FDA urologic](https://news.medtronic.com/2025-12-03-Medtronic-announces-FDA-clearance-of-Hugo-TM-robotic-assisted-surgery-system-for-urologic-surgical-procedures)
- [Stryker — Mako RPS handheld](https://www.stryker.com/us/en/about/news/2026/stryker-introduces-mako-handheld-robotics-mako-rps.html)
- [Tesla Optimus V3 basenor](https://www.basenor.com/blogs/news/tesla-optimus-v3-production-starts-this-summer-full-timeline)
- [Agility Robotics — Digit 100k totes](https://www.agilityrobotics.com/content/digit-moves-over-100k-totes)
- [Agility Robotics — GXO RAAS](https://www.agilityrobotics.com/content/digit-deployed-at-gxo-in-historic-humanoid-raas-agreement)
- [Figure 03 intro](https://www.figure.ai/news/introducing-figure-03)
- [Figure Helix](https://www.figure.ai/news/helix)
- [Hyundai — AI Robotics Strategy CES 2026](https://www.hyundai.com/worldwide/en/newsroom/detail/0000001093)
- [Boston Dynamics — New Atlas](https://bostondynamics.com/blog/boston-dynamics-unveils-new-atlas-robot-to-revolutionize-industry/)
- [Boston Dynamics — Stretch product](https://bostondynamics.com/products/stretch/)
- [CnEVPost — XPeng IRON](https://cnevpost.com/2025/11/05/xpeng-unveils-next-gen-iron-humanoid-robot/)
- [PRNewswire — AGIBOT 10,000](https://www.prnewswire.com/news-releases/agibot-reaches-10-000-units-as-real-world-demand-for-robots-accelerates-302728295.html)
- [emag.directindustry — China humanoid deep](https://emag.directindustry.com/2026/03/17/china-humanoid-robots-market-unitree-robotics-agibot-ubtech-leju-xpeng/)
- [John Deere — Autonomous 9RX CES 2025](https://www.deere.com/en/news/all-news/autonomous-9RX/)
- [New Holland — R4 Autonomous](https://agriculture.newholland.com/en-gb/europe/new-holland-world/news/2025/new-holland-autonomous-r4-robot-series)
- [Lely — 3 new robots milking](https://roboticsandautomationnews.com/2025/08/05/lely-launches-three-new-robots-for-milking-cows/93499/)
- [DJI — 농업 연례 보고서 2025](https://www.dji.com/kr/newsroom/news/dji-agricultural-annual-report-2025)
- [People's Daily — Chinese robots](https://en.people.cn/n3/2025/1208/c90000-20399637.html)

### NVIDIA / 공식 기술 블로그

- [NVIDIA — GR00T N1 announcement](https://nvidianews.nvidia.com/news/nvidia-isaac-gr00t-n1-open-humanoid-robot-foundation-model-simulation-frameworks)
- [NVIDIA — Cosmos platform CES 2025](https://nvidianews.nvidia.com/news/nvidia-launches-cosmos-world-foundation-model-platform-to-accelerate-physical-ai-development)
- [NVIDIA — Cosmos major release](https://nvidianews.nvidia.com/news/nvidia-announces-major-release-of-cosmos-world-foundation-models-and-physical-ai-data-tools)
- [NVIDIA — Robotics research open models](https://nvidianews.nvidia.com/news/nvidia-accelerates-robotics-research-and-development-with-new-open-models-and-simulation-libraries)
- [NVIDIA Dev Blog — Isaac Sim 5.0 GA](https://developer.nvidia.com/blog/isaac-sim-and-isaac-lab-are-now-available-for-early-developer-preview/)
- [NVIDIA Dev Blog — Newton physics](https://developer.nvidia.com/blog/announcing-newton-an-open-source-physics-engine-for-robotics-simulation/)
- [NVIDIA Dev Blog — WFM synthetic trajectory](https://developer.nvidia.com/blog/enhance-robot-learning-with-synthetic-trajectory-data-generated-by-world-foundation-models/)
- [NVIDIA Dev Blog — R²D² World Foundation](https://developer.nvidia.com/blog/r2d2-training-generalist-robots-with-nvidia-research-workflows-and-world-foundation-models/)
- [NVIDIA Dev Blog — Isaac Lab 2.3 teleop](https://developer.nvidia.com/blog/streamline-robot-learning-with-whole-body-control-and-enhanced-teleoperation-in-nvidia-isaac-lab-2-3/)
- [Isaac Sim](https://developer.nvidia.com/isaac/sim)
- [GR00T N1.5](https://research.nvidia.com/labs/gear/gr00t-n1_5/)
- [GR00T N1.6](https://research.nvidia.com/labs/gear/gr00t-n1_6/)
- [Linux Foundation — Newton contribution](https://www.linuxfoundation.org/press/linux-foundation-announces-contribution-of-newton-by-disney-research-google-deepmind-and-nvidia-to-accelerate-open-robot-learning)

### Physical Intelligence / DeepMind / Figure / 1X / TRI

- [PI π0 arXiv 2410.24164](https://arxiv.org/abs/2410.24164)
- [PI π0.5 arXiv 2504.16054](https://arxiv.org/abs/2504.16054)
- [PI π*0.6 arXiv 2511.14759](https://arxiv.org/abs/2511.14759)
- [PI blog — π0.5](https://www.pi.website/blog/pi05)
- [DeepMind — Gemini Robotics 1.5](https://deepmind.google/blog/gemini-robotics-15-brings-ai-agents-into-the-physical-world/)
- [DeepMind — Genie 3 world model](https://deepmind.google/blog/genie-3-a-new-frontier-for-world-models/)
- [DeepMind — Genie 2](https://deepmind.google/blog/genie-2-a-large-scale-foundation-world-model/)
- [TRI — Large Behavior Models](https://www.tri.global/our-work/large-behavior-models)
- [TRI — Atlas LBM](https://www.tri.global/news/ai-powered-robot-boston-dynamics-and-toyota-research-institute-takes-key-step-towards-general)
- [1X — World Model PDF](https://www.1x.tech/1x-world-model.pdf)
- [1X — NEO Gamma intro](https://www.1x.tech/discover/introducing-neo-gamma)

### arXiv 논문 (2025 VLA·데이터·벤치마크)

- [GR00T N1 — arXiv 2503.14734](https://arxiv.org/abs/2503.14734)
- [OpenVLA — arXiv 2406.09246](https://arxiv.org/abs/2406.09246)
- [Octo — arXiv 2405.12213](https://arxiv.org/abs/2405.12213)
- [RT-2 — arXiv 2307.15818](https://arxiv.org/abs/2307.15818)
- [RDT-1B — arXiv 2410.07864](https://arxiv.org/abs/2410.07864)
- [Gemini Robotics 1.0 — arXiv 2503.20020](https://arxiv.org/abs/2503.20020)
- [Gemini Robotics 1.5 — arXiv 2510.03342](https://arxiv.org/abs/2510.03342)
- [FAST tokenizer — arXiv 2501.09747](https://arxiv.org/abs/2501.09747)
- [Mobile ALOHA — arXiv 2401.02117](https://arxiv.org/abs/2401.02117)
- [ALOHA 2 — arXiv 2405.02292](https://arxiv.org/abs/2405.02292)
- [ALOHA Unleashed — arXiv 2410.13126](https://arxiv.org/html/2410.13126v1)
- [UMI — arXiv 2402.10329](https://arxiv.org/abs/2402.10329)
- [DROID — arXiv 2403.12945](https://arxiv.org/abs/2403.12945)
- [Open X-Embodiment — arXiv 2310.08864](https://arxiv.org/abs/2310.08864)
- [AgiBot World — arXiv 2503.06669](https://arxiv.org/abs/2503.06669)
- [Humanoid Everyday — arXiv 2510.08807](https://arxiv.org/abs/2510.08807)
- [PH2D — arXiv 2503.13441](https://arxiv.org/html/2503.13441)
- [RoboArena — arXiv 2506.18123](https://arxiv.org/abs/2506.18123)
- [RobotArena ∞ — arXiv 2510.23571](https://arxiv.org/abs/2510.23571)
- [RoboChallenge — arXiv 2510.17950](https://arxiv.org/abs/2510.17950)
- [PolaRiS — arXiv 2512.16881](https://arxiv.org/abs/2512.16881)
- [REALM — arXiv 2512.19562](https://arxiv.org/html/2512.19562v1)
- [AutoEval — arXiv 2503.24278](https://arxiv.org/html/2503.24278v1)
- [ManiSkill3 — arXiv 2410.00425](https://arxiv.org/abs/2410.00425)
- [LIBERO-PRO — arXiv 2510.03827](https://arxiv.org/pdf/2510.03827)
- [LIBERO-Plus — arXiv 2510.13626](https://arxiv.org/abs/2510.13626)
- [HumanoidBench — arXiv 2403.10506](https://arxiv.org/abs/2403.10506)
- [MuJoCo Playground — arXiv 2502.08844](https://arxiv.org/html/2502.08844v1)
- [Isaac Lab survey — arXiv 2511.04831](https://arxiv.org/html/2511.04831v1)
- [Reality Gap Survey — arXiv 2510.20808](https://arxiv.org/abs/2510.20808)
- [Real-is-Sim — arXiv 2504.03597](https://arxiv.org/html/2504.03597v1)
- [VLA Survey — arXiv 2505.04769](https://arxiv.org/html/2505.04769v1)
- [Humanoid World Models — arXiv 2506.01182](https://arxiv.org/pdf/2506.01182)
- [Spherical Diffusion Policy — arXiv 2507.01723](https://arxiv.org/abs/2507.01723)
- [3D Diffusion Policy — arXiv 2403.03954](https://arxiv.org/html/2403.03954v1)
- [EmbodiedBench — arXiv 2502.09560](https://arxiv.org/html/2502.09560v1)
- [Embodied AI Review — arXiv 2505.14235](https://arxiv.org/pdf/2505.14235)
- [IL Contact-Rich Survey — arXiv 2506.13498](https://arxiv.org/html/2506.13498v1)
- [Foundation Model Robotics Review — arXiv 2507.10087](https://arxiv.org/html/2507.10087v1)
- [Genesis 물리 sim 과장 — Stone Tao substack](https://stoneztao.substack.com/p/the-new-hyped-genesis-simulator-is)

### Hugging Face / GitHub / 블로그

- [Hugging Face — SmolVLA blog](https://huggingface.co/blog/smolvla)
- [Hugging Face — LeRobotDataset v3 blog](https://huggingface.co/blog/lerobot-datasets-v3)
- [Hugging Face — π0/FAST blog](https://huggingface.co/blog/pi0)
- [GitHub — LeRobot](https://github.com/huggingface/lerobot)
- [GitHub — SO-ARM100](https://github.com/TheRobotStudio/SO-ARM100)
- [GitHub — Isaac Lab](https://github.com/isaac-sim/IsaacLab)
- [GitHub — Isaac Lab Issue #3043](https://github.com/isaac-sim/IsaacLab/issues/3043)
- [GitHub — MuJoCo](https://github.com/google-deepmind/mujoco)
- [GitHub — Genesis](https://github.com/Genesis-Embodied-AI/Genesis)
- [GitHub — GR00T-Dreams](https://github.com/NVIDIA/GR00T-Dreams)
- [GitHub — InteriorGS](https://github.com/manycore-research/InteriorGS)
- [GitHub — AgiBot World](https://github.com/OpenDriveLab/AgiBot-World)
- [GitHub — SimplerEnv](https://github.com/simpler-env/SimplerEnv)
- [GitHub — HumanoidBench](https://github.com/carlosferrazza/humanoid-bench)
- [GitHub — ManiSkill](https://github.com/haosulab/ManiSkill)
- [GitHub — Awesome Sim2Real](https://github.com/LongchaoDa/AwesomeSim2Real)
- [Sergey Levine — Sporks of AGI](https://sergeylevine.substack.com/p/sporks-of-agi)

### 평가/벤치마크 프로젝트 페이지

- [DROID project](https://droid-dataset.github.io/)
- [Real2Sim Workshop CVPR 2025](https://real2simworkshop.github.io/)
- [Scalable Real2Sim](https://scalable-real2sim.github.io/)
- [Embodied Gaussians](https://embodied-gaussians.github.io/)
- [GWM — ICCV 2025 paper PDF](https://openaccess.thecvf.com/content/ICCV2025/papers/Lu_GWM_Towards_Scalable_Gaussian_World_Models_for_Robotic_Manipulation_ICCV_2025_paper.pdf)
- [ALOHA page](https://tonyzhaozh.github.io/aloha/)
- [Cosmos-Predict GitHub](https://github.com/nvidia-cosmos/cosmos-predict2.5)

---

## 부록. 조사 한계 & 주의사항

1. **시장 규모 수치의 편차**: 협동로봇·AMR·합성 데이터 영역에서 리서치펌별 추정 편차가 **2배 이상** 발생. **IFR 공식 지표(설치 대수·밀도)**가 가장 신뢰도 높으며, 민간 리서치펌 수치는 추정치임을 명시하고 사용할 것.

2. **VLA·FM은 시연 단계와 상용 단계 구분 필요**: π0.5·GR00T N1·Helix 등은 **연구·오픈소스 시연** 단계이며, 실제 공장/창고 대규모 KPI(pick/hr, 가동률)는 공개되지 않음. 기획안에 "이미 상용화됨"으로 오기재 금지.

3. **Ballie·Optimus V3 등 반복 지연**: 삼성 Ballie는 2024 이후 **3회 출시 지연**, Optimus V3는 2024 말 양산 예고 → 2026 여름 지연. "예고 시점"과 "실제 출시"를 구분하여 기술.

4. **arXiv 번호 검증**: 본 문서 arXiv 번호는 WebSearch로 URL·제목 교차검증된 것만 기재(2303.04137, 2307.15818, 2310.08864, 2401.02117, 2402.10329, 2403.12945, 2403.10506, 2403.03954, 2405.02292, 2405.12213, 2406.09246, 2410.00425, 2410.07864, 2410.13126, 2410.24164, 2501.09747, 2502.08844, 2502.09560, 2503.06669, 2503.13441, 2503.14734, 2503.20020, 2503.24278, 2504.03597, 2504.16054, 2505.04769, 2505.14235, 2506.01182, 2506.13498, 2506.18123, 2507.01723, 2507.10087, 2510.03342, 2510.03827, 2510.08807, 2510.13626, 2510.17950, 2510.20808, 2510.23571, 2511.04831, 2511.14759, 2512.13411, 2512.16881, 2512.19562).

5. **AI Smart Factory와의 경계** (MISSION.md 주의사항 반영): 공정 관리·최적화는 Smart Factory 영역. 본 문서는 **로봇 개체의 인지·의사결정·행동** 또는 **그 지능을 만드는 플랫폼/인프라**에 한정.

6. **중첩 도메인**:
   - 의료로봇(A-4) ↔ Healthcare 도메인
   - 배송드론(A-3) ↔ Mobility 도메인
   - 건설로봇(A-8) ↔ Construction Tech
   - 농업로봇(A-6) ↔ AgriTech

   팀이 도메인 귀속을 판단할 때 참고할 것.

7. **출처 드래프트 상세본**: 각 영역별로 인용 수치·대조 출처는 [docs/research-drafts/](research-drafts/) 참조.

---

## 검증 체크리스트 (계획서 종료 조건)

- [x] 14개 하위 영역 지도 (9 응용 + 5 플랫폼)
- [x] 영역별 What / 플레이어 / 최근 1년 트렌드
- [x] 영역별 페인포인트 2~4개 + 기존 서비스 맵핑 표
- [x] Cross-cutting 주목 기술 트렌드 7개 (VLA / FM / Embodied / Sim2Real / IL / Diffusion Policy / World Models)
- [x] 통합 출처 목록 200+ 링크
- [x] 발행일·발행처 명시 (수치 사실은 복수 출처 교차 인용)

**[docs/IDEAS.md](IDEAS.md)는 리서치 다음 단계(후보 선정)용으로 비워둡니다.**
