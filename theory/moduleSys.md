ESModule CommonJS
import require
export default module.exports
export { namedExport } exports.namedExport

Object.defineProperty(exports, "\_\_esModule", { value: true });
→ CommonJS가 ESModule처럼 동작하도록 보장.

CommonJS의 require와 exports를 ESModule의 import와 export로 변환하거나 반대로 변환.

###

ts는 일단 파일들(모듈)을 전역 모듈로 보기 때문에

export 등의 모듈 시스템 코드를 사용하면
전역 공통 공간이 아니라 독립된 공간으로 바라본다.
혹은 모듈 디텍션으로 컴파일러 옵션을 설정해주자

-> Unkown compiler option 'moduleDetection'에러의 경우
vs 코드의 setting.json에 아래 추가 (open user settings)
"typescript.tsdk": "./node_modules/typescript/lib"
tsc --version으로 타입스크립트 버전 확인하고 맞춰서 로컬 타입스크립트 재설치
npm install --save-dev typescript@5.7.2
command + shift + p로 설정 열어서
select typescript version 검색 후 Use VS Code's Version 선택 (안나오면 VS 껐다 키자 ^\_\_^)
