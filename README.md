## tsconfig.json 설정

```json
{
  "include": ["src"], // 타입스크립트 사용할 폴더 지정
  "compilerOptions": {
    "outDir": "build", // ts->js로 빌드될 폴더 지정
    "target": "ES6", // 어떤 시점의 js로 빌드할지 지정
    "lib": ["ES6"], // 타입스크립트에게 어떤 API를 사용하고 어떤 환경에서 코드를 실행하는 지를 지정
    // "lib":["ES6","DOM"] => 브라우저에서 돌아감 document.querySelector 같은 브라우저API 자동완성 지원
    "strict": true, // 모든 엄격한 타입 검사 옵션을 활성화
    "allowJs": true // 타입스크립트에서 자바스크립트를 사용 가능하게 함
  }
}
```

### ts-node

- 타입스크립트를 자바스크립트로 빌드하지 않고 실행시켜준다(develop모드)
