# 개발 도구 고지 / Development tool notices

2026-10-10 기준으로 비경회기 v0.1.0의 의존성 잠금 파일, 설치된 패키지의 버전·라이선스 선언·원문, 빌드 설정과 실제 사용 위치를 읽기 전용으로 확인했습니다. 이 목록은 개발·빌드·검증·로컬 미리보기 도구에 대한 기록이며, 모든 항목이 게임 브라우저 코드에 배포된다는 뜻은 아닙니다. 게임에 포함되는 라이브러리와 CSS는 [제3자 고지](THIRD_PARTY_NOTICES.md)를 참고하세요.

Reviewed on 2026-10-10 against the v0.1.0 dependency lockfile, installed package metadata and supplied licenses, and actual configuration/imports. This is a record of development, build, test and local preview tools, not a claim that every tool ships in the browser game. Libraries and CSS incorporated into the game are covered in [Third-party notices](THIRD_PARTY_NOTICES.md).

| 도구 / Tool | 확인 버전 / Version | 라이선스 / License | 확인 용도 / Purpose | 공식 출처 / Source | 보존 원문 / License text |
| --- | --- | --- | --- | --- | --- |
| `@cloudflare/vite-plugin` | 1.37.1 | MIT | Workers 빌드·미리보기 통합; 생성 wrapper의 배포 포함은 제3자 고지 참조 | [버전 출처](https://github.com/cloudflare/workers-sdk/tree/%40cloudflare%2Fvite-plugin%401.37.1/packages/vite-plugin-cloudflare) | [MIT](third-party-licenses/dev-tools/cloudflare-vite-plugin-1.37.1-LICENSE-MIT.txt) |
| `@cloudflare/workers-types` | 4.20260515.1 | MIT OR Apache-2.0 선언; 형 선언 헤더는 Apache-2.0 | Workers 형 검사 | [공식 저장소](https://github.com/cloudflare/workerd) | [Apache](third-party-licenses/dev-tools/workers-types-4.20260515.1-LICENSE-APACHE.txt), [저작권 헤더](third-party-licenses/dev-tools/workers-types-4.20260515.1-ATTRIBUTION.txt) |
| `@tailwindcss/postcss` | 4.2.1 | MIT | CSS 생성용 PostCSS 플러그인 | [공식 저장소](https://github.com/tailwindlabs/tailwindcss) | [MIT](third-party-licenses/dev-tools/tailwindcss-postcss-4.2.1-LICENSE.txt) |
| `@types/node` | 22.19.19 | MIT | Node.js 형 선언 | [공식 저장소](https://github.com/DefinitelyTyped/DefinitelyTyped/tree/master/types/node) | [MIT](third-party-licenses/dev-tools/definitelytyped-LICENSE.txt) |
| `@types/react` | 19.2.14 | MIT | React 형 선언 | [공식 저장소](https://github.com/DefinitelyTyped/DefinitelyTyped/tree/master/types/react) | [MIT](third-party-licenses/dev-tools/definitelytyped-LICENSE.txt) |
| `@types/react-dom` | 19.2.3 | MIT | React DOM 형 선언 | [공식 저장소](https://github.com/DefinitelyTyped/DefinitelyTyped/tree/master/types/react-dom) | [MIT](third-party-licenses/dev-tools/definitelytyped-LICENSE.txt) |
| `@vitejs/plugin-react` | 6.0.2 | MIT | Vinext의 React 빌드 플러그인 의존성 | [공식 저장소](https://github.com/vitejs/vite-plugin-react/tree/main/packages/plugin-react) | [MIT](third-party-licenses/dev-tools/vitejs-plugin-react-6.0.2-LICENSE.txt) |
| `drizzle-kit` | 0.31.10 | MIT 선언; 패키지 별도 원문 미확인 | 데이터베이스 마이그레이션 생성 | [해당 버전 선언](https://github.com/drizzle-team/drizzle-orm/blob/drizzle-kit%400.31.10/drizzle-kit/package.json) | 아래 확인 한계 참조 |
| `eslint` | 9.39.4 | MIT | 코드 린트 | [공식 저장소](https://github.com/eslint/eslint) | [MIT](third-party-licenses/dev-tools/eslint-9.39.4-LICENSE.txt) |
| `eslint-config-next` | 16.3.4 | MIT | Next.js용 린트 설정 | [버전 출처](https://github.com/vercel/next.js/tree/v16.3.4/packages/eslint-config-next) | [MIT](third-party-licenses/dev-tools/eslint-config-next-16.3.4-LICENSE.txt) |
| `fake-indexeddb` | 6.2.5 | Apache-2.0 | IndexedDB 자동 검증용 대체 구현 | [공식 저장소](https://github.com/dumbmatter/fakeIndexedDB) | [Apache](third-party-licenses/dev-tools/fake-indexeddb-6.2.5-LICENSE.txt) |
| `json-rpc-2.0` | 1.7.1 | MIT | 로컬 연결 미리보기 통신 | [공식 저장소](https://github.com/shogowada/json-rpc-2.0) | [MIT](third-party-licenses/dev-tools/json-rpc-2.0-1.7.1-LICENSE.txt) |
| `raw-body` | 3.0.2 | MIT | 로컬 연결 미리보기 요청 읽기 | [공식 저장소](https://github.com/stream-utils/raw-body) | [MIT](third-party-licenses/dev-tools/raw-body-3.0.2-LICENSE.txt) |
| `typescript` | 5.9.3 | Apache-2.0; 포함된 제3자 자료는 각각의 고지 적용 | 형 검사 | [공식 저장소](https://github.com/microsoft/TypeScript) | [Apache](third-party-licenses/dev-tools/typescript-5.9.3-LICENSE.txt), [포함 고지](third-party-licenses/dev-tools/typescript-5.9.3-ThirdPartyNoticeText.txt) |
| `vite` | 8.0.13 | MIT; 번들된 구성요소는 원문 내 각 라이선스 적용 | 개발 서버·번들 생성 | [공식 저장소](https://github.com/vitejs/vite) | [전체 라이선스와 포함 고지](third-party-licenses/dev-tools/vite-8.0.13-LICENSE.md) |
| `wrangler` | 4.92.0 | MIT OR Apache-2.0 | Workers 로컬 실행·배포 도구 | [버전 출처](https://github.com/cloudflare/workers-sdk/tree/wrangler%404.92.0/packages/wrangler) | [MIT](third-party-licenses/dev-tools/cloudflare-vite-plugin-1.37.1-LICENSE-MIT.txt), [Apache](third-party-licenses/dev-tools/wrangler-4.92.0-LICENSE-APACHE.txt) |

로컬 개발에서 확인한 Node.js는 v24.19.0입니다. [공식 해당 버전 LICENSE](https://github.com/nodejs/node/blob/v24.19.0/LICENSE)는 Node.js 자체의 MIT 조건과 포함된 외부 구성요소의 고지를 함께 제공합니다. 이는 운영 호스팅의 Node.js 사용 여부나 버전을 확인한 기록은 아닙니다.

The locally observed Node.js version was v24.19.0. Its [official versioned LICENSE](https://github.com/nodejs/node/blob/v24.19.0/LICENSE) contains the Node.js MIT terms and notices for bundled components. This does not establish the Node.js version or use in production hosting.

## 확인 범위와 한계 / Scope and limitations

- 직접 `devDependencies` 21개의 잠금 버전과 설치 버전이 일치함을 확인했습니다. 이 중 `vinext` 1.0.0-beta.5, `react-server-dom-webpack` 19.2.6, `@vitejs/plugin-rsc` 0.5.26, `tailwindcss` 4.2.1, `tw-animate-css` 1.4.0은 런타임 코드·생성 코드·CSS와 관련되어 제3자 고지에서 다룹니다. `devDependencies`라는 분류만으로 개발 전용이라고 판단하지 않습니다.
- 설치물에 제공된 라이선스·고지 원문은 그대로 보존했습니다. 별도 원문이 없는 Cloudflare 도구는 해당 버전 공식 저장소 원문과 형 선언의 저작권 헤더를 기록했습니다. ESLint Next 설정은 동일 버전 Next.js의 원문과 공식 버전 저장소를 사용했습니다. [원문 출처 기록](third-party-licenses/dev-tools/SOURCES.md)을 참고하세요.
- `drizzle-kit` 0.31.10의 패키지는 MIT로 선언하지만, 설치물에 별도 LICENSE가 없고 동일 버전 저장소 루트 [LICENSE](https://github.com/drizzle-team/drizzle-orm/blob/drizzle-kit%400.31.10/LICENSE)는 Apache-2.0입니다. 서로 다른 범위의 원문을 임의로 대체하거나 저작권 문구를 만들어 넣지 않았습니다. 이 도구를 재배포할 때는 해당 패키지의 적용 원문과 고지를 추가 확인해야 합니다.
- 개발 도구의 모든 전이 의존성을 독립적으로 전수 조사하지 않았습니다. Vite가 제공한 번들 라이선스와 TypeScript의 제3자 고지 파일은 생략하지 않았습니다. 서비스 약관·호스팅 비용·무료 API 제공 조건은 소프트웨어 라이선스와 별개이며, 사용 증거가 없는 외부 API를 이 목록에 추가하지 않았습니다.
- 이 공개 소개 저장소의 고지 추가만으로 실제 게임 배포물의 라이선스 의무가 모두 충족되었다고 주장하지 않습니다. 외부 권리자의 라이선스가 각 구성요소에 적용되며, 게임 전체의 재사용 허가는 [권리 안내](LICENSE)와 구분됩니다.

All 21 direct development dependencies were checked against the lockfile and installed versions. Five packages connected to runtime or CSS output are covered in the third-party notices rather than treated as development-only. Supplied license/notice texts are retained; missing texts use the stated official sources. Drizzle Kit's package-level MIT declaration and repository-level Apache text require further clarification before redistribution of the tool. The complete development dependency tree was not independently audited; Vite's bundled notices and TypeScript's supplied third-party notice file are preserved. Service terms and pricing are separate from software licenses. These repository notices do not establish that the deployed game satisfies every distribution obligation.
