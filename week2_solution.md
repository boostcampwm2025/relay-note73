# 릴레이 미션 수행

**[S033\_정영빈](#-s033_정영빈)**  
**[J159\_오희주](#-j159_오희주)**  
**[J176\_이경원](#-j176_이경원)**  
**[J177\_이규태](#-j177_이규태)**

## 🌞 S033\_정영빈

## 선택 퀘스트

**AI를 통한 Git Index 공식 문서 학습**

## 활동 사항

<details>
<summary>눌러 보기</summary>

### 📚 Git Index 바이너리 형식 구현

Git 호환 명령어 구현 미션을 진행하면서 Git Index의 바이너리 형식을 학습했습니다.

### 🔍 학습 프로세스

**1단계: 한국어로 시작**

- "git index 파일 구조"로 검색
- 표면적인 "스테이징 영역" 설명만 발견

**2단계: 영어로 전환**

- "git index file format binary"로 재검색
- Git 공식 문서 링크 획득

**3단계: 공식 문서 분석**

- https://git-scm.com/docs/index-format
- DIRC 헤더, Entry 구조, 8-byte alignment 등 명세 확인

### 💡 AI 활용 장점

**1. 바이너리 형식 이해**

- "DIRC는 DirCache의 약자" 같은 숨은 의미 파악
- hexdump로 실제 확인:

```bash
$ hexdump -C .git/index | head -1
00000000  44 49 52 43 00 00 00 02  |DIRC....|
```

**2. 디버깅 도구 활용**

```bash
$ git ls-files --debug
$ xxd .git/index
```

**3. 구현 가이드**

- TimeSpec (나노초 정밀도)
- 8바이트 정렬 패딩
- Big-endian 변환

### ⚠️ AI 활용 단점

**1. 복붙으로 인한 이해도 저하**

```swift
// 무작정 복사한 코드
data.withUnsafeBytes { $0.load(as: UInt32.self).bigEndian }
// 나중에야 "네트워크 바이트 순서구나" 깨달음
```

**2. 맥락 파악 실패**

- "Index out of bounds" 에러의 진짜 원인:
  - SHA-1 (20) vs SHA-256 (32) 길이 차이
  - SubSequence 처리 문제
  - null terminator 위치 계산 실수

### 🛠️ 구현 결과

```bash
# 호환성 테스트
./git add test.txt
git status  # ✅ 공식 Git이 인식!
```

</details>

## 느낀점 및 결론

**"AI는 나침반, 공식 문서는 지도"**

Git Index같은 복잡한 바이너리 형식을 다룰 때:

- AI로 빠른 개념 파악과 시작점 찾기
- 공식 문서로 정확한 스펙 확인
- 실제 구현물과 비교 검증

가장 큰 교훈은 AI가 제공하는 코드를 무작정 복사하지 말고, **이해하고 검증하는 과정이 필수**라는 것입니다.

---

## 🍏 J159\_오희주

## 선택 퀘스트

## 활동 사항

<details>
<summary>눌러 보기</summary>

</details>

## 느낀점 및 결론

---

## 🤓 J176\_이경원

## 선택 퀘스트

## 활동 사항

<details>
<summary>눌러 보기</summary>

</details>

## 느낀점 및 결론

---

## 🥸 J177\_이규태

## 선택 퀘스트

## 활동 사항

<details>
<summary>눌러 보기</summary>

</details>

## 느낀점 및 결론
