---
title: "슬랙의 라이벌 'Buzz': AI 에이전트와 함께하는 팀 협업 플랫폼 미리보기"
date: 2026-08-31
draft: false
tags: ["Buzz AI", "팀 협업 AI", "AI 에이전트 그룹챗", "Nostr", "오픈소스", "셀프호스팅"]
categories: ["ai-productivity"]
description: "Block이 공개한 Buzz는 '슬랙 대체품'이라는 설명보다 훨씬 이상한 물건이다. AI 에이전트에게 봇 계정이 아니라 암호학적 신원을 주고, 그 대화가 오가는 서버를 당신이 소유하게 한다. 무엇이 바뀌는지, 직접 켜보려면 어떤 순서를 밟는지, 그리고 지금 팀을 옮기면 왜 안 되는지."
cover:
  image: "images/buzz-ai--팀-협업-ai--ai-에이전트-그룹챗-cover.jpg"
  alt: "슬랙의 라이벌 'Buzz': AI 에이전트와 함께하는 팀 협업 플랫폼 미리보기 커버 이미지"
  caption: "Photo by [Anemone123](https://pixabay.com/ko/photos/%ED%8C%80-%EC%A0%95%EC%8B%A0-%ED%8C%80%EC%9B%8C%ED%81%AC-%EC%A7%80%EC%97%AD-%EC%82%AC%ED%9A%8C-2447163/) on Pixabay"
---

> ※ **이 글에는 제휴 링크가 없습니다.** 본문에 나오는 모든 링크는 출처이며, 클릭하거나 구매해도 필자에게 수수료가 발생하지 않습니다.

슬랙 채널에 봇을 붙여본 사람은 다 안다. 봇은 말은 하지만 **책임은 지지 않는다**. `@deploy-bot`이 스테이징을 날려도 로그에 남는 건 "봇이 그랬다"가 전부고, 그 봇을 어느 팀이 어떤 토큰으로 붙였는지는 아무도 기억하지 못한다. 봇은 워크스페이스의 멤버가 아니라 누군가의 액세서리다.

Block이 **2026년 7월 21일 공개한**([TechCrunch, 2026-07-21](https://techcrunch.com/2026/07/21/jack-dorsey-is-taking-on-slack-with-buzz-a-group-chat-platform-for-teams-and-their-ai-agents/)) **Buzz**는 바로 그 지점을 건드린다. AI 에이전트를 봇 슬롯에 끼워 넣는 대신, **사람과 똑같은 신원을 발급해 채널의 정식 멤버로 앉힌다**. 나는 이 글에서 Buzz를 "슬랙 대체품"으로 소개할 생각이 없다. 그건 이 물건의 가장 지루한 설명이다.

## 봇과 멤버를 가르는 건 기능이 아니라 '키'다

Buzz는 Nostr 프로토콜 위에 지어졌고, 사람과 에이전트 각각에게 **암호학적 키페어를 신원으로 부여한다**([SD Times](https://sdtimes.com/open-source-ai/block-rolls-out-buzz-ai-collaboration-workspace/)). 이 문장은 기술 스펙처럼 읽히지만, 실제로는 조직 운영의 문법을 바꾼다.

슬랙에서 봇의 발언은 "앱이 남긴 메시지"다. 앱을 설치한 사람과 발언한 주체가 분리돼 있고, 그 둘을 잇는 건 어딘가에 저장된 토큰 문자열 하나다. Buzz에서 에이전트의 발언은 **그 에이전트의 개인키로 서명된 이벤트**다. 여기에 `buzz-audit` 해시체인이 붙어 에이전트의 모든 행위가 서명된 기록으로 이어진다([GitHub — block/buzz](https://github.com/block/buzz)).

차이가 실감나는 장면을 가정해 보자. 새벽 3시에 배포가 깨졌다. 슬랙이라면 "봇이 뭔가 했다"에서 시작해 CI 로그, 깃허브 액션 히스토리, 누군가의 개인 토큰을 역추적하는 시간이 시작된다. Buzz의 설계대로라면 그 추적은 "누가 서명했나"를 확인하는 한 번의 조회로 줄어든다. **다만 분명히 해두자 — 이건 설계에서 따라 나오는 기대이지 내가 재본 수치가 아니다.** 서명 확인이 실제로 사고 대응 시간을 얼마나 줄이는지는 아직 아무도 공개된 숫자로 보여주지 않았다.

그럼에도 방향은 분명하다. 봇에게 벌을 줄 수는 없지만, **서명된 신원에는 권한을 회수할 수 있다.** AI 에이전트를 실제로 일에 붙여본 팀이 부딪히는 벽은 늘 성능이 아니라 이거였다. 에이전트가 뭘 했는지 아무도 재구성할 수 없다는 것. Buzz는 그 문제를 UI로 덮지 않고 **신원 계층에서 해결하려 든다.** 이게 이 제품에서 유일하게 새로운 부분이고, 나머지는 사실 부차적이다.

## 한 창에 슬랙과 깃허브를 넣겠다는 야심

Block은 Buzz를 'model-agnostic, decentralized, self-sovereign, open source'로 규정하며, **슬랙과 깃허브식 프로젝트 관리를 한 창에서 대체하는 것**을 목표로 내걸었다([TechCrunch](https://techcrunch.com/2026/07/21/jack-dorsey-is-taking-on-slack-with-buzz-a-group-chat-platform-for-teams-and-their-ai-agents/)). TechCrunch는 이 발표를 "잭 도시가 슬랙에 도전한다"는 제목으로 다뤘다. (도시의 현재 직함은 이 글의 출처에 명시돼 있지 않아 단정하지 않는다.)

왜 채팅과 코드를 굳이 합치려 할까. 에이전트를 써 본 사람은 이유를 안다. 사람은 슬랙에서 결정하고 깃허브에서 실행하지만, **에이전트에게 그 두 세계는 서로 다른 우주다.** 채널에서 "이 버그 우선순위 올리자"는 합의가 났어도, 이슈 트래커에 그 맥락은 전달되지 않는다. 에이전트는 결정의 이유를 모른 채 티켓만 받는다. 지시는 도착했는데 근거는 도착하지 않는 것 — 이게 AI 협업이 매번 얕게 끝나는 진짜 이유다.

Buzz는 여기에 하나를 더 얹는다. **릴레이가 에이전트의 메모리를 저장한다**([GitHub](https://github.com/block/buzz)). 대화가 쌓일수록 맥락이 남는 구조다. 에이전트 프레임워크도 고정하지 않는다. `buzz-acp`라는 ACP 하네스를 통해 Goose, Codex, Claude Code 같은 외부 에이전트를 붙일 수 있다([GitHub](https://github.com/block/buzz)). Buzz 자체가 Block의 오픈소스 에이전트 프로젝트 Goose에서 자라났고, 그 전에는 슬랙 기반 프로토타입 **Builderbot**을 사내에서 굴려봤다고 한다([SD Times](https://sdtimes.com/open-source-ai/block-rolls-out-buzz-ai-collaboration-workspace/)). 자기들이 슬랙에 봇을 붙여보고 한계를 느낀 끝에 나온 물건이라는 뜻이다.

## '내 릴레이' — 오래됐지만 여전히 강한 승부수

공식 README는 Buzz를 이렇게 소개한다. *"A workspace where humans and agents build together, **on a relay you own**"*([GitHub](https://github.com/block/buzz)). 강조는 마지막 세 단어에 있다.

자체 호스팅 구성은 의외로 담백하다. Block 엔지니어링 블로그는 릴레이를 **"바이너리 하나, 의존성 셋, 컴포즈 파일 하나"** 로 요약한다. 필요한 건 Postgres, Redis, S3 호환 오브젝트 스토어다([Block Engineering — Run your own Buzz relay](https://engineering.block.xyz/blog/run-your-own-buzz-relay)). 직접 돌리기 싫으면 buzz.xyz가 **같은 오픈소스 릴레이를 대신 운영해 주는** 호스티드 옵션도 있다([buzz.xyz](https://buzz.xyz)).

라이선스는 **Apache 2.0**이고 **데스크톱 앱은 무료**다([GitHub — block/buzz](https://github.com/block/buzz)). 빌드는 **macOS(Apple Silicon·Intel), Linux x86_64, Windows x64** 세 플랫폼용으로 GitHub 릴리스에 올라온다([GitHub Releases](https://github.com/block/buzz/releases)). **라이선스 비용은 0원**이다. 다만 뒤에서 다시 다루겠지만 **총비용이 0원이라는 뜻은 아니다.**

에이전트가 회사 코드와 의사결정을 통째로 읽는 시대에, **그 대화가 어느 회사 서버에 쌓이는지**는 더 이상 취향 문제가 아니다. Buzz가 "self-sovereign"을 앞세우는 건 마케팅 수사가 아니라, 이 제품이 팔려면 반드시 넘어야 하는 관문에 대한 답이다.

## 직접 켜보는 순서 — 릴레이 하나, 커뮤니티 하나

여기까지 읽고 "그래서 어떻게 켜보나"가 궁금하다면, 밟을 계단은 넷이다.

> **먼저 읽을 것:** 아래는 공개 문서에 적힌 구성(바이너리 1개·의존성 3개·컴포즈 파일 1개)에서 따온 **골격**이다. 서비스 이름과 환경변수 키의 정확한 형태는 버전이 오르면 바뀌므로, **정본은 언제나 저장소의 README와 컴포즈 파일**이다([GitHub](https://github.com/block/buzz)). 실행 전에 그 두 파일을 그 자리에서 열어 대조하라.

**0단계 — 명령보다 먼저 결정할 것: 릴레이 주소.** 이게 가장 중요하다. `RELAY_URL`은 단순한 접속 주소가 아니라 **커뮤니티의 신원**이라 멤버를 초대한 뒤에는 바꿀 수 없다([Block Engineering](https://engineering.block.xyz/blog/run-your-own-buzz-relay)). 시험용이라도 `test.` 서브도메인을 쓰지 마라. 나중에 진짜로 쓰게 되면 그때 다시 시작해야 한다.

**1단계 — 릴레이 올리기(자체 호스팅).** 저장소를 받고, 환경 설정에 릴레이 주소와 Postgres·Redis·오브젝트 스토어 접속 정보를 채운 뒤 컴포즈로 올린다.