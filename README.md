# Rookies6 TIL

사전학습 1주차-생성형 AI의 이해와 활용 1, 2 <br />
생성형 AI를 통한 프로그래밍이 작업 효율을 높여 줄 수 있지만, 코드 수정시 이해가 부족하다는 단점이 있다.<br />
NotebookLM을 이용하여 동영상 요약하거나 퀴즈를 만들어 공부하는데 이용할 수 있다.<br />
NotebookLM의 존재는 알고 있지만 음성 요약 기능의 신뢰가 부족하여 여태 활용하지 않았다, 하지만 예상 외로 효과적인 요약이 가능하여 다음 학기 복습에서 활용해보면 좋을 것 같다. <br />

1일차 <br />
Orca는 다수의 에이전트(생성형 AI)를 별개의 가상공간에서 같은 작업을 시킬 수 있다. <br />
worktree는 프로젝트에서 파생되어 에이전트를 작업시키는 별개의 공간이다. <br />

2일차 <br />
RAG는 LLM이 할루시네션 또는 신뢰 할 수 없는 출처 문제를 해결하기 위해 나온 것으로 <br />
파싱: 문자열 데이터를 프로그램이 사용 가능한 데이터로 변환시키는 것 <br />
임베딩: 데이터를 읽어 수치화 시키는 것 <br />
작동 방식은 데이터를 읽어 수치화 시키는 임베딩 과정을 통해 VectorDB에 저장함, 사용자의 질문도 마찬가지로 임베딩 과정을 통해 수치화 하고 VectorDB에서 가장 수치가 비슷한 자료를 선택하여 답을 함 <br />
모델 양자화: 숫자를 단순하게 만들어 처리하여 정확도를 줄이고 속도는 높아진다. <br />
MCP: AI가 도구를 사용할 수 있도록 하는 표준 연결 언어 <br />
git init: .git 폴더 생성 <br />
git add .: 폴더 안의 파일 스테이지에 올림 <br />
git commit -m"패치 설명": local repository에 저장 <br />
git push origin main: remote repository에 저장 <br />

3일차 <br />
antigravity와 같은 agent가 커밋, 푸쉬와 같은 명령어를 사용할 수 있게 하기 위해 github api key를 넣고 mcp를 명령어 실행 <br />
context7은 llm이 학습된 시점의 정보만 알기에 최신 라이브러리 변동 사항을 llm에 알려주기 위한 기능이다. <br />
playwright는 웹 스크래핑을 위한 도구 <br />
개요서 작성 시 어떤 스킬을 사용할 지 모를 때 vibeindex에서 만들려는 프로그램을 설명하면 맞춤 스킬들을 알려줌 <br />
개요서는 프로젝트 진행 전 프로그램의 목적 주요 기능을 간단히 설명하는 것, PRD는 프로젝트 시작 후 프로그램의 주요 기능에 필요한 기술과 요구사항을 적은 것 <br />
바이브 코딩 주의점 1. 명확한 기준 제시 2.구현 전에 공식 문서 조사하기 3. 오류 시 원인부터 분석하기 4. 난도에 따라 다른 수정 or 구현 방식을 거친다. 5. PRD는 전체 설명 각 기능 설명은 별도 파일에서 작성 <br />

//토큰 부족 시 구글 계정 변경 1. 브라우저에서 새로운 계정 로그인 2.agy에서 /logout 3. google oauth login 4. 브라우저 인증키 복사 터미널에 붙여넣기 <br />

4일차 <br />
Pydantic은 JSON 직렬화를 제공 <br />
직렬화: JSON <-> PYTHON 간단한 전환 <br />
grill-me는 안티그래비티 2.0에 속한 기술로 에이전트가 개발자에게 어떤식으로 프로그램을 진행할지 질문을 하는 방식인 기술이다. <br />
에이전트 이용 시 요구사항이 자세할수록 수정할 때 드는 토큰을 절약할 수 있다. <br />
ollama 설치하여 오프라인 상에서도 미리 받은 모델을 이용 가능 <br />

5일차 <br />
SSR(Server Side Rendering): 백엔드에서 Html 모두 작성해서 응답을 제공 받음 <br />
CSR(Client Side Rendering): 백엔드에서 데이터(json, xml)만 응답으로 제공 받음 <br />
웹 페이지에서 실시간 반영 되어야 하는 정보는 json 파일로 따로 제공받아서 모든 페이지 정보를 새로고침하는 소요를 줄인다. 부분 업데이트 진행 <br />
Reactjs - CSR <br />
Nextjs - CSR + SSR <br />
웹스크래핑 - requests, 풀링 or 파싱 - Beautifulsoup4, 둘 다 - Selenium, 데이터 분석 - Pandas, 시각화 - Seaborn, python코드와 DB 연결 데이터 저장 조회 - pymysql, <br />
파이썬에서 외부 데이터 키를 사용할 때 key가 없을 수 있기에 get을 이용하여 없으면 기본값으로 설정하게 한다. # my_dict.get('name', 'Python') <br />
CSS Selector tag 찾기 <br />
"abc" : abc 다 가져오기, "#abc" : id 가져오기, ".abc" class : 가져오기 <br />
Tag : 모든 tag. Tag1 Tag2 : tag1, tag2 가져오기, Tag1 > Tag2 : tag1의 자손인 tag2 <br />
tag[attr]  <br />
//미완 주말에 다시 작성하기 tag 파트 포함된 단어, 똑같은 단어에 따른 명령어 기록해두기<br />
