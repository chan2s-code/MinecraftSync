# VS Code 문제 해결 기록

---

# Ctrl + V가 터미널에서 동작하지 않음

## 증상

VS Code 터미널(cmd)에서

Ctrl + V

를 누르면

```
^V
```

만 입력되고 붙여넣기가 되지 않았다.

---

## 원인

VS Code 기본 단축키에서

터미널 붙여넣기 단축키는

```
Ctrl + Shift + V
```

로 설정되어 있었다.

---

## 해결

### 방법 1 (권장)

Ctrl + Shift + V 사용

또는

우클릭 → 붙여넣기

---

### 방법 2

VS Code 단축키에서

Terminal: Paste

를

Ctrl + V

로 변경 가능

---

# config.json이 보이지 않음

## 증상

프로젝트에는

config.json

이 존재한다고 나오지만

VS Code 탐색기에서는 보이지 않았다.

새 파일을 만들려고 하면

```
이미 존재하는 파일입니다.
```

라는 메시지가 출력되었다.

---

## 원인

VS Code의 Explorer 설정 또는 새로고침 문제였다.

실제 파일은 존재하고 있었으며

탐색기에서 정상적으로 표시되지 않았다.

---

## 해결

Explorer 새로고침 후 정상 표시되었다.

필요하면

Developer: Reload Window

를 실행한다.

---

# Mermaid Preview가 검은 화면

## 증상

Markdown Preview에서

Mermaid 다이어그램이

잠깐 나타난 뒤

검은 화면으로 변경되었다.

---

## 확인 내용

일반 Markdown은 정상 출력된다.

Mermaid만 렌더링되지 않는다.

---

## 현재 상태

원인 미확인

GitHub에서 정상 렌더링되는지 추후 확인 예정이다.