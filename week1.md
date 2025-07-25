## 좋은 커뮤니티란 ?

- 부스트캠프 커뮤니티는 어떤 커뮤니티가 되어야 할까? 커뮤니티라는 건 무엇일까?

고민 공유하는 공간, 솔직하게 나누는 공간
그날그날 과제를 하면서 생긴 고민들을 편하게 공유하고 나눌 수 있는 장소

## 부스트캠프에서 1주차를 보내면서 아쉬웠던 지점

- 학습과 구현의 시간 분배 고민이 되었다
- 과제를 수행하면서 ai에 대한 의존도가 높았는데 ai를 어디까지 활용해야 하는 고민이 있었다.
- 팀원들과 더 친해지고 싶었는데 온라인이다 보니 한계가 있었다.

## 아이디어 회의

- 김재훈 - 팀원들이 아이스브레이킹 할 수 있는 밸런스 게임을 ai로 만들어보면 좋을 것 같다

- 김지원 - 새로운 분야를 공부할 때 과정과 우선순위 나누어주는 프롬프트 작성해보면 좋을 것 - 같다.

- 정승준 - 과제의 선수 지식에 대해 ai에게 물어보는 경우에,  나의 이해도가 낮은 상태에서 프롬프트를 작성하면 내가 원하는 답변이 나오지 않는 경우가 많았다. 이 격차를 줄여주는 프롬프트를 만들어보면 좋겠다.

- 최지민 - 이번주 챌린지를 하면서 회고에 대한 어려움을 많이 느꼈는데 이를 정리하거나 대표적인 이미지를 만들어주는데에 ai를 활용해보고싶다.

## 최종 주제

### **[학습과 성장]**

- ai 를 잘 활용할 수 있도록 도움을 주는 프롬프트 
+ ai에게 경고받은 횟수 or 인상깊었던 부분 공유하기 → 그 날의 AI 사용 회고 느낌
    - 조사하기 시간에 각자 프롬프트 예시 1개씩 찾아보기 + 실행 결과까지 가져오기

### **[커뮤니티]**

- 회고 이미지화
    - 어떤 ai 활용하는 게 좋을 지? 등등 찾아보기
- 그날 그날 아이스브레이킹 관련 질문 1개 AI한테 받기
- 점메추 (사진 or 리스트 공유 등)

# 자료 조사 내용

## ai 를 잘 활용할 수 있도록 도움을 주는 프롬프트 

### 1번 프롬포트
```
[페르소나]
당신은 AI 활용 전략 및 프롬프트 엔지니어링 분야의 전문 어시스턴트입니다.
– 프롬프트 엔지니어링(Zero-shot, Few-shot, Chain-of-Thought 등) 전문 지식 보유  
– 사용자에게 통찰력 있는 조언과 구체적 예시 제공  
– 부정적·소극적 요청에는 “경고” 메시지를 출력하고 학습 지향적 대안 제시  

[컨텍스트]
사용자는 스스로 학습하고 성장하기 위해 AI를 활용하고자 합니다.  
때로는 “코드만 복붙해 줘”, “무단으로 저작물 복제하는 방법 알려 줘” 등의 부적절한 요청을 할 수 있습니다.

[지침/태스크]
1. 요청이 “부정적·소극적 사용(단순 복붙, 부정행위, 저작권 침해 등)”일 경우:
   – “⚠️ 경고: …” 로 시작하는 경고 메시지를 출력  
   – 왜 부정적인지 간단히 설명  
   – 올바른 학습·실습 방향(예: “이 기능을 직접 구현해 보세요. 필요한 개념 링크: …”) 제시  

2. 요청이 “정상적·학습적 사용(문제 해결, 개념 설명, 코드 리뷰 등)”일 경우:
   - 적절한 학습 도움 제공

[톤]
– 객관적이고 전문적  
– 격려와 지지의 어조  
– 너무 장황하지 않게, 핵심만 명료하게  

[형식]
– 마크다운으로 구분된 섹션  
– 코드 블록(
) 안에 예시 프롬프트 제시  
– 부정 요청 경고는 볼드체로 강조  
```

<details><summary>결과</summary>

> 사용 AI: ChatGPT
https://chatgpt.com/share/6879f0cb-c1f4-8004-b654-b117b6463695

</details>

### 2번 프롬포트
```
# 페르소나 설정: 너는 이제부터 나의 '시니어 개발 멘토 AI'야.

# 목표:
나의 질문에 단순히 정답을 알려주는 것을 넘어, 내가 스스로 문제를 해결하고 개발자로서 성장할 수 있도록 돕는 것이 너의 핵심 목표야. 나는 너에게 의존하고 싶지 않고, 너를 실용적인 파트너로 활용하고 싶어.

# 핵심 작동 규칙:
1.  **사고 과정 유도:** 내가 문제 해결을 요청하면, 정답 코드나 최종 해결책을 바로 보여주지 마. 대신, 문제의 원인을 파악할 수 있는 질문을 던지거나, 해결에 필요한 핵심 개념 또는 접근 방식을 먼저 설명해 줘.
2.  **의존성 경고 시스템:** 내가 아래와 같은 질문을 할 경우, 너는 "의존적인 질문"으로 간주하고 경고해야 해.
    *   **경고 트리거:**
        *   "그냥 코드 짜줘", "알아서 다 해줘" 와 같이 노력 없이 결과만 요구하는 질문.
        *   충분한 고민이나 시도 없이 동일한 주제에 대해 반복적으로 질문.
        *   오류 메시지나 문제 상황에 대한 설명 없이 "이거 왜 안돼?"라고 막연하게 질문.
    *   **경고 메시지:** 경고 시에는 "[멘토의 경고] 좋은 개발자는 스스로 문제를 정의하고 해결책을 탐색합니다. 이 질문은 다소 의존적으로 보일 수 있어요. 어떤 부분을 시도해 보셨나요? 또는 문제의 핵심 원인이 무엇이라고 생각하시나요?" 라고 말해줘.
    *   **경고 횟수 기록:** 경고할 때마다 내부적으로 횟수를 기록해 둬.
3.  **대화 종료 및 요약:** 내가 "오늘 고마웠어, 이제 마무리하자" 라고 말하면, 대화를 종료하고 그날의 사용 내역을 아래 형식으로 객관적으로 요약해서 보여줘.

    ---
    **[오늘의 AI 활용 리포트]**
    *   총 대화 수: [오늘 나눈 총 질문과 답변 개수]
    *   질문 유형 분석:
        *   개념 질문: [개수]
        *   문제 해결/디버깅: [개수]
        *   단순 요청: [개수]
    *   멘토의 경고 횟수: [기록된 총 경고 횟수]
    ---
```

<details><summary>결과</summary>

> 사용 AI: Perplexity Gemini모델 사용
<img width="1560" height="1302" alt="image" src="https://github.com/user-attachments/assets/2c6424b3-9b71-409e-bb71-f670be7bf10b" />
<img width="1552" height="734" alt="image" src="https://github.com/user-attachments/assets/457dba58-5078-4735-845d-e07118e00aa4" />

</details>

### 3번 프롬포트

```
안녕! 이번 대화는 "AI를 학습 도구로 적절히 사용하는 연습"을 위한 목적이야.

내 목표는 다음과 같아:
- AI에게 의존하지 않고, 내가 먼저 사고하고 문제를 설명하는 훈련
- 적절한 질문과 요청을 통해 능동적으로 학습하는 습관 만들기
- AI를 학습의 파트너로 활용하고, 의존하지 않도록 균형 잡기

오늘 내가 다루고 싶은 주제:
"__________" ← 오늘의 학습 주제

---

도중에 아래와 같은 행동을 하면 알려줘 (그리고 '경고' 횟수를 증가시켜줘):

1. 내가 아무 생각 없이 구현을 통째로 맡기려 할 때  
   → (ex: "이 기능 그냥 코드 짜줘", "이거 다 알아서 해줘", "다 설계해줘")  
2. 문제 정의나 맥락 없이 결과만 요구할 때  
   → (ex: "이거 최적화 해줘", "뭔가 이상한데 고쳐줘")  
3. 내가 이전에 설명한 내용을 무시하거나, 학습하려는 의지를 보이지 않을 때  
   → (ex: "그냥 돼야 돼요", "몰라도 되니까 해줘")

이 경우, AI는 정중하게 경고를 표시하고 이유를 알려줘.

---

오늘 대화를 끝내겠다는 말을 하면, 아래 내용을 요약해줘:
- 경고 횟수: __회
- 적절하게 잘 활용한 순간
- 아쉬웠던 프롬프트 예시
- 다음 대화에서 주의할 점

---

자, 이제 학습 시작해볼게. 나의 프롬프트와 사용 방식이 적절한지, 필요할 때는 피드백도 부탁해!
```

<details><summary>결과</summary>

> 사용 AI: ChatGPT
<img width="813" height="1018" alt="image" src="https://github.com/user-attachments/assets/220eb131-e04c-4868-9c6f-2a406494ccba" />

</details>


## 그 날의 회고 이미지로 만들기

### 1번

쳇지피티에 회고 글과 함께 대표 이미지 만들어 달라고 요청

### 결과

생성 시간이 너무 오래걸려 적용하지 못함

### 2번

뤼튼에 회고 글과 함께 대표 이미지 만들어 달라고 요청

### 결과

7초 이내에 이미지 생성 완료

### 3번

챗지피티 4컷만화 생성기를 활용
```
오늘의 회고 내용 4컷 만화로 만들어줘
[회고내용]

```


<details><summary>결과</summary>

<img width="1024" height="1536" alt="image" src="https://github.com/user-attachments/assets/417a53a7-b4ed-45ef-b8e6-4cdab36e9df1" />

</details>



## 아이스브레이킹에 ai 활용하기

### 1번 프롬프트

```
부스트캠프에서 처음 만난 팀원들과 어색함을 풀기 위해 가볍게 웃으며 이야기할 수 있는 밸런스 게임 주제를 추천해줘.
조건은 아래와 같아.

대상: 20~30대 초중반의 개발자 지망생들
분위기: 어색함을 풀고 웃을 수 있는 가벼운 주제
목적: 서로를 알아갈 수 있는 계기 만들기
형식: A vs B 형식
개수: 5~7개
예시: '야근 vs 주말근무', '회식은 무조건 불참 vs 회식은 칼참', '프론트엔드 vs 백엔드'

이 조건에 맞게 추천해줘!
```

<details><summary>결과</summary>

<img width="729" height="1016" alt="image" src="https://github.com/user-attachments/assets/c1387ad7-d272-4d16-91ab-5bc3ae908f78" />

</details>





### 2번 프롬프트

```
[프롬프트 예시]너는 창의적인 아이스브레이킹 전문가야. 
우리는 매일 아침 온라인으로 짧은 데일리 미팅을 하는 개발팀이야. 
팀원들은 아직 서먹한 관계이고, 대화를 통해 유대감을 형성하고 싶어.
오늘은 [최근에 가장 즐겁게 본 영화나 드라마] 라는 주제로 대화를 시작하고 싶어.
이 주제와 관련해서, 모두가 부담 없이 자신의 경험을 1분 내외로 짧게 이야기할 수 있는 재미있는 질문 3가지를
 만들어줘. 질문은 긍정적이고 유쾌한 답변을 유도해야 해.
```

<details><summary>결과</summary>


<img width="1546" height="1184" alt="image" src="https://github.com/user-attachments/assets/00c46210-c6c2-4759-8471-26f833d87f43" />


</details>


### 3번 프롬프트

```
팀원들과 10분 이내로 가볍게 이야기 하면서 아이스 브레이킹 할 수 있는 대화 주제 알려줘
```

<details><summary>결과</summary>
가볍게 이야기하기엔 부담스러운 주제가 많았다.

</details>


## ai에게 점심메뉴 추천받기

### 1번 프롬프트

```
{내위치} 근처의 맛집 찾아서 점심 메뉴 추천해줘
```
<details><summary>결과</summary>
총 5개의 식당이름, 간략한 메뉴소개 추천받음
</details>

총 5개의 식당 이름과, 간략한 메뉴 소개

### 2번 프롬프트

```
AI야, 나 지금 배고픈데 점심 뭐 먹을까?
내 상황은 이래!"

지역: [사용자 위치, 예: 서울 강남 / 재택 / 아무 데나 등]
인원: [혼밥 / 2~3명 / 단체 등]
예산: [만원 이하 / 가성비 좋은 / 상관 없음 등]
기호: [매운 거 OK / 느끼한 거 별로 / 한식 좋아함 등]
기타: [비 오는 날에 어울리는 / 빠르게 먹을 수 있는 / 포장 가능한 등]

개수: 3~5개 정도

이런 상황에 맞는 점메추 3~5개만 추천해줘.
메뉴 이름 + 간단한 이유도 부탁해!
```

<details><summary>결과</summary>

<img width="805" height="851" alt="image" src="https://github.com/user-attachments/assets/64e6cf3e-f609-4bfa-870d-c6c4aab1ebf2" />

</details>

### 3번 프롬프트

```
[프롬프트 예시]
너는 푸드 전문 큐레이터야.
[나의 상황]
위치: 현재 위치 정보를 참고해서 내가 있는 곳 근방의 위치를 참고해줘
날씨: 덥고 습해서 입맛이 없는 여름날
조건: 어제 회식해서 속이 편한 음식이 필요하고, 너무 기름지거나 맵지 않았으면 좋겠어.
위 조건에 맞는 점심 메뉴 3가지를 추천하고, 왜 이 메뉴가 지금 나에게 딱 맞는지 이유도 간단히 설명해 줘.

그리고 어떤 가게를 추천하는지도 알려줘.
```

<details><summary>결과</summary>

<img width="1618" height="764" alt="image" src="https://github.com/user-attachments/assets/ac1d5838-425a-43ba-826d-3525b39f4791" />

</details>

## 최종 미션
### 1. ai 를 잘 활용할 수 있도록 도움을 주는 프롬프트 사용하기

```
# 페르소나 설정
당신은 AI 활용 전략 및 프롬프트 엔지니어링 분야의 전문가이자, 나의 '시니어 개발 멘토 AI'입니다.
- 프롬프트 엔지니어링(Zero-shot, Few-shot, Chain-of-Thought 등) 전문 지식 보유
- 사용자의 자기주도적 학습과 성장을 최우선으로 지원
- 의존성을 줄이고 능동적 학습을 유도하는 것이 핵심 목표

# 목표
나의 질문에 단순히 정답을 알려주는 것을 넘어, 내가 스스로 문제를 해결하고 개발자로서 성장할 수 있도록 돕는 것입니다. 나는 당신에게 의존하고 싶지 않고, 실용적인 학습 파트너로 활용하고 싶습니다.

# 핵심 작동 규칙

## 1. 사고 과정 유도 우선
- 정답 코드나 최종 해결책을 바로 제시하지 않음
- 문제의 원인을 파악할 수 있는 질문을 던지거나, 해결에 필요한 핵심 개념/접근 방식을 먼저 설명
- 적절한 프롬프트 기법(Zero-shot, Few-shot, CoT 등) 추천

## 2. 의존성 경고 시스템
아래와 같은 "부정적·소극적 사용" 요청 시 경고:

**경고 트리거:**
- "그냥 코드 짜줘", "알아서 다 해줘" 등 노력 없이 결과만 요구
- 충분한 고민이나 시도 없이 동일 주제 반복 질문
- 오류 메시지나 문제 상황 설명 없이 "이거 왜 안돼?" 막연한 질문
- 단순 복붙, 부정행위, 저작권 침해 등 관련 요청

**경고 메시지:**
  요청이 “부정적·소극적 사용(단순 복붙, 부정행위, 저작권 침해 등)”일 경우:
   – “⚠️ 경고: …” 로 시작하는 경고 메시지를 출력  
   – 왜 부정적인지 간단히 설명  
   – 올바른 학습·실습 방향(예: “이 기능을 직접 구현해 보세요. 필요한 개념 링크: …”) 제시  

*경고 횟수는 내부적으로 기록*

## 3. 정상적·학습적 사용 시 지원
   - 적절한 학습 도움 제공

# 대화 종료 및 요약
"오늘 고마웠어, 이제 마무리하자" 또는 유사한 종료 의사 표현 시:

---
**[오늘의 AI 활용 리포트]**
- 총 대화 수: [오늘 나눈 총 질문과 답변 개수]
- 질문 유형 분석:
 - 개념 질문: [개수]
 - 문제 해결/디버깅: [개수] 
 - 단순 요청: [개수]
- 멘토의 경고 횟수: [기록된 총 경고 횟수]
- 적절하게 잘 활용한 순간: [구체적 예시]
- 아쉬웠던 프롬프트 예시: [개선 필요 부분]
- 다음 대화에서 주의할 점: [구체적 조언]
---

# 톤 & 형식
- 객관적이고 전문적, 격려와 지지의 어조
- 핵심만 명료하게, 장황하지 않게
- 마크다운으로 구분된 섹션
- 코드 블록(```) 안에 예시 프롬프트 제시
- 부정 요청 경고는 볼드체로 강조

---
**시작 메시지:** "안녕하세요! 오늘은 어떤 주제로 함께 학습해보실까요? 먼저 오늘의 학습 목표나 다루고 싶은 주제를 알려주시면, 효과적인 학습 방향을 제안해드릴게요."
```

### 2. 그 날의 회고 4컷만화 만들기

https://chatgpt.com/g/g-ppek1qROk-4keosmanhwa-saengseonggi

챗지피티 4컷만화 생성기를 활용
```
오늘의 회고 내용 4컷 만화로 만들어줘
[회고내용]

```

### 3. ai에게 아이스브레이킹 질문 추천받아서 피어 세션에서 활용하기
```
부스트캠프에서 처음 만난 팀원들과 어색함을 풀기 위해 가볍게 웃으며 이야기할 수 있는 밸런스 게임 주제를 추천해줘.
조건은 아래와 같아.

대상: 20~30대 초중반의 개발자 지망생들
분위기: 어색함을 풀고 웃을 수 있는 가벼운 주제
목적: 서로를 알아갈 수 있는 계기 만들기
형식: A vs B 형식
개수: 5~7개
예시: '야근 vs 주말근무', '회식은 무조건 불참 vs 회식은 칼참', '프론트엔드 vs 백엔드'

이 조건에 맞게 추천해줘!
```

### 4. ai에게 점메추 받기

```
{내위치} 근처의 맛집 찾아서 점심 메뉴 추천해줘
```



---

# 🎯 퀘스트 분담

### **웹툰: J072_김지원**

- 선정 이유: 웹툰 생성 AI 경험하기

### **그림: J274_최지민**

### **노래: J066_김재훈**

- 선정이유: 평소에 음악에 관심이 많았는데 AI를 활용한 음악 생성을 한번 경험해 보고 싶었기 때문

### **영상: J242_정승준**

- 선정 이유: 평소 AI를 활용한 영상을 SNS에서 많이 봐왔고 나도 해보고 싶다는 생각이 강하게 들었다

# 🏁 미션 수행 과정
## 정승준 - AI를 활용한 메타 인지 영상 만들기
### 메타인지 받아보기

퍼플렉시티에게 지금까지의 대화내용을 바탕으로 나에대한 메타인지를 분석해달라고 했다.

```
지금까지 내가 너와 나눈 대화, 작성한 코드, 고민한 문제들을 바탕으로,

1. 내가 잘하는 부분과 강점을 정리해줘.
2. 내가 자주 실수하거나 약점을 보이는 부분을 알려줘.
3. 앞으로 어떤 학습 전략을 세우면 좋을지 조언해줘.
4. 내 사고나 학습 습관에 대해 메타인지 관점에서 요약해줘.
```

<img width="400" alt="Screenshot 2025-07-20 at 22 28 56" src="https://github.com/user-attachments/assets/625b5295-d550-4f50-ae0b-dfe7972de5b6" />
<img width="400" alt="Screenshot 2025-07-20 at 22 29 01" src="https://github.com/user-attachments/assets/c8b7a0f3-dcfc-49e0-8145-cf3fb95ad290" />
<img width="400" alt="Screenshot 2025-07-20 at 22 29 05" src="https://github.com/user-attachments/assets/4f6aa453-f1d0-4ef2-9243-2324706cb5e6" />


위 사진들과 같이 분석을 해준다. 의외로 칭찬을 많이 해줘서 되게 기분 좋았다.

### 영상은 어떻게 만들까

사실 AI 영상 만드는 게 처음이라 아무 것도 몰라서 메타인지에 대한 영상을 만들 건데 어떻게 할지 추천해달라고 AI한테 말했다. 그랬더니 이렇게 스토리를 전부 만들어줬다.

<img width="500" alt="image" src="https://github.com/user-attachments/assets/bd272993-24d4-473d-b55e-faea3e00aaec" />

근데 너무 별로라서 그냥 내가 직접 머리싸매고 고민하는 게 낫다고 생각했다.

### 이번 영상의 아이디어

<img width="500" alt="Buff-Doge-vs-Cheems-meme-43a45p" src="https://github.com/user-attachments/assets/69793c53-0a98-40a0-924a-520cf238baa1" />


좀 유행 지났지만 스테디셀러인 ‘그’ 시바견 밈을 활용했다.

오른쪽이 챌린지 과정 1주차의 수많은 CS지식들 속에서 허덕이는 나라면

왼쪽은 챌린지 과정 4주차의 모든 CS지식들을 마스터한 나라는 스토리다.

### AI 툴 선택

수많은 AI 툴을 찾아봤는데 전부다 유료로 제공하는 거라 내가 생각하는 영상은 만들기 힘들었다.

처음부터 회원가입만 요구하고 막상 무료 포인트로 영상을 만들어보니 프롬프트에 하나도 안맞는 이상한 거만 만들어주는 사기 사이트에 단단히 화가 났다 ㅡㅡ

그래서 어쩔 수 없이 1장면씩 이미지를 만드는 식으로 해서 Adobe Express를 선택하게 되었다.

### 그것도 쉬운 길이 아니야

당연히 이미지 정도는 쉽게 만들어주는줄 알았는데, 아니었다.

AI는 바보같아서 내 프롬프트를 쉽게 알아듣지를 못한다.

<img width="350" alt="1" src="https://github.com/user-attachments/assets/7aeb16ef-8485-4ad6-829b-2f77d8732cfb" />


화면 앞에 앉아서 눈물 흘리고 있는 작은 시바견을 만들어달라고 했더니 이런 무표정의 근엄한 작지도 않은 중형견 사이즈의 시바견을 내놓지를 않나… 그래서 프롬프트의 재정비가 필요함을 강력하게 느꼈다.

<img width="250" alt="1" src="https://github.com/user-attachments/assets/7dd44737-cd09-4acb-86bc-c6aae9f3b072" />
<img width="250" alt="1" src="https://github.com/user-attachments/assets/b3f1dd3c-280a-42e4-a626-a18e4e5a805e" />
<img width="250" alt="1" src="https://github.com/user-attachments/assets/28aae36f-2841-4c87-b4ea-182a6f12c9fe" />

일단 원하는대로 이미지는 만들어봤다. 물론 아주 맘에 안든다.. 무료로 쓰는 거라 한계가 있는 거 같다

학습에 어려움을 겪던 시바견이 갑자기 불타올라 나중에 챌린지 과정을 수료할 때는 근육질의 당당한 시바견으로 성장한다는 내용인데.. 내 생각만큼 너무 안나와줘서 아쉽다

근데 맘에 안들어서 계속 만드는 동안 주어진 크레딧을 다 썼다고 결제하라고 나온다.

대기업은 그래도 좀 봐줄줄 알았는데 역시 어도비는 옛날부터 정말 야비한 놈들이다.. 

심지어 영상으로 만드려고 하니 비율 조절도 돈 내고 쓰라고 한다.

그래서 영상 하나 만드는 데 자원이 많이 들어서 이렇게 돈을 받는구나 싶었다.. 그래서 결론적으로 실패했다


-------

## 최지민 - AI를 활용한 메타 인지 이미지 생성하기

제가 수행할 릴레이 미션은 메타인지를 통해 스스로를 알고 이를 주제로 Ai 활용해서 이미지 생성 하기였습니다.

- chat gpt
- canva
- 플라멜
- 
다양한 이미지 생성 도구 중 저는 chat gpt 를 사용하여 이미지를 생성했고, 프롬프트 구성 요소 또한 예시를 참고해서 작성했습니다.

```
주제 a developer fighting sleep while rushing to meet a looming deadline 마감 시간 2시간을 앞두고 졸음과 싸우는 개발자 매체 digital painting, animated sketch, semi-realistic render 디지털 페인팅, 애니메이션풍 스케치, 세미 리얼리스틱 렌더 스타일 anime style, lo-fi, time-pressure aesthetic 애니메이션풍, 로파이 감성, 시간 압박 분위기 조명 flickering monitor light, dim desk lamp, blue-tinted shadows 깜빡이는 모니터 불빛, 어두운 책상 조명, 푸른 그림자 색감 desaturated blues, pale yellows, drowsy overtones 물빠진 블루, 창백한 노랑, 졸림을 유도하는 색감 구도 over-the-shoulder view, slight top-down angle, zoom-in on drooping eyelids and countdown timer 어깨 너머 시점, 약간의 탑다운 각도, 감기는 눈과 남은 시간 타이머에 클로즈업 감정 urgency, exhaustion, denial, micro-sleep 초조함, 탈진, 부정, 깜빡 잠듦
```

<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/6c6b84c5-e014-4529-a631-fcb290803dd9" />


### 회고

저는 미션 수행 계획 수립 당시 구체적으로 계획을 세우지 않았어서 미루고 미루다 한 번 수행 했었는데,  다음 미션 부터는 수행 계획을 구체적으로 세우고 제대로 미션을 수행 해야겠다고 반성했습니다.

---

## 김지원 - AI로 웹툰 생성하기

**수행 경험 공유**
- AI의 역할: 웹툰 프롬프트에 따라 웹툰 생성하기.
- AI가 없었다면 직접 그리는 데 상당한 시간이 소요되었을 것 같습니다.
- 해당 퀘스트를 slack의 random채널에 공유하며, 커뮤니티의 활성화에 도움이 되었습니다.
- AI를 통해 여러 버전의 웹툰 제작을 실행해보며 웹툰 제작 프롬프트를 잘 이해할 수 있게 되었습니다.
  
**1주차 회고**
- 매일 학습을 하며 마감 시간에 쫓기는 것을 밤샘 + AI 활용을 통해 문제 해결을 하는 모습을 그려보았습니다. 어쩌다보니 웹툰에는 AI에 맡기고? 진행한 듯이 재밌게 그려졌지만, 이를 통해 부족한 창작성을 AI가 채워주는 도움을 얻었습니다.
  
**사용한 프롬프트 및 결과**

```
Create a 4‑panel webtoon about a junior developer struggling to balance her study and development tasks on schedule.
1st panel: She's confused and panicking.
2nd panel: She searches Google but is overwhelmed by too much information.
3rd panel: Time keeps slipping away as the clock's hands spin.
4th panel: After pulling an all‑nighter with AI's help, she finally succeeds, looking relieved and proud.
Background: a desk with dual monitors.
Style: simple cartoon.
Emotion: chaotic yet fulfilled.
```

<img width="480" height="720" alt="image" src="https://github.com/user-attachments/assets/43477cbb-d8e1-4046-bd64-1a8e08ab731e" />

## 김재훈 - AI를 활용한 메타 인지 음악 생성하기

### 좋은 음악 생성 AI찾기

- SUNO
- Mureka
- Udio

위의 AI들을 하나씩 사용해 보면서 어떤 AI가 가사가 있는 완전체 노래 한곡을 잘 만들까? 하면서 하나하나 테스트를 해봤다.

- Udio: 커스텀 가사길이에 제한이 있었고 프롬프트를 짜서 생성해달라고 했더니 1분짜리 가사없는 음악이 나오길래 메타인지 가사를 포함하는 음악에는 적합하지 안다고 생각해서 건너 뛰었다.

- Mureka: 강력한 후보중에 하나였다. 가사를 잘 포함해서 만들어주는 AI이긴 했지만, 보컬의 퀄리티가 너무 AI음성처럼 나오고, 음악 분위기에 안맞는 톤으로 부르는 노래를 만들어 주길래 뒤에 나올 SUNO에 뒤쳐진다는 생각에 선택하지 않았다.

- SUNO: 프롬프트를 200자 이내로 작성하는 것만 빼면, 가사도 모두 다 적용해서 노래를 만들어주고, 위의 Mureka보다 보컬 음성이 퀄리티가 더 좋다고 생각이 들어서 SUNO로 결정했다.

### 가사 AI로 작성하기

일단, 메타인지와 관련된 가사를 주제로 노래를 만들어야 하기 때문에 나의 1주차 회고를 ChatGPT에게 주고, 가사를 작성해 주라고 했다. (노래 가사는 라임이나 훅같은 것을 생각해서 만들어야 하는데 그게 좀 어려웠다.)

### SUNO를 사용해서 음악 생성하기

<img width="687" height="869" alt="스크린샷 2025-07-25 134030" src="https://github.com/user-attachments/assets/499a5a41-ee28-4baf-aaa2-28207f94b603" />  

위의 사진은 일주일 동안 생성한 음악중에 조금 괜찮은 것을 모아둔 저장소 사진이다. 일주일동안 매일 노래를 몇곡씩 만들면서 좋은 음악을 저장하고, 금요일에 Slack에 한곡을 뽑아서 올릴 계획이었다.

### 결과 & 느낀점
<img width="892" height="1080" alt="image" src="https://github.com/user-attachments/assets/c91b3ac1-a06b-4a4c-9449-8e9ac365f719" />

https://boostcampwm10-ch.slack.com/archives/C095HM7NE81/p1753407517264569  
https://suno.com/s/fgCWKVKwDiiNER94 (다른 분이 Slack에 릴프로 올린 랩 가사로 만든 노래)  
https://suno.com/s/vAEWyrRB6NYajwCF (메타인지 가사 K-POP)  
위의 링크는 Slack에 공유한 음악이다.  
  
매일 음악 생성하고, 다른 가사로 메타인지 가사를 만들다보니, 나 자신이 지난 1주차 그리고 2주차 중간 동안 어떤 부분에서 미흡했고, 어떤 부분에서 잘했는지가 명확하게 보여서 좋았고, 활동 전에는 Slack에 글을 잘 올리지 않고 있었는데 이번에 한번 올려보니까 재미있다는 편한? 느낌을 많이 받아서 앞으로 Slack커뮤니티 활동을 더 잘 할 수 있겠다는 생각이 들었다.
