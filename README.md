# QA Daily Log

## 2026-09-10
[playwright-e2e-automation] 
- test: 게시글 생성 E2E 시나리오 추가 

## 2026-09-09
[playwright-e2e-automation] 
- docs: 테스트 구조 개선사항 README 반영  
`beforeAll` 사용자 재사용 + `beforeEach` 인증 공통화 + `test.step()` 리포트 구조화  

## 2026-09-08
[playwright-e2e-automation] 
- refactor: E2E 테스트 단계를 test.step으로 구조화

## 2026-09-07
[playwright-e2e-automation] 
- refactor: 테스트별 JWT 인증 설정 공통화  
(beforeEach로 addInitScript 공통화)
- 불필요한 코드 제거 

## 2026-09-06
[playwright-e2e-automation] 
- docs: README에 CI 상태 배지 추가

## 2026-09-05
[playwright-e2e-automation] 
- refactor: 테스트 사용자 생성 로직 공통화

## 2026-09-04
[playwright-e2e-automation] 
- test: 게시글 삭제 E2E 시나리오 추가 

## 2026-09-03
[playwright-e2e-automation] 
- ci: Playwright  테스트 리포트 artifact 추가 
- Test Fail 시에만 artifacts가 생성되도록 설정하려다가 아래 이유로 Pass/Fail 모든 경우에 artifacts가 생성되도록 함 - if: always()  
① 테스트 실행 증적을 남기기 위해  
② retention-days: 7로 7일 후 GitHub 저장소에서 파일이 쌓이지 않고 사라지도록 설정함  

## 2026-09-01
[playwright-e2e-automation] 
- docs: 리팩토링 및 CI 반영해 README 업데이트

## 2026-08-31
[playwright-e2e-automation] 
- refactor: 테스트 데이터 상수 분리

## 2026-08-30
[playwright-e2e-automation] 
- refactor: 토큰 인증 및 게시글 cleanup 추가 

## 2026-08-28
[playwright-e2e-automation] 
- refactor: UI 로그인 과정을 API 인증으로 대체 

## 2026-08-27
[playwright-e2e-automation] 
- refactor: 테스트 구조 및 문서 정리  
- ci: GitHub Actions E2E 테스트 자동화 추가  

## 2026-08-26
[playwright-e2e-automation] 
- refactor: API 요청 로직 분리
- refactor: 테스트 코드 구조 및 가독성 개선 
- docs: README.md 수정 

## 2026-08-25
[playwright-e2e-automation]  
- docs: README.md 추가  

## 2026-08-24
[playwright-e2e-automation]  
refactor: config에 baseURL 분리 + API URL 하드코딩 제거  
- API_BASE_URL 추가 for API TEST
- playwright.config.ts 파일에 baseURL 추가 for UI TEST

## 2026-08-23
[playwright-e2e-automation] Repository 생성  
API → 테스트 사용자 생성  
API → 게시글 생성 (Authorization 헤더에 토큰을 포함하여 요청)  
UI  → 로그인  
UI  → API로 생성한 게시글 확인  
UI  → 게시글 수정  
API → 수정 요청 발생 확인  
API → 게시글 재조회  
API → UI에서 수정한 body와 최종 서버 데이터 비교  

이후 작업 예정 순서  
① config/baseURL 분리 + API URL 하드코딩 제거  
② API/UI 역할 분리 리팩터링  
③ 테스트 이름 정리  
④ README  
⑤ GitHub Actions CI  

Repository 정리  
[api-test-automation] API Test Automation with Postman & Newman  
[playwright-test-automation] API Test Automation with Playwright  
[playwright-e2e-automation] API & UI E2E Test Automation with Playwright  

## 2026-08-22
- TypeScript를 사용해서 assertion 추가 (category)

## 2026-08-21
- TypeScript를 사용해서 assertion 추가 (title, price)

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
