---
title: "Salesforce Slack AI 에이전트: 업무 생산성 혁명과 활용법"
date: 2026-06-08
draft: false
tags:
  - 슬랙 AI 에이전트
  - Salesforce AI
  - Slackbot
  - AI 생산성
  - 업무 자동화
categories:
  - ai-productivity
description: "Salesforce가 2026년 1월 GA 출시한 Slackbot AI 에이전트의 핵심 기능, 요금, 한계, 그리고 실무 활용법을 구체적인 수치와 함께 정리했습니다."
cover:
  image: "images/슬랙-ai-에이전트--salesforce-ai-cover.jpg"
  alt: "Salesforce Slack AI 에이전트: 업무 생산성 혁명과 활용법 커버 이미지"
  caption: "Photo by [emkanicepic](https://pixabay.com/ko/photos/%EB%8B%A4%EB%A6%AC-%EA%B8%80%EB%A6%AC%EB%8B%88%EC%BC%80-%EB%B2%A0%EB%A5%BC%EB%A6%B0-%ED%8F%AC%EC%B8%A0%EB%8B%B4-4087894/) on Pixabay"
---

> ※ 이 글에는 제휴 마케팅 링크가 포함될 수 있으며, 구매 시 수수료를 받을 수 있습니다.

---

매일 수백 개의 Slack 메시지를 처리하면서 정작 중요한 일을 미루고 있지는 않으신가요? Salesforce는 2026년 3월, Slackbot을 단순 알림 봇에서 업무 전반을 대신 처리하는 AI 에이전트로 탈바꿈시키는 30개 신규 기능을 발표했습니다. ([techcrunch.com](https://techcrunch.com/2026/03/31/salesforce-announces-an-ai-heavy-makeover-for-slack-with-30-new-features/)) 이 글에서는 Slack AI 에이전트가 실제로 무엇을 할 수 있고, 어떤 한계가 있으며, 어느 요금제부터 의미 있게 사용할 수 있는지를 검증된 수치 중심으로 정리합니다.

---

## Slackbot이란 무엇인가

![단순 알림 봇에서 AI 에이전트로 — Slackbot의 진화 타임라인](/images/슬랙-ai-에이전트--salesforce-ai-diagram.png)
*단순 알림 봇에서 AI 에이전트로 — Slackbot의 진화 타임라인*


Slackbot은 Salesforce가 2026년 1월 13일 정식 출시(GA)한 개인 AI 에이전트입니다. ([salesforce.com](https://www.salesforce.com/news/press-releases/2026/01/13/slackbot-announcement/)) 기존 Slackbot이 자동 응답이나 키워드 알림 수준에 머물렀다면, 새 Slackbot은 이메일 초안 작성, 회의 일정 조율, 받은 편지함 요약, Salesforce CRM 데이터 업데이트까지 자연어 대화로 처리합니다.

핵심 구조는 **MCP(Model Context Protocol) 클라이언트**입니다. ([salesforce.com](https://www.salesforce.com/slack/slackbot/agent-orchestration/)) Slackbot은 Slack 마켓플레이스 2,600개 이상의 앱과 Salesforce AppExchange 6,000개 이상의 앱을 하나의 대화 인터페이스에서 연결합니다. 사용자가 별도 탭을 열거나 앱을 전환하지 않아도, Slackbot에게 "지난주 미팅에서 나온 액션 아이템 정리해줘"라고 입력하면 Slackbot이 알아서 관련 앱을 호출하고 결과를 돌려줍니다.

2026년 여름부터는 모든 신규 Salesforce 고객에게 Slack이 첫날부터 사전 프로비저닝된 상태로 제공됩니다. ([techcrunch.com](https://techcrunch.com/2026/03/31/salesforce-announces-an-ai-heavy-makeover-for-slack-with-30-new-features/)) Salesforce CRM과 Slack을 별도로 연결하는 설정 없이 즉시 AI 기능을 쓸 수 있게 되는 것입니다.

---

## 핵심 기능 6가지

### 1. 회의 자동 녹취·요약 및 액션 아이템 추출

Slackbot은 Slack 내 허들(Huddle) 또는 연동된 화상회의를 자동으로 전사(transcribe)하고, 회의가 끝나면 요약본과 액션 아이템을 참석자 전원에게 보내줍니다. ([siliconangle.com](https://siliconangle.com/2026/03/31/salesforce-transforms-slackbot-ultimate-work-assistant-30-new-ai-features/)) 회의에 늦게 들어오거나 놓친 내용이 있어도 즉시 따라잡을 수 있습니다.

**단점:** 자동 전사·요약 품질은 회의 음질과 발화 명확성에 의존합니다. 여러 사람이 동시에 발언하거나 배경 소음이 큰 환경에서는 전사 오류가 발생할 수 있으며, 이를 검증하지 않고 그대로 공유하면 잘못된 액션 아이템이 전달될 수 있습니다.

### 2. Agentforce 통합 — CRM을 대화로 제어

Agentforce와의 통합을 통해 Slack 채널에서 직접 Salesforce CRM의 영업 기회를 업데이트하거나, 고객 케이스를 담당자에게 라우팅하거나, 워크플로우를 트리거할 수 있습니다. ([salesforce.com](https://www.salesforce.com/slack/slackbot/agent-orchestration/)) 영업팀이 CRM 앱을 열지 않고도 Slack에서 "삼성전자 딜 클로징 확률 80%로 업데이트해줘"라고 입력하면 처리됩니다.

**단점:** Agentforce 연동은 Salesforce CRM을 이미 사용하는 팀에게만 실질적 가치가 있습니다. Salesforce를 쓰지 않는 조직에서는 이 핵심 기능의 상당 부분이 무의미합니다.

### 3. 데스크탑 에이전트 — Slack 밖에서도 작동

Slackbot은 Slack 앱 외부에서도 독립적으로 실행되는 데스크탑 에이전트로 작동합니다. ([thenextweb.com](https://thenextweb.com/news/slack-slackbot-30-ai-features-agentic)) 진행 중인 거래, Slack 대화 흐름, 캘린더 일정, 사용자 행동 패턴을 상시 모니터링하며 맥락 기반 제안을 제공합니다. 예를 들어 중요한 고객 미팅 30분 전에 관련 대화 스레드와 CRM 메모를 자동으로 브리핑해줄 수 있습니다.

### 4. Einstein Trust Layer — 데이터 보안 아키텍처

Slackbot의 AI 처리는 **Einstein Trust Layer** 위에서 실행됩니다. ([slack.com](https://slack.com/ai-agents)) 고객 데이터는 LLM 학습에 절대 사용되지 않으며, 모든 LLM 호스팅은 Slack의 AWS VPC(가상 사설 클라우드) 내에서 이루어집니다. 데이터가 Slack 인프라 외부로 유출되지 않는 구조입니다.

### 5. MCP 클라이언트로서의 앱 연동

Slackbot이 MCP 클라이언트로 작동한다는 것은, 단일 자연어 요청으로 여러 앱을 조율할 수 있다는 의미입니다. ([salesforce.com](https://www.salesforce.com/slack/slackbot/agent-orchestration/)) Google Calendar, Jira, GitHub, Salesforce CRM 등 연동된 앱들을 Slackbot이 오케스트레이션하여 복합적인 업무 흐름을 자동화할 수 있습니다.

### 6. 이메일·받은 편지함 요약 및 초안 작성

Slackbot은 이메일 초안 작성, 받은 편지함 요약, 회의 일정 조율을 자연어로 처리합니다. ([salesforce.com](https://www.salesforce.com/news/press-releases/2026/01/13/slackbot-announcement/)) 반복적인 이메일 작성 시간을 줄이고, 놓친 메시지를 빠르게 캐치업할 수 있습니다.

---

## 단점과 한계 — 반드시 알아야 할 4가지

### 한계 1. 폐쇄형 정원 구조 — 외부 도구 정보 접근 불가

Slack AI는 기본적으로 **Slack 내부 데이터에만 접근**합니다. ([questionbase.com](https://questionbase.com)) CRM에 저장된 고객 이력, Confluence 위키, 이메일 아카이브, Jira 티켓 같은 외부 도구의 정보는 기본 설정에서 Slackbot이 읽을 수 없습니다. 결국 조직 지식의 상당 부분이 Slackbot의 사각지대에 남게 됩니다. MCP를 통한 외부 앱 연동이 이를 일부 해결하지만, 연동 설정과 권한 관리는 IT 팀의 별도 작업이 필요합니다.

### 한계 2. 무상태(Stateless) AI — 누적 학습 없음

각 Slackbot 상호작용은 기본적으로 **무상태**입니다. ([infoq.com](https://infoq.com)) Slackbot은 팀 특유의 용어, 업무 우선순위, 반복되는 패턴을 대화가 거듭될수록 학습하지 않습니다. 오늘 "우리 팀에서 '딜클' 은 딜 클로징을 의미해"라고 알려줘도, 다음 세션에서는 다시 설명해야 할 수 있습니다. 또한 컨텍스트 윈도우 한계에 근접하면 응답 품질이 눈에 띄게 저하됩니다. ([infoq.com](https://infoq.com))

### 한계 3. 데스크탑 모니터링의 프라이버시 논란

데스크탑 에이전트가 사용자의 습관, 대화, 일정을 상시 감시하는 구조는 **직장 내 프라이버시 침해 우려**를 낳습니다. ([linkedin.com/askturing-ai](https://linkedin.com/askturing-ai)) 현재는 옵트인(opt-in) 방식이지만, 기업이 전사 정책으로 강제 활성화할 경우 직원 동의 없이 행동 패턴이 수집될 수 있다는 논란이 존재합니다. 민감한 업무를 다루는 조직이나 원격 근무자가 많은 팀은 이 기능을 도입 전 법무·HR과 반드시 검토해야 합니다.

### 한계 4. 에이전트 스프롤(AI Sprawl) 위험

팀 내 AI 에이전트가 늘어날수록 **에이전트 스프롤** 현상이 발생합니다. ([eesel.ai](https://eesel.ai)) 각 에이전트가 독립된 권한과 데이터 범위로 분리되어 운영되면, 오히려 사내 지식이 통합되지 않고 분산되는 역효과가 납니다. Slackbot, Agentforce, 외부 AI 도구가 각자의 컨텍스트 안에서만 작동하면 "AI가 많은데 왜 더 복잡해졌지?"라는 상황이 생길 수 있습니다.

---

## 요금 및 플랜 — 어느 플랜부터 제대로 쓸 수 있나

| 플랜 | 월정액 (연간) | 월정액 (월간) | Slackbot 접근 |
|------|-------------|-------------|--------------|
| Free | 무료 | 무료 | 제한 체험만 |
| Pro | $7.25/user | $8.75/user | 제한 체험만 |
| Business+ | **$15/user** | $18/user | **전체 AI 기능 포함** |
| Enterprise+ | 견적 문의 | — | 전체 AI 기능 + 고급 관리 |

 ([slack.com/pricing](https://slack.com/pricing))

**Enterprise+ 실구매 데이터:** Vendr의 2026년 실거래 데이터 기준 Enterprise+ 실제 체결 단가는 $21.95~$28.10/user/month이며, 중앙값은 $26.18/user/month입니다. ([vendr.com](https://www.vendr.com/blog/slack-pricing-what-it-costs-in-2026-real-enterprise-data))

**핵심 포인트:** Free·Pro 플랜 사용자는 Slackbot을 제한적으로 체험할 수 있을 뿐, 회의 요약·이메일 초안·CRM 연동 등 핵심 AI 기능을 지속적으로 사용하려면 **Business+ 이상**이 필요합니다. ([slack.com/pricing](https://slack.com/pricing)) 10인 팀 기준 연간 결제 시 Business+는 월 $150(≒ 약 21만 원) 수준입니다.

---

## 경쟁 도구 비교표

| 항목 | Slack AI (Slackbot) | Microsoft Copilot for Teams | Notion AI |
|------|--------------------|-----------------------------|-----------|
| 기반 플랫폼 | Slack (Salesforce) | Microsoft Teams | Notion |
| AI 에이전트 수준 | 고급 (MCP 오케스트레이션) | 고급 (Microsoft 365 연동) | 중급 (문서 중심) |
| CRM 연동 | Salesforce 네이티브 | Dynamics 365 네이티브 | 없음 |
| 외부 앱 연동 | 2,600+ (Slack 마켓플레이스) | Microsoft 365 생태계 | 제한적 |
| 데이터 보안 | Einstein Trust Layer + AWS VPC | Microsoft Purview | Notion 자체 암호화 |
| AI 포함 시작 요금 | $15/user/월 (Business+) | $30/user/월 | $10/user/월 |
| 무상태 한계 | 있음 | 있음 | 있음 |
| Salesforce 미사용 팀 적합도 | 낮음 | 보통 | 높음 |

* 표시 항목은 공개 자료 기반 추정이며 공식 출처로 검증되지 않았습니다.*

---

## 이런 팀에게 추천합니다

**강력 추천:**
- **Salesforce CRM 사용 중인 영업팀·CS팀** — Agentforce 연동으로 CRM 업무를 Slack 대화 하나로 처리할 수 있어 생산성 향상 폭이 큽니다.
- **원격·분산 팀** — 비동기 회의가 많고 회의록 관리가 어려운 팀에게 자동 요약·액션 아이템 추출은 즉각적인 가치를 제공합니다.
- **이미 Slack Business+ 사용 중인 팀** — 추가 비용 없이 AI 기능을 쓸 수 있으므로 도입 장벽이 없습니다.

**신중히 검토 필요:**
- **Salesforce를 쓰지 않는 조직** — MCP 연동 설정에 IT 리소스를 투입해야 하며, 핵심 기능의 상당 부분이 제한됩니다.
- **강력한 데이터 프라이버시 정책이 필요한 산업** — 금융·의료·법무 분야에서는 데스크탑 모니터링 기능 도입 전 반드시 컴플라이언스 검토가 선행되어야 합니다.
- **스타트업·소규모 팀** — 1인당 월 $15 이상의 비용이 부담될 수 있으며, Free·Pro 플랜으로는 AI 기능을 지속 사용할 수 없습니다.

---

## 자주 묻는 질문 (FAQ)

**Q1. Free 플랜에서도 Slackbot AI 기능을 쓸 수 있나요?**

Free·Pro 플랜은 Slackbot의 제한적인 체험만 제공합니다. ([slack.com/pricing](https://slack.com/pricing)) 회의 요약, 이메일 초안, CRM 연동 등 핵심 AI 기능을 지속적으로 사용하려면 Business+($15/user/월, 연간 결제 기준) 이상이 필요합니다. 팀 규모와 업무 형태를 고려해 체험 기간 동안 가치를 검증한 뒤 업그레이드하는 것을 권장합니다.

**Q2. Slackbot이 회사 내부 데이터를 AI 학습에 사용하나요?**

사용하지 않습니다. Einstein Trust Layer는 고객 데이터가 LLM 훈련에 활용되는 것을 명시적으로 차단하며, 모든 AI 처리는 Slack의 AWS VPC 내에서만 이루어집니다. ([slack.com/ai-agents](https://slack.com/ai-agents)) 단, 기업 내부 정책과 계약 조건을 직접 확인하는 것이 가장 안전합니다.

**Q3. Microsoft Teams를 이미 사용 중인데 Slack AI로 전환할 필요가 있나요?**

Salesforce CRM을 쓰는 팀이라면 Slack AI의 네이티브 Agentforce 연동은 강력한 차별점입니다. 반면 Microsoft 365(Outlook, SharePoint, Dynamics 365) 생태계에 깊이 묶여 있다면 Microsoft Copilot for Teams가 더 자연스러운 선택일 수 있습니다. 두 도구 모두 무상태 AI의 한계를 갖고 있으므로, 실제 업무 흐름에서 어느 쪽 연동이 더 많은 마찰을 줄여주는지를 기준으로 판단하세요.

---

## 참고 링크

- Salesforce Slackbot 공식 발표 (2026년 1월): [salesforce.com](https://www.salesforce.com/news/press-releases/2026/01/13/slackbot-announcement/)
- 30개 AI 기능 발표 (TechCrunch, 2026년 3월): [techcrunch.com](https://techcrunch.com/2026/03/31/salesforce-announces-an-ai-heavy-makeover-for-slack-with-30-new-features/)
- Slackbot MCP 에이전트 오케스트레이션: [salesforce.com](https://www.salesforce.com/slack/slackbot/agent-orchestration/)
- Slack AI 보안 아키텍처 (Einstein Trust Layer): [slack.com/ai-agents](https://slack.com/ai-agents)
- Slack 공식 요금제: [slack.com/pricing](https://slack.com/pricing)
- Enterprise+ 실구매 단가 데이터 (Vendr 2026): [vendr.com](https://www.vendr.com/blog/slack-pricing-what-it-costs-in-2026-real-enterprise-data)
- Slackbot 30개 기능 심층 분석 (SiliconAngle): [siliconangle.com](https://siliconangle.com/2026/03/31/salesforce-transforms-slackbot-ultimate-work-assistant-30-new-ai-features/)
- Slackbot 데스크탑 에이전트 (The Next Web): [thenextweb.com](https://thenextweb.com/news/slack-slackbot-30-ai-features-agentic)