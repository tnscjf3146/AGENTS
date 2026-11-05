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
├── AGENTS.md      # AI 에이전트에게 주는 협업 원칙과 규칙
├── README.md      # 저장소 소개
├── .env.example   # 환경변수 예시 (복사해서 .env로 사용)
└── .gitignore     # .env 파일 추적 제외
```

## 파일 설명

- [AGENTS.md](#agentsmd)
- [README.md](#readmemd)
- [.env.example](#envexample)
- [.gitignore](#gitignore)

### AGENTS.md

### README.md

### .env.example

AGENTS의 env는 특별하다. 환경변수를 적용한다. 프로젝트마다 원하는 명령은 다르고, 필요한 프롬프트는 다르기에 프로젝트의 성향에 따라 env는 바뀔 예정이다.

이 AGENTS 폴더는 하나의 세션만을 위한 것이 아닌 여러 세션을 위한 협업용 문서, 즉 에이전트들의 업무 매뉴얼이다. 그렇기 때문에 이 env에는 프로젝트마다의 변수를 관리한다. 

### .gitignore

## 사용 방법

다른 프로젝트 폴더 안에 이 저장소를 클론하고, 그 프로젝트의 `.gitignore`에 `AGENTS/`를 추가해 추적하지 않게 한다.

```bash
git clone https://github.com/tnscjf3146/AGENTS
echo "AGENTS/" >> .gitignore
```

