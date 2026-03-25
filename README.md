# c-actions-lab

C 언어 소스 코드를 GitHub Actions로 자동 빌드하는 실습용 프로젝트입니다.  
이 프로젝트는 간단한 덧셈 프로그램을 통해 다음 내용을 학습하는 것을 목표로 합니다.

- C 언어 소스 코드 작성
- Makefile을 이용한 빌드 자동화
- GitHub Actions를 이용한 CI(Continuous Integration) 실습
- 저장소 push 시 자동 빌드 동작 확인

---

## 1. 프로젝트 개요

이 프로젝트는 `src/main.c` 파일에 작성된 간단한 C 프로그램을 빌드하는 구조로 되어 있습니다.  
프로그램은 두 정수 `a`, `b`를 선언하고, 두 수의 합 `sum`을 계산하여 출력합니다.

실습자는 이 프로젝트를 통해 다음과 같은 DevOps 기초 흐름을 경험할 수 있습니다.

1. 로컬에서 소스 코드 작성
2. GitHub 저장소에 업로드
3. GitHub Actions 워크플로 자동 실행
4. 빌드 성공 여부 확인

---

## 2. 프로젝트 구조

```text
c-actions-lab/
├─ src/
│  └─ main.c
├─ Makefile
├─ README.md
└─ .github/
   └─ workflows/
      └─ c-build.yml