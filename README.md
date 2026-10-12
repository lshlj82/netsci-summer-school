# 거듭제곱 법칙과 척도 없는 네트워크: 네트워크 과학 인터랙티브 데모

『[네트워크 사이언스](https://www.acornpub.co.kr/product/%EB%84%A4%ED%8A%B8%EC%9B%8C%ED%81%AC-%EC%82%AC%EC%9D%B4%EC%96%B8%EC%8A%A4/5911/category/25/display/1/)』(에이콘출판사, 2023) 4장 **척도 없는 성질(the scale-free property)** 과 『[네트워크 분석](https://www.acornpub.co.kr/product/%EB%84%A4%ED%8A%B8%EC%9B%8C%ED%81%AC-%EB%B6%84%EC%84%9D/5797/category/25/display/1/)』(에이콘출판사, 2022) 3장 **허브(hubs)** 의 내용을, 네트워크를 직접 만들고 링크수 분포를 그려 보며 배우는 웹 데모 모음입니다.

경상국립대학교 물리학과 [이상훈](https://sites.google.com/view/netscilab/principal-investigator) 교수가 [2024 복잡계 여름학교](https://www.complexity.kr/?p=1268)에서 진행한 ‘거듭제곱 법칙과 척도 없는 네트워크’ 강의의 강의자료를 기반으로, Claude Opus 5.5(Anthropic)가 제작했습니다.

**데모 바로가기:** https://lshlj82.github.io/netsci-summer-school/

## 데모 목록

| 번호 | 파일 | 다루는 내용 |
|:---:|---|---|
| 01 | [`01-power-law-scale-free.html`](01-power-law-scale-free.html) | 월드와이드웹과 허브, 무작위 네트워크와 척도 없는 네트워크의 비교, 로그 척도, 척도 변환과 “척도 없음”의 의미, 프랙탈 차원, 이산적인 형식과 연속적인 형식의 정규화 |
| 02 | [`02-hubs-moments.html`](02-hubs-moments.html) | 허브와 꼬리, 가장 큰 허브의 크기, 고속도로와 항공로, 링크수 분포의 모멘트와 발산, 실제 네트워크의 표준편차, 보편성 |
| 03 | [`03-plotting-fitting.html`](03-plotting-fitting.html) | 선형 묶기, 로그 묶기, 누적 분포, 등수 그림, 최소제곱법과 최대우도추정, 적합도 검정과 p-값, “척도 없는 네트워크는 드물다” 논쟁 |
| 04 | [`04-networks-tails.html`](04-networks-tails.html) | 극단적인 좁은 세상, 링크수 지수의 역할과 에르되시-갈라이 정리, 구조 모형, 이웃 수 보존 무작위화, 숨은 매개변수 모형, 두꺼운 꼬리와 혼합된 분포 |

<!-- 새 데모를 추가하면 위 표에 한 줄씩 추가하세요. -->

## 정규 교과목

이 특강의 주제는 경상국립대학교 물리학과 정규 교과목 「네트워크 과학」에서도 다룹니다.

- **교과목 보조자료 페이지**: https://lshlj82.github.io/netsci-course-GNU/ ([소스](https://github.com/lshlj82/netsci-course-GNU)). 네트워크의 기본 요소에서 네트워크 동역학까지 열한 가지 브라우저 시뮬레이션.
- **척도 없는 네트워크 데모**(교과목 데모 7): https://lshlj82.github.io/SFN/ ([소스](https://github.com/lshlj82/SFN)). 무작위 네트워크와 척도 없는 네트워크의 비교, 견고성, 경로 길이.

## 주요 기능

- **네트워크를 직접 만들기**: 같은 노드 수와 평균 링크수를 가진 무작위 네트워크와 척도 없는 네트워크를 브라우저에서 생성하고, 힘 기반 배치(force-directed layout)로 그려 허브를 눈으로 비교합니다.
- **로그 척도 실험**: 같은 분포를 선형 척도, 세로축만 로그, 모두 로그 척도로 바꿔 가며 그려 봅니다.
- **통계적 추정과 검정**: 같은 표본에 선형 묶기, 로그 묶기, 누적 분포, 등수 그림을 적용해 비교하고, 최소제곱법과 최대우도추정의 링크수 지수를 반복 실험으로 비교하며, 콜모고로프-스미르노프 거리와 가상 데이터로 p-값을 계산합니다.
- **네트워크 모형 조립**: 구조 모형의 미연결 링크 짝짓기, 이웃 수 보존 링크 교환, 숨은 매개변수 모형을 단계별로 실행합니다.
- **척도 변환**: 기준 링크수 k와 배율 b를 움직여, 거듭제곱 분포의 비율 p(bk)/p(k)가 k와 무관하게 일정하다는 것을 푸아송 분포와 비교해 확인합니다.
- **한국어 본문, 영어 원어 병기**: 중요한 용어는 괄호 안에 영어 원어를 함께 적었습니다.
- **반응형, 화면 모드 전환, 동작 줄이기 설정 지원**: 휴대폰에서도 사용할 수 있습니다. 처음에는 운영체제 설정에 맞춰 열리고, 오른쪽 위 버튼으로 라이트와 다크 모드를 바꿀 수 있으며 선택은 브라우저에 저장됩니다. "동작 줄이기(reduced motion)" 설정도 따릅니다.

## 저장소 구조

```
.
├── index.html                       # 전체 데모 목록(첫 화면)
├── 01-power-law-scale-free.html     # 거듭제곱 분포와 척도 없음
├── 02-hubs-moments.html             # 허브와 모멘트
├── 03-plotting-fitting.html         # 링크수 분포 그리기와 지수 측정
├── 04-networks-tails.html           # 네트워크 만들기와 꼬리의 종류
└── README.md
```

각 HTML 파일은 CSS와 JavaScript를 모두 안에 담은 독립된 단일 파일입니다. 수식은 [KaTeX](https://katex.org/)로 미리 조판해 HTML에 넣어 두었기 때문에 실행 중에 수식 라이브러리를 불러오지 않습니다. 외부에서 불러오는 것은 KaTeX의 스타일시트와 수식 글꼴(jsDelivr CDN, 버전 0.16.9 고정, 무결성 해시 포함), 그리고 Google Fonts(Noto Serif KR, Noto Sans KR, STIX Two Text)뿐입니다.

## 로컬에서 실행하기

HTML 파일을 브라우저로 바로 열어도 동작합니다. 로컬 서버로 확인하려면 다음과 같이 실행합니다.

```bash
git clone https://github.com/lshlj82/netsci-summer-school.git
cd netsci-summer-school
python3 -m http.server 8000
# 브라우저에서 http://localhost:8000 접속
```

## 구현 메모

- 그래프 안의 축 이름, 눈금(10의 거듭제곱), 주석은 아래첨자와 위첨자를 직접 조판하는 작은 렌더러로 그리고, 곡선에 가리지 않도록 테두리를 둘러 표시합니다.
- 척도 없는 네트워크는 고-강-김의 정적 모형(static model)으로 만듭니다. 노드 i에 가중치 i^(−α)를 주고, 가중치에 비례하는 확률로 고른 두 노드를 연결하는 일을 원하는 링크 수만큼 반복하면 링크수 지수 γ = 1 + 1/α인 네트워크가 됩니다. 무작위 네트워크는 링크 수를 정해 둔 G(N, L) 방식으로 만듭니다.
- 네트워크 그림은 가장 큰 연결 덩어리만 프루크터만-라인골드(Fruchterman–Reingold) 방식으로 배치합니다. 배치 계산은 화면이 멈추지 않도록 잘게 나눠서 합니다.
- 링크수 분포 그래프는 노드 2만 개짜리 네트워크를 따로 만들어 그립니다.
- 리만-제타 함수 ζ(γ)와 후르비츠-제타 함수 ζ(γ, q)는 오일러-매클로린 공식으로 계산합니다.
- 지수 측정 데모의 이산적인 거듭제곱 분포 표본은 누적분포 표에서 역변환으로 정확히 뽑고, 링크수 지수는 이산적인 로그 우도를 직접 최대화합니다. 근사식 γ = 1 + N[Σ ln(kᵢ/(K_min − 1/2))]⁻¹은 K_min이 작으면 오차가 커서, 데모에서는 비교용으로 함께 보여 줍니다.
- 적합도 검정에서는 가상 데이터마다 K_min을 고정한 채 γ를 다시 추정해 거리를 잽니다(클라우셋 등의 원래 방법은 K_min까지 다시 찾습니다).
- 실제 네트워크의 표준편차 그림은 『네트워크 사이언스』 표 4.1의 값으로 계산합니다.
- 프랙탈 데모의 시에르핀스키 삼각형은 파스칼 삼각형의 홀수 칸으로 만듭니다.

## 참고문헌

1. [네트워크 사이언스](https://www.acornpub.co.kr/product/%EB%84%A4%ED%8A%B8%EC%9B%8C%ED%81%AC-%EC%82%AC%EC%9D%B4%EC%96%B8%EC%8A%A4/5911/category/25/display/1/) (에이콘출판사, 2023), [이미진](https://scholar.google.com/citations?user=YtV_KAgAAAAJ)·[윤진혁](https://scholar.google.com/citations?user=F_tGTBYAAAAJ)·[이상훈](https://sites.google.com/view/netscilab/principal-investigator)·[이은](https://scholar.google.com/citations?user=kXggWVUAAAAJ)·[조항현](https://scholar.google.com/citations?user=EAxaIyYAAAAJ&hl=en)·[김희태](https://scholar.google.dk/citations?user=52OfnhEAAAAJ)·[손승우](https://scholar.google.com/citations?user=GUpdvGoAAAAJ) 옮김.
   * 원서: [Albert-László Barabási](https://scholar.google.com/citations?user=vsj2slIAAAAJ&hl=en), [Network Science](https://networksciencebook.com/) (Cambridge University Press, 2016).
2. [네트워크 분석](https://www.acornpub.co.kr/product/%EB%84%A4%ED%8A%B8%EC%9B%8C%ED%81%AC-%EB%B6%84%EC%84%9D/5797/category/25/display/1/) (에이콘출판사, 2022), [손승우](https://scholar.google.com/citations?user=GUpdvGoAAAAJ)·[엄영호](https://scholar.google.com/citations?user=4nirJyUAAAAJ)·[이상훈](https://sites.google.com/view/netscilab/principal-investigator)·[이은](https://scholar.google.com/citations?user=kXggWVUAAAAJ)·[김희태](https://scholar.google.dk/citations?user=52OfnhEAAAAJ)·[이미진](https://scholar.google.com/citations?user=YtV_KAgAAAAJ) 옮김.
   * 원서: [Filippo Menczer](https://scholar.google.com/citations?user=f_kGJwkAAAAJ), [Santo Fortunato](https://scholar.google.com/citations?user=NDrCCokAAAAJ), and [Clayton A. Davis](https://scholar.google.com/citations?user=oZC6UJsAAAAJ), [A First Course in Network Science](https://www.amazon.com/First-Course-Network-Science/dp/1108471137) (Cambridge University Press, 2020).
3. R. Albert, H. Jeong, and A.-L. Barabási, “[Diameter of the World-Wide Web](https://doi.org/10.1038/43601),” *Nature* **401**, 130 (1999).
4. M. P. H. Stumpf and M. A. Porter, “[Critical Truths About Power Laws](https://doi.org/10.1126/science.1216142),” *Science* **335**, 665 (2012).
5. J. Bagrow and Y.-Y. Ahn, *[Working with Network Data](https://cambridgeuniversitypress.github.io/WorkingWithNetworkData/)* (Cambridge University Press, 2024).
6. K.-I. Goh, B. Kahng, and D. Kim, “[Universal Behavior of Load Distribution in Scale-Free Networks](https://doi.org/10.1103/PhysRevLett.87.278701),” *Physical Review Letters* **87**, 278701 (2001).
7. A. Clauset, C. R. Shalizi, and M. E. J. Newman, “[Power-law distributions in empirical data](https://doi.org/10.1137/070710111),” *SIAM Review* **51**, 661–703 (2009).
8. A. D. Broido and A. Clauset, “[Scale-free networks are rare](https://www.nature.com/articles/s41467-019-08746-5),” *Nature Communications* **10**, 1017 (2019).
9. P. Holme, “[Rare and everywhere: Perspectives on scale-free networks](https://www.nature.com/articles/s41467-019-09038-8),” *Nature Communications* **10**, 1016 (2019).
10. I. Voitalov, P. van der Hoorn, R. van der Hofstad, and D. Krioukov, “[Scale-free networks well done](https://journals.aps.org/prresearch/abstract/10.1103/PhysRevResearch.1.033034),” *Physical Review Research* **1**, 033034 (2019).
11. S. A. Frank, “[The common patterns of nature](https://onlinelibrary.wiley.com/doi/full/10.1111/j.1420-9101.2009.01775.x),” *Journal of Evolutionary Biology* **22**(8), 1563–1585 (2009).
12. D. Sornette and G. Ouillon, “[Dragon-kings: Mechanisms, statistical methods and empirical evidence](https://link.springer.com/article/10.1140/epjst/e2012-01559-5),” *The European Physical Journal Special Topics* **205**, 1–26 (2012).
13. H. Jeong, S. P. Mason, A.-L. Barabási, and Z. N. Oltvai, “[Lethality and centrality in protein networks](https://doi.org/10.1038/35075138),” *Nature* **411**, 41 (2001). 목록 페이지 표지의 예시 네트워크.
14. 로그 묶기 코드: https://github.com/h2jo/log_binning

## 제작

- **내용**: [이상훈](https://sites.google.com/view/netscilab/principal-investigator) (경상국립대학교 물리학과), [2024 복잡계 여름학교](https://www.complexity.kr/?p=1268) ‘거듭제곱 법칙과 척도 없는 네트워크’ 강의자료
- **제작**: Claude Opus 5.5 (Anthropic)
