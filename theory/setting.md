npm init

npm i @types/node

타입스크립트 컴파일러 설치 (글로벌)
sudo npm install typescript -g
(tsc -v 확인)

타입스크립트 실행(typescript execute)

sudo npm i -g tsx (ts-node 대신 최신)
tsx 경로 -> 바로 실행
tsc 경로 -> JS 파일로 컴파일 -> node 경로로 실행

### 타입스크립트 컴파일러 옵션

얼마나 엄격하게 타입 오류를 체크할 것인지, 자바스크립트 코드의 버전은 어떻게 할 지 등 세팅

tsc --init -> tsconfig.json 생성
