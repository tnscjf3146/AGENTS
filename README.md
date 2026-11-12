# AGENTS

AGENTS 깃은 발전해 가는 대(大) AI 시대, 프롬프트 엔지니어링을 위한 프롬프트의 모음이다.

상황에 맞게 추천 및 해결책을 알아서 잘 딱 깔끔하고 센스 있게 만들 수 있게 하기 위한,
나의 AI 툴에게 쥐여 주는 나와 의사소통하는 기본적인 원칙이자 규칙이다.

## 만든 이유

[꾸기(얌얌이) 글](https://teamyumyum.github.io/posts/ste-writing-rules/), 이 글을 읽고 시작되었다.

프롬프팅을 통해 에이전트에게 컨벤션을 주고,  
에이전트와 소통하려는 자세가 준비되어야 에이전트는 소통을 한다는 점을 깨닫게 되었으며,  
프롬프트 엔지니어링, 즉 AI 활용 능력을 높이기 위함이다.

## 목록

- [폴더 구조](#폴더-구조)
- [사용 방법](#사용-방법)

## 폴더 구조

```
AGENTS/
├── AGENTS.md              # AI 에이전트가 읽는 진입점. 언제 어떤 컨벤션을 볼지 알려 준다
├── README.md              # 저장소 소개
└── conventions/
    ├── writing.md         # 문서 쓰기 컨벤션 (WC1~WC16)
    └── hooks.md           # 훅 컨벤션 (HK1~HK16)
```

## 파일 설명

- [AGENTS.md](#agentsmd)
- [README.md](#readmemd)

### AGENTS.md

AI가 매 세션 읽는 진입점이다. 규칙 전문은 담지 않고, 답변·보고·문서를 쓸 때 `conventions/writing.md`를 보러 가게 한다.

문서 쓰기 컨벤션의 핵심은 다음과 같다. 답변, 보고, 문서에 적용하고, 코드와 결정 기록에는 적용하지 않는다.

- 첫 문장에 결론을 쓰고, 문단으로 잇는다. 목록, 절 제목, 표는 꼭 필요할 때만 쓴다.
- 한 문장에는 판단 하나만 쓴다. 주어와 조사를 빼지 않고, 20어절을 넘기지 않는다.
- 낯선 용어는 처음 쓸 때 설명한다. 다른 문서를 가리킬 때는 요지를 함께 쓴다.

### README.md

## 사용 방법

다른 프로젝트 폴더 안에 이 저장소를 클론하고, 그 프로젝트의 `.gitignore`에 `AGENTS/`를 추가해 추적하지 않게 한다.

```bash
git clone https://github.com/tnscjf3146/AGENTS
echo "AGENTS/" >> .gitignore
```

이 폴더는 여러 프로젝트가 같이 쓰는 공용 매뉴얼이라 프로젝트 정보는 여기에 적지 않는다.
프로젝트 루트는 아래처럼 구성한다.

```
프로젝트/
├── AGENTS.md      # 프로젝트 정보 (커밋한다)
├── CLAUDE.md      # @AGENTS.md 한 줄 (Claude Code용)
├── .gitignore     # AGENTS/ 추가
└── AGENTS/        # 이 공용 매뉴얼 (커밋하지 않는다)
```

루트 `AGENTS.md`는 아래 형식으로 쓴다. 값은 공용 매뉴얼의 문서 파일 이름과 같게 쓴다.

```markdown
# 프로젝트 이름
공용 매뉴얼은 @AGENTS/AGENTS.md 를 읽는다.
공용 매뉴얼은 구성원의 특징, 특성에 따라 달라지기 마련이다. 루트 AGENTS.md의 우선순위가 먼저다. 내용이 다르면 루트 AGENTS.md를 따른다.

## 우선순위
- 루트 AGENTS.md > 공용 매뉴얼 순서다.

## 프로젝트 정보
- STACK: react, spring
- ROLE: planner, designer, frontend, backend
- TOOLS: jira, notion
- ASSETS: figma
```

- 프로젝트 정보는 루트 `AGENTS.md`에 적는다.
- 우선순위는 루트 `AGENTS.md` > 공용 매뉴얼 순서다.

