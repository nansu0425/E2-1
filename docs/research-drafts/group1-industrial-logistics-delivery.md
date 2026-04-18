# AI Robotics — 산업용/협동, 물류, 배달 리서치

**기준일**: 2026-04-18 | "최근 1년" = 2025-04 ~ 2026-04

## 공통 배경

- **IFR World Robotics 2025**: 2024년 산업용 로봇 신규 설치 **542,000대**(4년 연속 50만 돌파), 아시아 74%. 2025년 6% 성장해 575,000대 전망.
- **협동로봇(cobot) 설치**: 2017년 11,100대 → 2024년 **64,500대**, 산업용 내 비중 2.8% → 11.9%.
- **한국 로봇 밀도**: 제조업 종사자 1만 명당 **1,012~1,220대**(세계 1위).
- **정책**: 제4차 지능형로봇 기본계획 — 2030년까지 3조원, 로봇 100만 대 보급. K-휴머노이드 연합 2025-04 출범(1조원 이상, 2028 목표).

## [영역 1] 산업용/협동 로봇

### 1. 시장/도입 현황
- 글로벌 cobot 시장 2025: **US$ 3.06B ~ 4.18B**, 2026: US$ 3.38B~5.43B, CAGR 18.9~29.9%. 2035: US$ 85.93B (Precedence).
- APAC 점유율 2025 **42%** (Grand View).
- 한국 cobot 시장 **약 3.6억 달러**(인더스트리뉴스).
- 자동차 산업이 최대 수요처(45%, IFR).
- **국내/해외 온도차**: 해외는 UR(UR20/UR30 25kg/35kg 상향), FANUC/ABB AI-cobot 공격. 국내는 두산·한화·레인보우·HD현대로보틱스가 중국 저가 + 규모 경제 미실현으로 적자. 두산로보틱스는 매출 83%가 cobot, 2026 흑자전환 목표.

### 2. 주요 플레이어
| 구분 | 기업 | 비고 |
|---|---|---|
| 국내 | 두산로보틱스 | 2026 CES Scan & Go(AMR+cobot+3D 비전 AI) AI 최고혁신상 2개. NVIDIA와 Physical AI 협업 |
| 국내 | HD현대로보틱스 | 2026까지 10종 신제품, AI 제어기 Hi7(2025-10). 노이라와 조선 4족 용접 휴머노이드 |
| 국내 | 레인보우로보틱스 | 삼성 지분 확대, 그룹 로봇 중심축 |
| 국내 | 한화로보틱스 | 2023 분사, 식음료·서비스 확장 |
| 해외 | UR(Teradyne) | PolyScope X + NVIDIA Isaac AI Accelerator |
| 해외 | FANUC/ABB/KUKA/Yaskawa | 전통 4강 |
| 해외 | Physical Intelligence | π0/π0.5 오픈소스 VLA |

### 3. 최근 1년 기술 트렌드
- **VLA 파운데이션 모델 상용화 초입**: π0/π0.5, GR00T N1(2025-03, 합성 780k trajectory), Gemini Robotics, OpenVLA(7B), SmolVLA(450M).
- **Physical AI + 디지털 트윈**: Isaac Sim, Newton(DeepMind+Disney).
- **ISO 10218-2:2025 + ISO/TS 15066** 통합: cobot을 "로봇 응용"으로 재정의.
- **AI 비전 bin picking 성숙**: Inbolt 온-암 AI(2025-12), pick 1초 미만 + 95% 성공률.
- **한국**: 이동식 협동로봇 산업표준, 대구 규제자유특구, 2025 AI 규제합리화 로드맵.
- **RaaS 확산**: Rapid Robotics, Vention.

### 4. 공공연한 문제/한계
- 속도-안전 트레이드오프(ISO 10218-2에 따른 재설정).
- cobot 도입 기업 산재 증가 보고(ScienceDirect 2025).
- 중소 현장 사이클 타임 오히려 증가 (기계신문 2025).
- 통합/프로그래밍 비용: 셀 전체 $50k~150k+.
- 국내 제조사 적자, 중국 저가 경쟁.

### 5. 현장 페인포인트
1. 프로그래밍·재설정 부담 (다품종 소량).
2. 안전영역 전략 부재 → 일괄 저속화.
3. Bin picking 실패(겹침·반사·파지 간섭).
4. SMB 자본 부담 (ROI 12-18개월).
5. 한국 특유: 중국 저가 유입, 규제 해석 혼란.

### 6. 기존 제품 맵핑
| 제품 | 기능 | AI | 한계 |
|---|---|---|---|
| UR20/UR30 + AI Accelerator | 25~35kg, PolyScope X | NVIDIA Isaac | 별도 HW/옵션 |
| 두산 Scan & Go | cobot+AMR 통합 | Physical AI, 3D | 상용 초기 |
| HD Hi7 | AI 제어기 | 위험 예측 | 협동용 부족 |
| π0.5 | 모바일 매니퓰레이터 | VLA | 실환경 일반화 초기 |
| GR00T N1 | 휴머노이드 FM | 멀티모달 VLA | HW 보급 전 |
| Inbolt on-arm | 랜덤빈 피킹 | 온-암 AI 비전 | 레퍼런스 부족 |

### 7. 기술적 공백
- 실시간 안전영역 재구성 (작업자 위치 인식 기반 속도/토크 조정).
- 자연어 재티칭 (말/시연 한두 번으로 공정 학습).
- 다품종 소량 제로샷 비전 피킹 (FM은 있으나 SME 배포 X).
- 국내 cobot 제조사 자체 FM 부재 (HD 'RFM' 언급, 미출시).

## [영역 2] 물류/창고 로봇

### 1. 시장/도입 현황
- AMR 2026: **US$ 2.75B~6.18B**(보고서별), 2032: US$ 7.07B, CAGR 14.4%.
- AI 피킹로봇 2024 $2.3B → 2034 **$240B**(10배↑, 로봇신문).
- 2025 글로벌 로지스틱스 로봇 판매 **450,000대+**(2019 대비 +500%).
- Amazon 로봇 **100만 대+** 보유(2025-07 돌파).
- **국내**: 쿠팡 대구 FC(아시아 최대), THiRAbot AGV·소팅봇. 자동화 인력 330(2024-01) → 750(2025-10).
- **CJ대한통운** 군포 FC 국내 최초 AI 휴머노이드 실증, Icheon 허브 5G 프라이빗망 + 500대 로봇 sub-10ms.

### 2. 주요 플레이어
| 구분 | 기업 | 비고 |
|---|---|---|
| 국내 | 쿠팡 | AGV/소팅봇 |
| 국내 | CJ대한통운 | 에이전틱 AI + 휴머노이드, RFM |
| 국내 | 티엑스알로보틱스 | 쿠팡 물류 |
| 국내 | 씨메스 | 3D 비전+AI 피킹 |
| 해외 | Amazon Robotics | Sequoia(+75%), Proteus, Sparrow, Digit |
| 해외 | Boston Dynamics | Stretch(700 case/hr), DHL 1,000+대 |
| 해외 | Locus Robotics | DHL 5억 건 피킹(2024-06) |
| 해외 | Geek+ 상장(2025), GreyOrange Series D $135M+ Google Cloud DeepNav(2025-08) |
| 해외 | Agility Robotics Digit | Amazon FC 토트 테스트 |

### 3. 최근 1년 기술 트렌드
- 휴머노이드의 창고 진입 (Digit Amazon, CJ 휴머노이드).
- 오케스트레이션 + Gen AI: GreyOrange × Google Gemini DeepNav.
- 대규모 VLA/FM 접목: CJ + Physical AI, Isaac GR00T 기반.
- 5G 프라이빗 네트워크(CJ 500대 sub-10ms).
- 복잡 SKU bin picking 적응형 그립.
- DHL 1,000+ Stretch MOU(2025-05), Otto Group 20+ 시설.

### 4. 공공연한 문제/한계
- SKU 다양성 대응 (이형·파손품 변동).
- 피킹 실패 원인: 엉킴·마찰 부족·포즈 추정 오류.
- 성수기 노동 수요: MHI 2025 — 45~52% 기업 "노동 확보 매우 어렵다".
- Jacobin(2025-12): 로봇화가 근골격 부상 패턴만 이동.
- 다기능 훈련이 부상과 상관.

### 5. 현장 페인포인트
1. 피킹 정확도 99.5%+ but 이형·변형 SKU 급락.
2. 성수기 인력 충원 불가.
3. 로봇 간 트래픽 혼잡 / 사람 협착.
4. SW 통합 복잡도 (WMS-로봇 OS-AMR).

### 6. 기존 제품 맵핑
| 제품 | 기능 | AI | 한계 |
|---|---|---|---|
| Amazon Sequoia | 컨테이너 피킹 통합 | 비전+모션 | 품목 형상 제약 |
| Amazon Digit | 이족, 토트 재활용 | Locomotion+manip | 파일럿 |
| BD Stretch | 언로딩 700 case/hr | 비전+딥러닝 파지 | 케이스박스 위주 |
| Locus AMR | 피킹 어시스트 | 경로·주문 AI | 사람이 파지 |
| GreyOrange DeepNav | 동적 오케스트레이션 | Gemini LLM | 신규 출시 |
| Geek+ | Goods-to-person | 경로 AI | 고정 선반 |
| 쿠팡 THiRAbot | 반송/분류 | 비전·스케줄 | 내부 전용 |
| CJ 휴머노이드 PoC | 포장/분류 | RFM + Gen AI | 초기 PoC |

### 7. 기술적 공백
- 완전 이형·깨지기 쉬운·비포장 SKU 제로샷 피킹.
- 로봇+사람 혼재 실시간 동선 예측.
- 휴머노이드 실제 FC 운영 KPI 공개 부재.
- 국내 중견·중소 3PL 고가 AMR 장벽, RaaS 확산 미흡.

## [영역 3] 배달/라스트마일 로봇

### 1. 시장/도입 현황
- 글로벌 배달로봇 2025: **US$ 0.80B**(M&M), 2026 자율 라스트마일 **US$ 1.6B**(Fortune BI), 2030 US$ 3.24B CAGR 32.4%.
- 국내: 2021 $2.71M → 2026 **$14.65M**, 연 40%(세계 최고, KISTI).
- Starship: 누적 **900만 건, 1,900만 km, 2,700대, 270 사이트, 7개국**. 2027 **12,000대** 목표.

### 2. 주요 플레이어
| 구분 | 기업 | 비고 |
|---|---|---|
| 국내 | 뉴빌리티 | 2025-12 251억 Series B(누적 550억), 재주문율 80%, 142 사이트 |
| 국내 | 우아한형제들 딜리 | 실내 서빙 렌탈(월 90만, 2년) |
| 국내 | 로보티즈 | 실외 '개미' LG사이언스파크 실증 |
| 해외 | Starship | Uber Eats·Grubhub·Bolt 제휴 |
| 해외 | Serve Robotics | $80M(2025-01) + DoorDash(2025-10) + Uber Eats 2,000대 |
| 해외 | Nuro | $6B valuation, Uber·Lucid 2031 20,000대 |
| 해외 | Coco Robotics | $80M Series B(2025-06), 누적 $120M+ |
| 해외 | Kiwibot | 30+ 미국 대학 |
| 해외 | Avride | 4륜, 2025 눈길 주행 |

### 3. 최근 1년 기술 트렌드
- 대형 플랫폼-로봇 제휴(Uber/DoorDash/Starship).
- 자금 유입: Coco $80M, Starship $50M, Serve $80M, 뉴빌리티 251억.
- 전천후 주행: Waymo all-weather, Avride 눈길.
- 한국 규제 완화: 2023 지능형로봇법 개정(500kg/15km/h 보도 허용 + 의무보험), 2025 로드맵(16→8개 항목, 60→30일).
- 순찰·보안 겸업(뉴빌리티 북미·사우디).

### 4. 공공연한 문제/한계
- **사고 급증**: Coco LA 버스쉘터 유리 파손, 시카고 CTA 버스쉘터 파손. Serve WH 뇌성마비 mobility scooter 충돌 반복.
- 시카고 파일럿 중단 청원 800명+(2025-12).
- 접근성 침해 (휠체어·보행기).
- 규제 패치워크.
- 날씨 취약 (폭설 중단).
- 보도법 제약(15km/h·500kg).

### 5. 현장 페인포인트
1. 보행자·접근성 약자 충돌/차단.
2. 계단·경사·엘리베이터.
3. 도난·장난.
4. 운영비 대비 건당 수익성.

### 6. 기존 제품 맵핑
| 제품 | 기능 | AI | 한계 |
|---|---|---|---|
| Starship | 보도 자율, 1.5~2km | 비전·LiDAR | 소형 페이로드, 폭설 |
| Serve Gen3 | 보도, 4시간+ | Jetson | 사고 사례 |
| Nuro R3 | 공공도로 | end-to-end | B2C 피벗 |
| Coco | 보도(하이브리드) | 비전+텔레옵 | 충돌 사고 |
| 뉴빌리티 뉴비 | 실외+순찰 | 저가 카메라 SLAM | 15km/h, 엘리베이터 |
| 우아한 딜리 | 실내 서빙 | 실내 SLAM | 테이블번호 수동 |
| Kiwibot | 캠퍼스 | 비전·LiDAR | 학내 한정 |

### 7. 기술적 공백
- 실내↔실외 연속 배송 (공동현관·엘리베이터 자동 연동).
- 이형 지형(눈/빗물/연석) 안정 주행.
- 보행자 의도 예측 + 접근성 인지 (휠체어·시각장애인).
- 소량·초소형 상품(의약품) 도심 배송.
- 한국 MaaS 요금제 (실외 B2C 단가).

## 통합 출처 (80+)

### 영역 1 산업/협동
- IFR World Robotics 2025: https://ifr.org/ifr-press-releases/news/global-robot-demand-in-factories-doubles-over-10-years
- IFR Executive Summary: https://ifr.org/img/worldrobotics/Executive_Summary_WR_2025_Industrial_Robots.pdf
- IFR Korea leads: https://ifr.org/ifr-press-releases/news/global-robotics-race-korea-singapore-and-germany-in-the-lead
- The Robot Report doubled: https://www.therobotreport.com/ifr-industrial-robot-deployments-have-doubled-in-10-years/
- Fortune Business Insights cobot: https://www.fortunebusinessinsights.com/industry-reports/collaborative-robots-market-101692
- MarketsandMarkets cobot: https://www.marketsandmarkets.com/Market-Reports/collaborative-robot-market-194541294.html
- Precedence Research cobot: https://www.precedenceresearch.com/collaborative-robots-market
- 인더스트리뉴스: https://www.industrynews.co.kr/news/articleView.html?idxno=50550
- 삼일PwC: https://www.pwc.com/kr/ko/insights/industry-focus/industrial-robot-market.html
- 로봇신문 10대 뉴스: https://www.irobotnews.com/news/articleView.html?idxno=44124
- 이코노믹리뷰 두산: https://www.econovill.com/news/articleView.html?idxno=726696
- 두산로보틱스 2024 사업보고서: https://www.doosanrobotics.com/pdf/bereport_2024.pdf
- 한국일보 HD Hi7: https://www.hankookilbo.com/News/Read/A2025100113260005391
- K-Humanoid Alliance Wikipedia: https://en.wikipedia.org/wiki/K-Humanoid_Alliance
- 정책브리핑 K-휴머노이드: https://www.korea.kr/briefing/pressReleaseView.do?newsId=156683522
- The Robot Report VLA: https://www.therobotreport.com/vision-language-action-models-are-the-next-leap-in-autonomous-robotics/
- VLA Wikipedia: https://en.wikipedia.org/wiki/Vision-language-action_model
- PI π0.5: https://www.physicalintelligence.company/blog/pi05
- arXiv 2410.24164: https://arxiv.org/abs/2410.24164
- NVIDIA GR00T N1: https://nvidianews.nvidia.com/news/nvidia-isaac-gr00t-n1-open-humanoid-robot-foundation-model-simulation-frameworks
- UR20 product: https://www.universal-robots.com/products/ur20/
- Robot Report UR30 payload: https://www.therobotreport.com/universal-robots-increases-payload-capacity-of-ur20-ur30-cobots/
- Standard Bots safety: https://standardbots.com/blog/collaborative-robot-safety-standards
- Frontiers cobot review 2025: https://www.frontiersin.org/journals/robotics-and-ai/articles/10.3389/frobt.2025.1605682/full
- ScienceDirect HRC safety 2025: https://www.sciencedirect.com/science/article/abs/pii/S0040162525000538
- 기계신문 거북이: https://www.mtnews.net/news/articleView.html?idxno=23639
- 정책브리핑 이동식 cobot 표준: https://korea.kr/news/policyNewsView.do?newsId=148935814
- Bloomberg Korea aging: https://www.bloomberg.com/news/newsletters/2025-01-07/robots-fill-workforce-gap-in-korea-s-aging-society
- Trade.gov Korea Robotics: https://www.trade.gov/market-intelligence/south-korea-robotics-industry
- Inbolt bin picking: https://roboticsandautomationnews.com/2025/12/30/inbolt-launches-human-like-bin-picking-solution-powered-by-on-arm-ai-vision/97944/

### 영역 2 물류
- MarketsandMarkets AMR: https://www.marketsandmarkets.com/PressReleases/autonomous-mobile-robots.asp
- Grand View AMR: https://www.grandviewresearch.com/industry-analysis/autonomous-mobile-robots-market
- 로봇신문 AI피킹: https://www.irobotnews.com/news/articleView.html?idxno=44198
- Cyzerg 2025 trends: https://cyzerg.com/blog/5-warehouse-automation-trends-2025/
- Automate.org Amazon 1M: https://www.automate.org/robotics/industry-insights/amazon-robotics-surpasses-one-million-systems-deployed
- aboutamazon 2 new: https://www.aboutamazon.com/news/operations/amazon-introduces-new-robotics-solutions
- Robotics 24/7 Sequoia+Digit: https://www.robotics247.com/article/amazon_tests_sequoia_system_and_agility_robotics_digit_for_fulfillment
- Jacobin Amazon: https://jacobin.com/2025/12/amazon-robots-automation-workforce-ai
- DHL Group 1,000 Stretch: https://group.dhl.com/en/media-relations/press-releases/2025/dhl-group-signs-mou-with-boston-dynamics-and-accelerates-cross-business-automation-strategy.html
- Robot Report DHL Stretch: https://www.therobotreport.com/dhl-buying-1000-stretch-robots-from-boston-dynamics/
- Boston Dynamics Stretch: https://bostondynamics.com/products/stretch/
- GreyOrange Google Cloud: https://www.globenewswire.com/news-release/2025/08/12/3131636/0/en/GreyOrange-Teams-With-Google-Cloud-on-Breakthrough-Warehouse-AI.html
- 로봇신문 쿠팡: https://www.irobotnews.com/news/articleView.html?idxno=29492
- 디일렉 티엑스알: https://www.thelec.kr/news/articleView.html?idxno=33343
- CJ뉴스룸 휴머노이드: https://cjnews.cj.net/cj대한통운-에이전틱-ai와-휴머노이드로-물류의-미/
- CJ Latest: https://www.cjlogistics.com/ko/newsroom/latest/LT_00000411
- McKinsey logistics: https://www.mckinsey.com/industries/logistics/our-insights/automation-in-logistics-big-opportunity-bigger-uncertainty
- McKinsey warehouse: https://www.mckinsey.com/capabilities/operations/our-insights/getting-warehouse-automation-right
- TGW picking: https://www.tgw-group.com/us/news/detail/robotic-picking-trends/
- ScienceDirect bin-picking 2025: https://www.sciencedirect.com/science/article/abs/pii/S0921889025003331

### 영역 3 배달
- M&M delivery: https://www.marketsandmarkets.com/Market-Reports/delivery-robot-market-263997316.html
- Fortune BI US last mile: https://www.fortunebusinessinsights.com/us-autonomous-last-mile-delivery-market-115056
- Starship $50M: https://www.starship.xyz/press/starship-technologies-raises-50m-series-c/
- Robot Report Starship: https://www.therobotreport.com/starship-technologies-obtains-series-c-funding-for-autonomous-deliveries/
- Restaurant Dive: https://www.restaurantdive.com/news/starship-technologies-raises-50-million-us-robotics-delivery/802863/
- Starship Uber Eats: https://www.starship.xyz/press/starship-technologies-and-uber-eats-launch-autonomous-delivery-partnership/
- Robot Report Coco: https://www.therobotreport.com/coco-robotics-raises-80m-to-scale-sidewalk-delivery-robots/
- DC Velocity Coco: https://www.dcvelocity.com/transportation/trucking/parcel-postal-carriers/sidewalk-delivery-bot-firm-coco-robotics-raises-80-million
- WebProNews Serve: https://www.webpronews.com/delivery-robot-collides-with-mobility-scooter-sparking-accessibility-outrage/
- CM Eaglet Chicago: https://thecmeaglet.com/chicago-delivery-robot-smashes-through-bus-shelter-glass-raising-safety-concerns-over-pilot-program/
- Block Club Chicago petition: https://blockclubchicago.org/2025/12/08/delivery-robots-take-over-chicago-sidewalks-sparking-debate-and-a-petition-to-hit-pause/
- Supply Chain Dive: https://www.supplychaindive.com/news/delivery-robot-bills-laws-proliferate-state-legislatures/648303/
- RAN last-mile: https://roboticsandautomationnews.com/2025/09/26/last-mile-delivery-robots-navigating-sidewalks-and-urban-landscapes/94758/
- 와우테일 뉴빌리티: https://wowtale.net/2025/12/10/251683/
- 전자신문 뉴빌리티: https://www.etnews.com/20251210000332
- 머니투데이 젠슨황: https://www.mt.co.kr/future/2025/12/11/2025121020264396675
- 뉴빌리티: https://www.neubility.co.kr/ko
- Bloter 딜리: http://www.bloter.net/archives/361340
- ZDNet 실외로봇: https://zdnet.co.kr/view/?no=20230728173101
- 로봇신문 법개정: https://www.irobotnews.com/news/articleView.html?idxno=31475
- Waymo all-weather: https://waymo.com/blog/2025/10/creating-an-all-weather-driver/
- Avride snow: https://medium.com/avride/how-avrides-four-wheeled-delivery-robots-handle-snow-5e5650ec6bf8
