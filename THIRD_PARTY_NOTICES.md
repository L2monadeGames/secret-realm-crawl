# 외부 소프트웨어·리소스 고지 / Third-party notices

확인일: 2026-10-10 · 게임 소개 버전: v0.1.0

비경회기(祕境廻起) / Secret Realm Crawl은 아래 외부 소프트웨어와 리소스를 사용하거나 개발에 이용합니다. 외부 자료에는 각 원래 라이선스와 서비스 약관이 적용되며, 이 저장소의 [권리 안내](LICENSE)가 그 권리를 제한하거나 게임 자체에 같은 라이선스를 부여하지 않습니다. 원문에 있는 외부 저작권자 표시는 해당 자료의 출처입니다.

Third-party components keep their own licenses and service terms. The project's [rights notice](LICENSE) neither restricts those rights nor licenses the game under those third-party licenses. Attribution in the preserved license texts identifies the upstream rights holders.

## 조사 범위와 포함 여부 / Scope

최신 기본 브랜치의 package.json·잠금 파일, 설치된 패키지의 LICENSE/NOTICE 및 실제 import 경로를 읽기 전용으로 확인했습니다. 비교한 기존 로컬 브라우저·서버·CSS 산출물은 2026-10-08 빌드입니다. 최신 소스 또는 현재 운영 배포물과 같은 바이트인지 확인하지 않았습니다. 아래 버전은 조사한 잠금 파일·설치 패키지 기준입니다.

기존 번들에서 확인한 항목과 현행 import 경로에서 도달하는 항목을 구분했습니다. 후자는 최종 빌드의 tree shaking으로 제외될 수 있습니다. 설치된 모든 패키지를 배포 포함으로 주장하지 않습니다. 기존 JavaScript 번들에는 라이선스 배너나 별도 LICENSE/NOTICE 파일이 발견되지 않았고, CSS에는 Tailwind 라이선스 식별 배너가 남아 있습니다.

The review covers current dependency metadata, versioned installed license files, actual runtime import paths, and an existing local build dated 2026-10-08. Its identity with the latest source or live deployment is unverified. Import-path candidates may be removed by final tree shaking; installation alone does not establish distribution. No separate LICENSE/NOTICE files or JavaScript license banners were found in that inspected build. The CSS retains a Tailwind license identifier banner.

## 게임 실행 및 CSS / Runtime and generated CSS

라이선스 링크는 원문 파일로 연결됩니다. MIT·ISC·0BSD·Apache-2.0은 외부 구성요소의 조건이며 게임 코드·문서·이미지 전체에 적용되는 라이선스가 아닙니다. Lucide 원문은 ISC와 Feather 파생 아이콘에 적용되는 MIT 부분을 함께 포함합니다.

License links preserve upstream texts. These licenses apply to their respective third-party components, not to the game as a whole. Lucide's text includes both ISC and the MIT terms for Feather-derived icons.

| 구성요소 | 버전 | 라이선스 | 확인 범위 |
|---|---|---|---|
| [react](third-party-licenses/runtime/react-19.2.6.LICENSE) | 19.2.6 | MIT | 기존 번들 및 현행 사용 경로 |
| [react-dom](third-party-licenses/runtime/react-dom-19.2.6.LICENSE) | 19.2.6 | MIT | 기존 번들 및 현행 사용 경로 |
| [scheduler](third-party-licenses/runtime/scheduler-0.27.0.LICENSE) | 0.27.0 | MIT | 기존 번들 및 현행 사용 경로 |
| [react-server-dom-webpack](third-party-licenses/runtime/react-server-dom-webpack-19.2.6.LICENSE) | 19.2.6 | MIT | 기존 번들 및 현행 사용 경로 |
| [vinext](third-party-licenses/runtime/vinext-1.0.0-beta.5.LICENSE) | 1.0.0-beta.5 | MIT | 기존 번들 및 현행 사용 경로 |
| [@vitejs/plugin-rsc](third-party-licenses/runtime/vitejs-plugin-rsc-0.5.26.LICENSE) | 0.5.26 | MIT | 기존 번들 및 현행 사용 경로 |
| [@hiogawa/utils](third-party-licenses/runtime/hiogawa-utils-1.7.0-upstream.LICENSE) | 1.7.0 | MIT | 기존 번들 및 현행 사용 경로 |
| [lucide-react](third-party-licenses/assets/lucide-react-1.31.0.LICENSE) | 1.31.0 | ISC + MIT (Feather) | 기존 번들 및 현행 사용 경로 |
| [class-variance-authority](third-party-licenses/runtime/class-variance-authority-0.7.1.LICENSE) | 0.7.1 | Apache-2.0 | 기존 번들 및 현행 사용 경로 |
| [clsx](third-party-licenses/runtime/clsx-2.1.1.license) | 2.1.1 | MIT | 현행 import 경로; 최종 tree shaking 미확인 |
| [tailwind-merge](third-party-licenses/runtime/tailwind-merge-3.6.0.LICENSE.md) | 3.6.0 | MIT | 기존 번들 및 현행 사용 경로 |
| [zod](third-party-licenses/runtime/zod-3.25.76.LICENSE) | 3.25.76 | MIT | 기존 번들 및 현행 사용 경로 |
| [tailwindcss](third-party-licenses/runtime/tailwindcss-4.2.1.LICENSE) | 4.2.1 | MIT | 기존 CSS 산출물 |
| [tw-animate-css](third-party-licenses/runtime/tw-animate-css-1.4.0.LICENSE) | 1.4.0 | MIT | 기존 CSS 산출물 |
| [radix-ui](third-party-licenses/runtime/radix-ui-1.6.7.LICENSE) | 1.6.7 | MIT | 현행 import 경로; 최종 tree shaking 미확인 |

Vinext 및 RSC 어댑터는 개발 의존성으로 선언되어 있어도 실제 브라우저·서버 런타임 코드가 기존 산출물에 포함되어 있습니다. RSC 어댑터 내부에 포함된 React Server Components 19.2.6과 @hiogawa/utils 1.7.0도 확인했습니다. `next/*` 호출은 조사한 구성에서 Vinext shim으로 치환되므로 Next.js 16.3.4 패키지 전체의 런타임 포함을 의미하지 않습니다.

Vinext and the RSC adapter contribute runtime code even though they are declared as development dependencies. The adapter also embeds React Server Components 19.2.6 and @hiogawa/utils 1.7.0. In the reviewed configuration, `next/*` imports resolve through Vinext shims; this does not establish distribution of the complete Next.js package.

`@cloudflare/vite-plugin` 1.37.1은 빌드·미리보기 도구이며, 생성한 Worker wrapper는 기존 서버 산출물에서 확인했습니다. 플러그인 전체가 런타임에 배포된다고 단정하지 않습니다. 해당 버전의 [MIT 원문](third-party-licenses/dev-tools/cloudflare-vite-plugin-1.37.1-LICENSE-MIT.txt)은 개발 도구 고지와 공유합니다. `drizzle-orm` 0.45.2는 설치되어 있지만 현행 서버 import 경로와 기존 번들에서 포함 근거를 확인하지 못해 실행 포함 목록에 넣지 않았습니다. 도달하지 않는 기본 UI 구성요소와 그 의존성도 설치만으로 목록에 추가하지 않았습니다.

`@cloudflare/vite-plugin` 1.37.1 is a build/preview tool; its generated Worker wrapper was found in the existing server output. This does not establish runtime distribution of the entire plugin. Its versioned [MIT text](third-party-licenses/dev-tools/cloudflare-vite-plugin-1.37.1-LICENSE-MIT.txt) is shared with the development notices. Installed `drizzle-orm` 0.45.2 was not included in the runtime list because its inclusion was not established by the current server import paths or existing bundles. Unreached starter UI components and their dependencies were not added solely because they are installed.

## 선택한 UI의 전이 의존성 / Transitive UI dependencies

현행 소스의 Radix 사용은 Dialog, AlertDialog, Progress, Slot, Popover입니다. 해당 모듈의 실제 import/re-export 경로를 따라 아래 의존성을 확인했습니다. 모든 Radix 컴포넌트나 모든 설치 패키지가 포함된다는 뜻은 아닙니다. 선언만 있고 조사한 모듈에서 도달하지 않은 @radix-ui/react-use-rect 및 @radix-ui/rect는 제외했습니다.

The current Radix imports use Dialog, AlertDialog, Progress, Slot and Popover. The following list follows their actual module import/re-export paths. It does not claim that every Radix component is shipped. Metadata-only candidates @radix-ui/react-use-rect and @radix-ui/rect are excluded.

| 구성요소 | 버전 | 라이선스 | 확인 범위 |
|---|---|---|---|
| [@floating-ui/core](third-party-licenses/runtime/floating-ui-core-1.8.0.LICENSE) | 1.8.0 | MIT | 현행 import 경로; 최종 tree shaking 미확인 |
| [@floating-ui/dom](third-party-licenses/runtime/floating-ui-dom-1.8.0.LICENSE) | 1.8.0 | MIT | 현행 import 경로; 최종 tree shaking 미확인 |
| [@floating-ui/react-dom](third-party-licenses/runtime/floating-ui-react-dom-2.1.9.LICENSE) | 2.1.9 | MIT | 현행 import 경로; 최종 tree shaking 미확인 |
| [@floating-ui/utils](third-party-licenses/runtime/floating-ui-utils-0.2.12.LICENSE) | 0.2.12 | MIT | 현행 import 경로; 최종 tree shaking 미확인 |
| [@radix-ui/primitive](third-party-licenses/runtime/radix-ui-primitive-1.1.7.LICENSE) | 1.1.7 | MIT | 현행 import 경로; 최종 tree shaking 미확인 |
| [@radix-ui/react-alert-dialog](third-party-licenses/runtime/radix-ui-react-alert-dialog-1.1.23.LICENSE) | 1.1.23 | MIT | 기존 번들 및 현행 사용 경로 |
| [@radix-ui/react-arrow](third-party-licenses/runtime/radix-ui-react-arrow-1.1.15.LICENSE) | 1.1.15 | MIT | 현행 import 경로; 최종 tree shaking 미확인 |
| [@radix-ui/react-compose-refs](third-party-licenses/runtime/radix-ui-react-compose-refs-1.1.5.LICENSE) | 1.1.5 | MIT | 현행 import 경로; 최종 tree shaking 미확인 |
| [@radix-ui/react-context](third-party-licenses/runtime/radix-ui-react-context-1.2.2.LICENSE) | 1.2.2 | MIT | 현행 import 경로; 최종 tree shaking 미확인 |
| [@radix-ui/react-dialog](third-party-licenses/runtime/radix-ui-react-dialog-1.1.23.LICENSE) | 1.1.23 | MIT | 기존 번들 및 현행 사용 경로 |
| [@radix-ui/react-dismissable-layer](third-party-licenses/runtime/radix-ui-react-dismissable-layer-1.1.19.LICENSE) | 1.1.19 | MIT | 기존 번들 및 현행 사용 경로 |
| [@radix-ui/react-focus-guards](third-party-licenses/runtime/radix-ui-react-focus-guards-1.1.6.LICENSE) | 1.1.6 | MIT | 기존 번들 및 현행 사용 경로 |
| [@radix-ui/react-focus-scope](third-party-licenses/runtime/radix-ui-react-focus-scope-1.1.16.LICENSE) | 1.1.16 | MIT | 기존 번들 및 현행 사용 경로 |
| [@radix-ui/react-id](third-party-licenses/runtime/radix-ui-react-id-1.1.4.LICENSE) | 1.1.4 | MIT | 현행 import 경로; 최종 tree shaking 미확인 |
| [@radix-ui/react-popover](third-party-licenses/runtime/radix-ui-react-popover-1.1.23.LICENSE) | 1.1.23 | MIT | 현행 import 경로; 최종 tree shaking 미확인 |
| [@radix-ui/react-popper](third-party-licenses/runtime/radix-ui-react-popper-1.3.7.LICENSE) | 1.3.7 | MIT | 현행 import 경로; 최종 tree shaking 미확인 |
| [@radix-ui/react-portal](third-party-licenses/runtime/radix-ui-react-portal-1.1.17.LICENSE) | 1.1.17 | MIT | 현행 import 경로; 최종 tree shaking 미확인 |
| [@radix-ui/react-presence](third-party-licenses/runtime/radix-ui-react-presence-1.1.10.LICENSE) | 1.1.10 | MIT | 현행 import 경로; 최종 tree shaking 미확인 |
| [@radix-ui/react-primitive](third-party-licenses/runtime/radix-ui-react-primitive-2.1.10.LICENSE) | 2.1.10 | MIT | 현행 import 경로; 최종 tree shaking 미확인 |
| [@radix-ui/react-progress](third-party-licenses/runtime/radix-ui-react-progress-1.1.16.LICENSE) | 1.1.16 | MIT | 기존 번들 및 현행 사용 경로 |
| [@radix-ui/react-slot](third-party-licenses/runtime/radix-ui-react-slot-1.3.3.LICENSE) | 1.3.3 | MIT | 기존 번들 및 현행 사용 경로 |
| [@radix-ui/react-use-callback-ref](third-party-licenses/runtime/radix-ui-react-use-callback-ref-1.1.4.LICENSE) | 1.1.4 | MIT | 현행 import 경로; 최종 tree shaking 미확인 |
| [@radix-ui/react-use-controllable-state](third-party-licenses/runtime/radix-ui-react-use-controllable-state-1.2.6.LICENSE) | 1.2.6 | MIT | 현행 import 경로; 최종 tree shaking 미확인 |
| [@radix-ui/react-use-effect-event](third-party-licenses/runtime/radix-ui-react-use-effect-event-0.0.5.LICENSE) | 0.0.5 | MIT | 현행 import 경로; 최종 tree shaking 미확인 |
| [@radix-ui/react-use-layout-effect](third-party-licenses/runtime/radix-ui-react-use-layout-effect-1.1.4.LICENSE) | 1.1.4 | MIT | 현행 import 경로; 최종 tree shaking 미확인 |
| [@radix-ui/react-use-size](third-party-licenses/runtime/radix-ui-react-use-size-1.1.4.LICENSE) | 1.1.4 | MIT | 현행 import 경로; 최종 tree shaking 미확인 |
| [aria-hidden](third-party-licenses/runtime/aria-hidden-1.2.6.LICENSE) | 1.2.6 | MIT | 기존 번들 및 현행 사용 경로 |
| [detect-node-es](third-party-licenses/runtime/detect-node-es-1.1.0.LICENSE) | 1.1.0 | MIT | 현행 import 경로; 최종 tree shaking 미확인 |
| [get-nonce](third-party-licenses/runtime/get-nonce-1.0.1.LICENSE) | 1.0.1 | MIT | 기존 번들 및 현행 사용 경로 |
| [react-remove-scroll](third-party-licenses/runtime/react-remove-scroll-2.7.2.LICENSE) | 2.7.2 | MIT | 기존 번들 및 현행 사용 경로 |
| [react-remove-scroll-bar](third-party-licenses/runtime/react-remove-scroll-bar-upstream.LICENSE) | 2.3.8 | MIT | 기존 번들; 2.3.8 원문 대응 미확인 |
| [react-style-singleton](third-party-licenses/runtime/react-style-singleton-2.2.3.LICENSE) | 2.2.3 | MIT | 현행 import 경로; 최종 tree shaking 미확인 |
| [tslib](third-party-licenses/runtime/tslib-2.8.1.LICENSE.txt) | 2.8.1 | 0BSD | 현행 import 경로; 최종 tree shaking 미확인 |
| [use-callback-ref](third-party-licenses/runtime/use-callback-ref-1.3.3.LICENSE) | 1.3.3 | MIT | 현행 import 경로; 최종 tree shaking 미확인 |
| [use-sidecar](third-party-licenses/runtime/use-sidecar-1.1.3.LICENSE) | 1.1.3 | MIT | 기존 번들 및 현행 사용 경로 |

## 원문 출처와 확인 제한 / License provenance

원문은 [외부 라이선스 폴더](third-party-licenses/)에 보존했습니다. 패키지별 공개 출처와 원문 SHA-256은 [런타임 원문 출처 목록](third-party-licenses/runtime/SOURCES.md)에서 확인할 수 있습니다. 설치 패키지의 원문 파일은 바이트를 변경하지 않았습니다. 별도 NOTICE 파일이 없는 패키지에 NOTICE 내용을 임의로 만들지 않았습니다.

- @vitejs/plugin-rsc 0.5.26의 원문은 [공식 해당 버전 태그](https://github.com/vitejs/vite-plugin-react/blob/plugin-rsc%400.5.26/LICENSE)에서 확보했습니다.
- @hiogawa/utils 1.7.0은 RSC 패키지의 내부 소스 표시와 서버 번들로 확인했습니다. [공식 저장소 원문](https://github.com/hi-ogawa/js-utils/blob/978a54938a661c389d7fe80b457eef2c2441ff08/LICENSE)을 보존했으며, 같은 공개 리비전의 패키지 메타데이터도 1.7.0/MIT입니다. npm 배포 압축파일 안의 LICENSE 바이트와의 일치는 별도로 확인하지 않았습니다.
- react-remove-scroll-bar 2.3.8의 설치 패키지는 MIT 메타데이터만 있고 LICENSE 파일이 없습니다. [공식 저장소 원문](https://github.com/theKashey/react-remove-scroll-bar/blob/master/LICENSE)을 참고용으로 보존했으나 조사한 공식 브랜치의 package.json은 2.3.7이므로 설치된 2.3.8에 대한 원문 대응은 아직 미확인입니다.

Installed license files are preserved byte-for-byte. The RSC adapter license comes from its exact official version tag. The @hiogawa/utils repository revision identifies version 1.7.0 and provides the preserved MIT text, but matching it to the published npm archive was not independently verified. The installed react-remove-scroll-bar 2.3.8 package lacks a license text; its official repository license is provided as a reference, and the reviewed repository metadata reports 2.3.7. Version-specific correspondence remains unverified.

## 관련 고지 / Related notices

이미지·아이콘·글꼴의 출처와 호스팅·외부 서비스 조건은 [자산·서비스 고지](ASSET_AND_SERVICE_NOTICES.md)를, 빌드·개발 도구는 [개발 도구 고지](DEV_TOOL_NOTICES.md)를 참고하십시오. 서비스 약관과 소프트웨어 라이선스는 별개입니다.

See [asset and service notices](ASSET_AND_SERVICE_NOTICES.md) for artwork, icons, fonts and hosting terms, and [development tool notices](DEV_TOOL_NOTICES.md) for build/development tools. Service terms and software licenses are separate.

## 실제 배포물에 필요한 후속 확인 / Deployment follow-up

이 소개 저장소의 고지만으로 실제 게임 배포물의 모든 라이선스 의무를 충족했다고 주장하지 않습니다. 운영 사이트는 이번 문서 작업에서 수정하거나 재배포하지 않았습니다.

실제 운영 브라우저·서버·정적 파일의 구성과 버전을 대조한 뒤, 포함된 외부 코드와 함께 필요한 저작권 표시 및 LICENSE 전문을 제공하고, 원래 NOTICE가 있다면 적용되는 NOTICE도 포함해야 합니다. MIT·ISC·Apache-2.0 등 각 조건에 맞게 제공 방식을 검증해야 합니다. 특히 CVA의 [Apache-2.0 원문](third-party-licenses/runtime/class-variance-authority-0.7.1.LICENSE)을 포함하고, 외부 파일을 수정하여 배포한다면 그 라이선스가 요구하는 변경 표시도 확인해야 합니다. react-remove-scroll-bar의 버전 대응과 최신 빌드의 정확한 모듈 목록도 보완 대상입니다.

These repository notices do not certify complete compliance of the live game distribution. The live site was not modified or redeployed for this documentation task. Compare the actual deployed inventory and versions, supply applicable copyright and full LICENSE texts with distributed copies, retain applicable upstream NOTICE content, and verify any required modification notices. The react-remove-scroll-bar version correspondence and exact module inventory of the latest build still need follow-up.
