# Git Commit 메시지 규칙 (수업용 간단 버전)

## 1. 기본 구조


<타입>: <변경 내용 요약>

- 한 줄로 간결하게 작성 (50자 이내 권장)
- 무엇을, 왜 수정했는지 알 수 있게 적기

---

## 2. 타입 (Type)
아래 다섯 가지 타입만 사용합니다.

- **feat**: 새로운 기능 추가  
  예) `feat: 로그인 기능 추가`

- **fix**: 버그 수정  
  예) `fix: 회원가입 오류 수정`

- **docs**: 문서 관련 수정  
  예) `docs: README 설치 방법 추가`

- **style**: 코드 스타일 변경 (동작 변화 없음)  
  예) `style: 들여쓰기 수정`

- **chore**: 빌드, 패키지, 환경설정 등 잡일  
  예) `chore: .gitignore 파일 추가`

---

## 3. 좋은 예시

```
feat: 회원가입 기능 추가
fix: 로그인 시 비밀번호 검증 오류 수정
docs: 설치 가이드 업데이트
style: 코드 줄바꿈 수정
chore: 라이브러리 버전 업데이트
```

---

## 4. 나쁜 예시
```
update file # 어떤 파일을 왜 수정했는지 알 수 없음
bug fix # 구체적이지 않음
작업 완료 # 모호한 표현
```

---

## 5. 실습 예제
```bash
# 1. 새 파일 추가
git add hello.txt
git commit -m "feat: hello.txt 파일 추가"

# 2. 내용 수정 후 커밋
git commit -am "fix: hello.txt 문구 오류 수정"

# 3. 문서 수정
git add README.md
git commit -m "docs: README 설치 방법 추가"
```

👉 이 파일을 저장소에 추가하려면 아래 명령어를 쓰면 됩니다:

```bash
echo "위 내용 복붙" > COMMIT_RULES.md
git add COMMIT_RULES.md
git commit -m "docs: 커밋 메시지 규칙 문서 추가"
git push origin main
```
