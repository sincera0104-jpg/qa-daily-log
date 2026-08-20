# QA Daily Log

## 2026-08-20
[Codex]
- api-test-automation 프로젝트 구조 분석
- 개선할 사항 분석
- 'GET 존재하지 않는 상품'에 Status Code assertion 추가 
- diff 확인
- Postman과 동기화 방법 확인 (추후 연동 및 Playwright API TEST로 대체)
- git add, commit, push 
- staging 되었는지 직접 확인 
- Codex에게 어디까지 맡겨야할지 고민 

[Playwright]
- tests/api/products.spec.ts 생성 

[Tistory]
- 'Conventional Commits 스타일' 발행 

## 2026-08-19
- Fake Store Carts API POST 장바구니 추가 request 추가

## 2026-08-18
- Fake Store Carts API chaining tests 추가

## 2026-08-15
- Fake Store Carts API request 추가 

## 2026-08-14
api-test-automation
- Fake Store Content-Type assertion 추가 
- api-test-automation README prerequisites 추가 
- .gitignore 분류 명확화 

## 2026-08-13

- api-test-automation README에 테스트 결과 CI 뱃지 추가 (Add CI status badge to README)

## 2026-08-12

- Newman HTML Report 생성 + Artifact 업로드 
`(npm install -g newman-reporter-htmlextra)`

## 2026-08-11

- api-test-automation README.md 생성 

## 2026-08-10

CrudCrud API Resource 

- CRUD API Chaining으로 End-to-End 시나리오 구성
- GitHub Repository Secrets 통한 환경변수 관리 
- YAML indentation 및 실행 경로 문제 디버깅

## 2026-08-09

- API 검증 그리고 자동화 내용 문서 정리 
- `git push -u`에서 `-u`의 의미 학습
- `git commit -m`에서 `-m`의 의미 학습

## 2026-08-07

Fake Store API Resource 

[Postman]
- 검증 Assertions 작성 (collection.json)
- 환경 설정 (environment.json)
- Postman Runner PASS

[Newman]
- CLI 환경 Node.js, Newman 설정 
- Environment의 Share Value 추가 
- Newman CLI PASS

[Git]
- Git 저장소 구성
- GitHub Repository 연결

[Github Actions]
- GitHub Actions Workflow 구성 (.yaml)
- GitHub Actions CI 실행
