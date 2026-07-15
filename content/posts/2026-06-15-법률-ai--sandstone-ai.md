---
title: "법률 전문가를 위한 AI 도구: Sandstone AI 솔루션 분석"
date: 2026-06-15
draft: false
tags:
  - 법률 AI
  - Sandstone AI
  - 인하우스 법무팀
  - AI 자동화
  - 법률 테크
categories:
  - ai-productivity
description: "2026년 가장 빠르게 성장하는 법률 AI 스타트업 Sandstone AI를 분석합니다. $30M 시리즈 A 유치, 인하우스 법무팀 특화 기능, 단점과 한계까지 솔직하게 정리합니다."
cover:
  image: "images/법률-ai--sandstone-ai-cover.jpg"
  alt: "법률 전문가를 위한 AI 도구: Sandstone AI 솔루션 분석 커버 이미지"
  caption: "Photo by [geralt](https://pixabay.com/ko/photos/%EC%A0%95%EB%8B%B9%EC%84%B1-%EC%B2%9C%EC%B9%AD-%EC%86%8C%EC%9C%A0-%EC%88%98-%EA%B0%91-3222265/) on Pixabay"
---

> ※ 이 글에는 제휴 마케팅 링크가 포함될 수 있으며, 구매 시 수수료를 받을 수 있습니다.

기업 법무팀의 하루는 끝없는 계약서 검토, 이메일 요청 처리, 리스크 판단으로 가득 차 있습니다. 2026년 들어 이 반복 업무를 AI 에이전트에게 위임하는 움직임이 본격화되고 있으며, 그 중심에 Sandstone AI가 있습니다. Sequoia Capital과 Lightspeed Venture Partners 양사 모두의 투자를 받은 이 스타트업이 인하우스 법무팀의 일하는 방식을 어떻게 재정의하고 있는지, 그리고 어떤 한계가 있는지 살펴봅니다.

---

## Sandstone AI란 무엇인가

![시드 $10M 출시 → 90일 만에 매출 40배 → 시리즈 A $30M: 법률 AI 시장의 이례적 트랙션](/images/법률-ai--sandstone-ai-diagram.png)
*시드 $10M 출시 → 90일 만에 매출 40배 → 시리즈 A $30M: 법률 AI 시장의 이례적 트랙션*


Sandstone AI는 기업 내부 법무팀(인하우스 리걸팀)을 전담하는 AI 에이전트 플랫폼입니다. 2026년 1월 Sequoia Capital 주도의 $10M 시드 라운드와 함께 공식 출시([출처](https://www.artificiallawyer.com/2026/01/13/sandstone-raises-10m-seed-led-by-sequoia-for-inhouse-ai-agents/))되었으며, 불과 6개월 만인 2026년 6월 Lightspeed Venture Partners 주도의 $30M 시리즈 A를 유치([출처](https://techcrunch.com/2026/06/09/sandstone-raises-30m-to-bring-ai-to-in-house-legal-teams/))했습니다.

공동 창업자는 McKinsey 법률 테크 부문 출신의 Nick Fleisher와 기업 내부 변호사(in-house attorney) 경력의 Jarryd Strydom([출처](https://www.artificiallawyer.com/2026/01/13/sandstone-raises-10m-seed-led-by-sequoia-for-inhouse-ai-agents/))입니다. 두 창업자의 배경이 말해주듯, Sandstone은 법률 테크를 외부에서 바라보는 시각이 아니라 실제 법무팀이 겪는 병목을 직접 경험한 사람들이 설계한 도구입니다.

Lightspeed는 이 플랫폼을 **"인하우스 리걸을 위한 운영 체제(the operating system for in-house legal)"**([출처](https://lsvp.com/stories/the-operating-system-for-in-house-legal-our-series-a-in-sandstone/))로 정의했습니다. 단순한 계약서 검토 도구가 아니라, 법무팀이 처리하는 모든 워크플로우의 인테이크·컨텍스트·실행을 하나로 통합하는 플랫폼이라는 의미입니다.

---

## 핵심 기능 상세 분석

### 1. AI 인테이크 자동화 — 요청이 발생하는 원점에서 캡처

법무팀이 가장 많이 받는 요청은 이메일, Slack 메시지, Jira 티켓 등 다양한 채널을 통해 들어옵니다. Sandstone은 이 요청들을 팀이 이미 사용 중인 툴(Slack, Microsoft Teams, 이메일, Salesforce, Jira)에서 직접 캡처합니다([출처](https://lsvp.com/stories/the-operating-system-for-in-house-legal-our-series-a-in-sandstone/)). 즉, 별도의 포털이나 시스템으로 이동할 필요 없이 업무 요청이 발생하는 원점에서 자동으로 인테이크가 시작됩니다.

인테이크된 요청은 AI가 자동으로 업무 유형(NDA, 벤더 계약 검토, 고용 계약 등)을 분류하고 적절한 워크플로우로 배정합니다. 법무팀 담당자가 직접 분류하고 배정하는 수작업이 사라지며, 비즈니스 이해관계자(법무팀 외부 임직원)는 Slack이나 Teams에서 직접 AI 에이전트와 대화하며 법무 요청을 제출하고 진행 상태를 확인할 수 있는 셀프서비스 인테이크를 활용할 수 있습니다.

**이 기능의 한계:**
- 자동 분류 정확도는 팀의 과거 데이터 양과 품질에 의존합니다. 신규 법무팀이거나 히스토리 데이터가 적은 경우 초기 분류 오류 발생 가능성이 있습니다.
- Slack·Jira 같은 특정 도구에 의존하므로, 해당 툴을 사용하지 않는 팀에서는 인테이크 자동화의 혜택이 제한적입니다.

### 2. AI 기반 계약서 초안 작성 및 레드라이닝

Sandstone의 핵심 차별점 중 하나는 플레이북(playbook)을 처음부터 새로 작성하지 않는다는 점입니다. 대신 팀이 실제로 협상하며 작성한 레드라인 계약서를 수집하여 AI 플레이북을 구축합니다([출처](https://thelegalwire.ai/what-sandstone-reveals-about-the-ai-native-legal-department/)). 팀 고유의 협상 성향과 리스크 허용 기준이 자동으로 인코딩된다는 의미입니다.

계약서 초안을 작성하거나 상대방 초안을 검토할 때, AI는 팀의 실제 협상 패턴에 기반해 리스크 조항을 식별하고 대안 문구를 제안합니다. 이론적 베스트 프랙티스가 아닌 "우리 팀이 실제로 수용해온 기준"을 반영한다는 것이 핵심입니다.

**이 기능의 한계:**
- 과거 계약서 데이터가 부족하거나 표준화되지 않은 경우 플레이북 품질이 저하될 수 있습니다. 역사가 짧은 법무팀이나 계약서 형식이 제각각인 경우 플레이북 구축에 상당한 초기 셋업 비용이 발생할 수 있습니다.
- AI가 생성한 모든 초안과 레드라인은 반드시 변호사의 검토를 거쳐야 합니다. 플랫폼 자체적으로 최종 법적 판단을 내리지 않으며, AI 출력물은 명시적으로 초안 단계로 취급됩니다([출처](https://thelegalwire.ai/what-sandstone-reveals-about-the-ai-native-legal-department/)). 완전 자동화를 기대하는 팀에게는 실망스러울 수 있습니다.

### 3. 자기학습형 에이전틱 워크플로우

Sandstone의 에이전트는 고정된 템플릿이 아닙니다. 각 상호작용을 통해 지속적으로 학습하며 팀의 패턴을 업데이트합니다. 시간이 지날수록 팀에 더 특화된 지원이 가능해지는 구조입니다. 처음 도입했을 때보다 6개월, 1년 후에 더 정확한 분류와 더 적절한 문구 제안이 이루어진다는 것이 장기 사용자에게 유리한 요소입니다.

### 4. 통합 법률 컨텍스트 레이어

Sandstone은 모든 결정, 문서, 비즈니스 관계에 걸쳐 통합된 법률 컨텍스트를 유지합니다([출처](https://lsvp.com/stories/the-operating-system-for-in-house-legal-our-series-a-in-sandstone/)). 특정 벤더와의 계약 이력, 협상 결과, 수정 사항이 하나의 컨텍스트로 누적됩니다. 담당자가 교체되더라도 조직의 법률 지식이 손실되지 않는다는 점은 이직률이 높은 법무 조직에서 특히 가치 있는 기능입니다.

### 5. 운영 메트릭 대시보드

법무팀의 생산성을 가시화하는 기능입니다. 사이클 타임(요청 접수부터 완료까지 소요 시간), 자동 해결율, 워크로드 및 용량 벤치마킹 등의 지표를 제공합니다. CFO나 CEO에게 법무팀의 ROI를 설명해야 하는 법무책임자(General Counsel)에게 유용한 데이터를 제공합니다. "법무팀이 얼마나 기여하고 있는가"를 숫자로 증명해야 하는 상황에서 강력한 도구가 됩니다.

---

## 실제 도입 사례와 성장 지표

Sandstone의 현재 고객사에는 Wayfair, Grindr, Mercury, Cox Media, ElevenLabs([출처](https://www.artificiallawyer.com/2026/06/09/sandstone-raises-30m-for-ai-native-inhouse-teams/))가 포함되어 있습니다. 전자상거래 대기업부터 핀테크, 미디어, AI 스타트업까지 다양한 업종의 인하우스 법무팀이 채택한 것을 확인할 수 있습니다.

가장 주목할 만한 성장 지표는 **90일 만에 매출 40배 성장**([출처](https://techcrunch.com/2026/06/09/sandstone-raises-30m-to-bring-ai-to-in-house-legal-teams/))입니다. 시드 라운드 직후 6개월 이내에 이 수치를 달성한 것은 법률 AI 시장에서 이례적인 트랙션으로 평가됩니다. 단, 절대적인 매출 규모는 공개되지 않았으며, 40배라는 성장률은 초기 베이스가 낮을 때 발생하기 쉬운 지표라는 점을 함께 고려해야 합니다.

---

## 단점 및 한계 — 도입 전 반드시 확인하세요

아무리 혁신적인 도구라도 한계는 있습니다. Sandstone AI를 도입하기 전에 반드시 고려해야 할 핵심 제약 사항을 구체적으로 정리합니다.

### 한계 1: 인하우스 법무팀 전용 — 로펌·개인 변호사 사용 불가

Sandstone은 명시적으로 기업 내부 법무팀만을 대상으로 설계되어 있습니다. 외부 로펌, 법률 사무소, 개인 개업 변호사는 이 플랫폼의 설계 대상이 아닙니다. 법률 AI 시장의 상당 부분을 차지하는 로펌 세그먼트에는 접근조차 할 수 없다는 점은 Sandstone의 잠재 시장 규모를 제한하는 요소이기도 합니다([출처](https://thelegalwire.ai/what-sandstone-reveals-about-the-ai-native-legal-department/)).

실무적으로 보면, 규모가 작은 스타트업의 법무팀이나 외부 법률 자문에 주로 의존하는 기업도 이 플랫폼의 혜택을 받기 어렵습니다. 내부 법무팀이 존재하고 어느 정도 규모가 있어야 플랫폼이 효과를 발휘합니다. 1~2인 법무팀의 경우 도입 비용 대비 효과가 낮을 가능성이 있습니다.

### 한계 2: AI 출력물은 초안 — 완전 자율 실행 불가

Sandstone의 모든 AI 출력물은 명시적으로 사람의 검토를 필요로 하는 초안으로 취급됩니다([출처](https://thelegalwire.ai/what-sandstone-reveals-about-the-ai-native-legal-department/)). 최종 리스크 평가와 전략적 결정은 반드시 변호사가 내려야 합니다. AI가 계약서를 완성하고 자동 서명까지 진행하는 완전 자율화 단계는 현재 지원하지 않습니다.

이는 법적 책임 구조상 피할 수 없는 현실이기도 하지만, "AI가 법무 업무를 다 해준다"는 기대를 갖고 도입하면 실망할 수 있습니다. 반복 업무의 속도와 품질을 높여주는 효율화 도구이지, 사람 변호사를 대체하는 것은 아닙니다.

### 한계 3: 초기 스타트업 리스크 — 경쟁 환경 불확실성

Sandstone은 2026년 1월에 공식 출시된 매우 초기 단계의 회사입니다([출처](https://www.artificiallawyer.com/2026/01/13/sandstone-raises-10m-seed-led-by-sequoia-for-inhouse-ai-agents/)). Anthropic Claude for Legal처럼 프런티어 AI 제공사들이 법률 워크플로우에 직접 진입하는 경쟁 압력에 노출되어 있습니다. 대형 AI 기업들이 법률 특화 기능을 무기화할 경우 스타트업으로서의 차별점이 흔들릴 수 있다는 점은 장기 도입 시 고려해야 할 리스크입니다. 엔터프라이즈 계약에서는 벤더 안정성이 중요한 판단 기준이 됩니다.

### 한계 4: 공개 가격 없음 — 소규모 팀의 접근성 장벽

가격 정보가 전혀 공개되지 않습니다([출처](https://sandstone.com/)). 도입을 검토하려면 반드시 영업 데모를 신청하고 별도 견적을 받아야 합니다. 비용을 미리 파악하지 못한 채 영업 프로세스를 진행해야 하므로, 예산 확인이 우선인 소규모 팀에게는 진입 장벽이 됩니다. 특히 IT·법무·재무 부서가 협의해서 도구를 선택하는 조직에서는 가격 투명성의 부재가 의사결정을 지연시킬 수 있습니다.

---

## 요금 및 가격 정보

| 플랜 | 가격 | 접근 방법 |
|------|------|---------|
| Enterprise | 견적 문의 필요 | [sandstone.com](https://sandstone.com/) 데모 신청 |

Sandstone AI는 현재 모든 고객에게 엔터프라이즈 세일즈 모델을 적용합니다. 공식 웹사이트([sandstone.com](https://sandstone.com/))에서 데모를 신청하면 영업팀과 연결되며, 팀 규모와 사용 범위에 따라 맞춤 견적을 제공받는 방식입니다. 공개된 가격 구간은 존재하지 않습니다([출처](https://sandstone.com/)).

참고로 법률 AI 경쟁사들의 가격 정보는 다음과 같습니다:

- **Harvey AI**: 공개 가격 없음, 엔터프라이즈 전용
- **Thomson Reuters CoCounsel**: 구독 기반, 정확한 가격은 견적 문의 필요
- **Microsoft 365 Copilot** (법률팀 포함): 사용자당 월 $30 — 단, 법률 특화 기능은 제한적이며 범용 생산성 도구에 해당

*위 경쟁사 가격 정보는 공개 검색 기반 추정치로, 변경 가능성이 있으며 반드시 각 업체에 직접 확인이 필요합니다.*

---

## 경쟁 도구 비교표

| 항목 | Sandstone AI | Harvey AI | Microsoft Copilot (Legal) | Thomson Reuters CoCounsel |
|------|-------------|-----------|--------------------------|--------------------------|
| **주요 대상** | 인하우스 법무팀 | 로펌·인하우스 | 전사 포함 | 법률 리서치 중심 |
| **통합 채널** | Slack, Teams, Salesforce, Jira, Email | 자체 인터페이스 중심 | Microsoft 생태계 | 자체 포털 |
| **플레이북 자동 학습** | 실제 레드라인 계약 기반 | 없음 | 없음 | 없음 |
| **인테이크 자동화** | 있음 (원점 캡처) | 제한적 | 제한적 | 없음 |
| **운영 메트릭 대시보드** | 있음 | 불명확 | 없음 | 없음 |
| **공개 가격** | 없음 | 없음 | $30/사용자/월 | 없음 |
| **완전 자율 실행** | 없음 (초안+사람 검토) | 없음 | 없음 | 없음 |
| **출시 시기** | 2026년 1월 | 2022년 | — | 수십 년 |

* 표시 항목은 공개 정보 기반 추정치로, 각 업체에 직접 확인을 권장합니다.*

---

## 추천 대상

**Sandstone AI가 적합한 팀:**
- 중견~대기업의 내부 법무팀으로, 이메일·Slack·Jira로 들어오는 요청을 수동으로 처리하는 데 병목을 겪고 있는 경우
- 벤더 계약, NDA, 고용 계약 등 반복적인 계약 유형이 많고, 협상 패턴이 이미 어느 정도 누적되어 있는 팀
- General Counsel 또는 법무팀장이 팀의 생산성과 ROI를 정량적으로 경영진에게 보여줘야 하는 상황
- Slack/Teams/Salesforce/Jira를 이미 핵심 업무 도구로 사용 중인 조직
- 담당자 이직이나 지식 손실 문제를 구조적으로 해결하고 싶은 법무팀

**Sandstone AI가 적합하지 않은 경우:**
- 외부 로펌 또는 개인 법률 사무소 — 설계 자체가 인하우스 전용
- 내부 법무팀이 없는 초기 스타트업 — 도입 효과를 기대하기 어려움
- 가격을 사전에 확인한 뒤 도입 여부를 결정하고 싶은 소규모 팀 — 공개 가격 없음
- AI가 법무 업무를 완전 자율로 처리해주길 기대하는 경우 — 현재 기술 수준은 "초안+사람 검토" 구조

---

## 자주 묻는 질문 (FAQ)

**Q1. Sandstone AI는 어떤 언어의 계약서를 지원하나요?**

현재 공식 발표된 고객사는 미국 기반 기업들이며, 공개된 지원 언어 목록은 영어 중심입니다. 글로벌 기업의 경우 다국어 계약서 처리 가능 여부를 데모 신청 시 별도로 확인해야 합니다. 최신 지원 언어 정보는 공식 사이트([sandstone.com](https://sandstone.com/))에서 직접 문의하는 것이 가장 정확합니다.

**Q2. 기존 계약 관리 시스템(CLM)과 연동이 가능한가요?**

Sandstone은 Slack, Microsoft Teams, Salesforce, Jira, 이메일과의 통합을 공식 지원합니다([출처](https://lsvp.com/stories/the-operating-system-for-in-house-legal-our-series-a-in-sandstone/)). DocuSign, Ironclad, Icertis 같은 전문 CLM 시스템과의 통합 여부는 공개 정보에서 확인되지 않았습니다. 기존 CLM과의 연동이 중요한 조건이라면 데모 신청 시 반드시 이 점을 명시하고 확인을 요청하세요.

**Q3. 데이터 보안과 기밀 유지는 어떻게 보장되나요?**

법률 데이터는 극도로 민감한 특성을 가집니다. Sandstone이 Wayfair, Grindr 등 공개 기업의 인하우스 법무팀([출처](https://www.artificiallawyer.com/2026/06/09/sandstone-raises-30m-for-ai-native-inhouse-teams/))을 고객으로 유치한 것을 보면 기본적인 엔터프라이즈 보안 요건은 충족하는 것으로 추정됩니다. 그러나 SOC 2 인증 여부, 데이터 거주(data residency) 옵션, AI 모델 훈련에 고객 데이터 사용 여부 등 구체적인 보안 정책은 현재 공개 정보에서 확인되지 않았습니다. 도입 전 반드시 데모와 계약 협상 단계에서 상세한 데이터 처리 방침 문서를 요청하고 법무팀 내부에서 검토하세요.

---

## 결론: 2026년 법률 AI의 새로운 기준점

Sandstone AI는 "법률 AI 도구"라는 카테고리를 새롭게 정의하고 있습니다. 단순히 계약서를 분석해주는 도구가 아니라, 법무팀이 업무를 접수하고 분류하고 처리하고 측정하는 전체 운영 체계를 AI로 재구축하는 접근입니다.

90일 40배 매출 성장([출처](https://techcrunch.com/2026/06/09/sandstone-raises-30m-to-bring-ai-to-in-house-legal-teams/))이라는 수치는 시장의 수요가 실재함을 보여줍니다. 하지만 인하우스 법무팀 전용이라는 제약, 공개 가격 부재, 초기 스타트업 리스크, 그리고 AI 출력물에 반드시 사람의 검토가 필요하다는 구조적 한계는 무시할 수 없는 고려 요소입니다.

법무팀의 반복 업무를 줄이고 전략적 가치를 높이려는 General Counsel에게는 가장 먼저 데모를 신청해볼 만한 도구입니다. 단, 이 도구가 변호사의 판단을 대신하는 것이 아니라 더 나은 판단을 더 빠르게 내릴 수 있도록 지원한다는 관점으로 접근해야 합니다. 법적 판단의 최종 책임은 여전히 사람에게 있습니다.

---

## 참고 링크

- [Sandstone AI 공식 사이트 — 데모 신청](https://sandstone.com/)
- [시드 라운드 발표 — Artificial Lawyer (2026-01-13)](https://www.artificiallawyer.com/2026/01/13/sandstone-raises-10m-seed-led-by-sequoia-for-inhouse-ai-agents/)
- [시리즈 A 발표 — TechCrunch (2026-06-09)](https://techcrunch.com/2026/06/09/sandstone-raises-30m-to-bring-ai-to-in-house-legal-teams/)
- [Lightspeed 투자 논거 — LSVP](https://lsvp.com/stories/the-operating-system-for-in-house-legal-our-series-a-in-sandstone/)
- [Artificial Lawyer — 시리즈 A 심층 분석 (2026-06-09)](https://www.artificiallawyer.com/2026/06/09/sandstone-raises-30m-for-ai-native-inhouse-teams/)
- [The Legal Wire — AI 네이티브 법무팀 인사이트](https://thelegalwire.ai/what-sandstone-reveals-about-the-ai-native-legal-department/)