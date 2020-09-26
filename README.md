# selftest-coding-guideline

SelfTest 프로젝트를 위한 코딩 가이드라인입니다.

## 개발 툴

- **비주얼 스튜디오 코드**에 프로젝트 불러와서 코딩 (실행을 위한 커맨드라인도 달려있음)
  - 확장프로그램 **Prettier** 설치 (코드 자동으로 정리하는 확장 프로그램, **ctrl+shift+f 한 번씩 눌러주고 커밋하기!!**)
- Git 관리 프로그램 **GitKraken** 사용 (GUI, 통일하면 도와주기 편함)
- **Trello**는 각자 할일 올려놓고 알아서 잘 쓰면 됨.

## Git 관리

- https://github.com/KennethanCeyer/tutorial-git 참고
  - 우리는 GUI 툴 깃크라켄 사용 예정이니 commit, push 등이 무슨 단어인지만 알면 대충 사용 가능

### Git 기본

- master 브랜치에 최종 발표 전까지 건드리지 않고 기본 브랜치는 dev 브랜치로!
- dev 브랜치에는 **작동이 잘 될 때만 push**하고, 그 전까지는 dev 브랜치에서 기능 단위로 하나 파생시켜서 개발
  - 브랜치 이름 예: feature/login (로그인 기능 개발 브랜치)
- 로컬에서 작업하면서 커밋 꾸준히 하다가 깃헙 서버로 올릴 때 push 해주면 됩니다.
- 백엔드는 같이 개발하는 사람이 두 명이니 더 신경써서 해야됨
  - 기능 개발이 완료되어 dev 브랜치로 머지하고 싶을때 dev로 풀리퀘를 날리면 확인하고 merge하겠음

### 브랜치 네이밍

- 통일된 규격은 없지만 협업 간에 보통 통일하는 편
- https://rumblefish.tistory.com/65 대로 하면 좋을 것 같음
- 부득이한 상황이면 안해도 됨 (알아보기만 쉽게 이름 짓기)

### 커밋 메시지 작성

- 마찬가지로 통일된 규격은 없습니다. 하지만 가독성을 위해서 통일하는게 좋습니다.
- https://richone.tistory.com/26 참고
- **제목 앞에 붙는 커밋 타입 양식 통일**: https://siyoon210.tistory.com/56
- **완전히 따르지 않아도 됨.** 한국어 상관 없음. 내용은 뭐 했는지만 대충 적어도 됨.
- 단, **현재형으로 적어주세요.**
- 커밋은 **작은 단위로 꾸준히** 할수록 좋습니다. (그 시점으로 돌아가는 데에도 유용)
- push하기 전까지는 이미 커밋한 메세지도 수정할 수 있으니 참고! (깃크라켄 amend 기능)
- 영어 예시:

```
feat: Summarize changes in around 50 characters or less

More detailed explanatory text, if necessary. Wrap it to about 72
characters or so. ... (생략)
```

- 한국어 예시: https://tttsss77.tistory.com/58

```
fix: 버그 픽스

~에서 있었던 ~를 해결한다.
```

```
feat: 로그인 기능 추가

메인 페이지에서 로그인 기능을 추가한다.

추가로 말할 내용 blah blah이다.

* 어쩌구

* 저쩌구
```

### 풀 리퀘스트 작성법

https://brunch.co.kr/@anonymdevoo/9 참고
