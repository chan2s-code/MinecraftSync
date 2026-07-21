# Git & GitHub 학습 정리

## Git이란?

Git은 프로젝트의 변경 사항을 기록하고 관리하는 버전 관리 시스템(VCS)이다.

- 코드 변경 이력 관리
- 이전 버전 복원
- 여러 사람이 동시에 협업 가능
- GitHub와 함께 많이 사용

---

## Git과 GitHub의 차이

### Git

내 컴퓨터에서 버전을 관리하는 프로그램

### GitHub

Git 저장소를 인터넷에 올려 공유하는 서비스

즉,

Git = 버전 관리 프로그램

GitHub = Git 저장소를 보관하는 사이트

---

## 기본 작업 순서

```text
파일 수정

↓

git add

↓

git commit

↓

git push

↓

GitHub 업로드
```

---

## 자주 사용하는 명령어

### 상태 확인

```bash
git status
```

현재 변경된 파일을 확인한다.

---

### 변경 내용 추가

```bash
git add .
```

모든 변경 파일을 Commit 대상으로 등록한다.

특정 파일만 등록

```bash
git add README.md
```

---

### Commit 생성

```bash
git commit -m "메시지"
```

예시

```bash
git commit -m "Add Google Drive config"
```

---

### GitHub 업로드

```bash
git push
```

---

### 최신 내용 받기

```bash
git pull
```

---

## .gitignore

Git이 추적하지 않을 파일을 지정한다.

예시

```gitignore
config.json
.env
token.json
__pycache__/
*.pyc
```

---

## 이미 추적 중인 파일은?

.gitignore에 추가해도 이미 Git이 추적 중인 파일은 계속 올라간다.

추적을 해제하려면

```bash
git rm --cached config.json
```

를 사용한다.

파일은 삭제되지 않고 Git에서만 제거된다.

---

## config.example.json을 사용하는 이유

실제 설정 파일은 GitHub에 올리지 않는다.

대신

config.example.json

을 제공하여

사용자가 복사 후

config.json

으로 사용한다.

---

## 앞으로 자주 사용할 명령어

```bash
git status
git add .
git commit -m "메시지"
git push
git pull
```