# 자산·서비스 고지 / Asset and service notices

[전체 외부 구성요소 고지](THIRD_PARTY_NOTICES.md) · [한국어 소개](README.md) · [English guide](README.en.md)

검토 기준: 비경회기(祕境廻起) / Secret Realm Crawl **v0.1.0**, 2026-10-10. 최신 소스의 실제 사용, 자산 출처 기록, 설치된 해당 버전 라이선스, 기존 로컬 빌드를 읽기 전용으로 확인했습니다. 이 안내는 게임 코드·자산의 새 재사용 라이선스를 부여하지 않습니다.

## 현재 확인된 자산

| 자산 | 확인한 사용 및 권리 안내 | 원문·출처 |
|---|---|---|
| Lucide React 1.31.0 | 게임 UI의 SVG 아이콘. ISC가 적용되며 Feather에서 유래한 아이콘에는 원문에 포함된 MIT 고지도 적용됩니다. | [해당 버전의 전체 고지](third-party-licenses/assets/lucide-react-1.31.0.LICENSE), [공식 라이선스 안내](https://lucide.dev/license) |
| 직접 작성한 SVG 요소 | 일부 아이콘 도형. 작성자가 실제 보유한 권리만 유보하며, 결합된 Lucide 부분에는 외부 라이선스가 우선합니다. | [프로젝트 권리 안내](LICENSE) |
| AI 생성 배경 이미지 (`sect-landscape-v1.png`) | 현재 시작·지역 화면의 배경에 OpenAI 이미지 생성 도구로 만든 자료가 포함됩니다. 생성 사실만으로 오픈소스 라이선스나 모든 제삼자 권리를 포괄하는 독점 소유권이 생기지는 않습니다. | [OpenAI 이용약관](https://openai.com/policies/terms-of-use/), [서비스 약관](https://openai.com/policies/service-terms/) |
| 수련 도식 (`cultivation-meditation-brush-v3.png`) | 현재 게임의 수련 오버레이에서 사용합니다. 앞서 생성한 그림을 바탕으로 투명 이미지를 다시 생성했다는 기록은 있으나, 원본·후속 생성의 제공자와 적용 약관은 확인하지 못했습니다. 시제품 폴더에 있다는 이유로 미사용 자료로 분류하지 않습니다. | 생성 경위 확인; 제공자·적용 약관 추가 확인 필요 |
| 파비콘 (`favicon.svg`) | 현재 브라우저 아이콘으로 사용합니다. 최초 출처·권리 조건을 확정할 별도 기록을 확인하지 못했으므로, 직접 작성한 자산으로 단정하거나 외부 권리까지 소유한다고 주장하지 않습니다. | 출처·권리 조건 추가 확인 필요 |
| 시스템 글꼴 | 기기에 설치된 글꼴과 일반 폴백을 지정합니다. 확인한 소스·로컬 빌드에서 외부 웹폰트 다운로드나 폰트 파일 재배포의 증거는 찾지 못했습니다. 각 글꼴의 권리는 유지됩니다. | Arial, Apple SD Gothic Neo, Malgun Gothic, Batang, AppleMyungjo, Georgia 등 시스템 글꼴 |

## 빌드 지원 및 보존 자료

- **Sites Vite Plugin 0.2.0**: 사이트 빌드 지원 코드에 이 출처와 OpenAI의 MIT 고지가 명시되어 있습니다. [보존된 MIT 원문](third-party-licenses/assets/openai-sites-vite-plugin-0.2.0.LICENSE)을 제공합니다. 플러그인 소스 코드는 이 소개 저장소에 포함하지 않습니다.
- **shadcn Tailwind CSS 4.13.0**: 보존된 스타일시트의 [MIT 원문](third-party-licenses/assets/shadcn-tailwind-4.13.0.LICENSE)입니다. 최신 소스에서 직접 참조를 확인하지 못했으므로 현재 게임에 포함된 CSS라고 단정하지 않습니다. 설치된 `@shadcn/react` 패키지와는 별도 항목입니다.
- 위의 현재 사용 수련 도식과 별개로, 이전·시제품 이미지와 기본 SVG 일부의 최초 출처·재배포 권한은 완전히 확인하지 못했습니다. 현행 UI 참조를 찾지 못한 `dungeon.webp`, `file.svg`, `globe.svg`, `window.svg`도 검사한 기존 로컬 정적 빌드에는 포함되어 있습니다. 최신 운영 배포물에 남아 있다면 출처와 권한을 확인하거나, 별도 승인된 개발 작업에서 배포 대상 제외 여부를 검토해야 합니다. 이 저장소에는 그 이미지·SVG 파일을 복사하지 않았습니다.

## 서비스와 API

| 서비스 | 확인한 범위 | 약관 |
|---|---|---|
| ChatGPT Sites | 공식 게임 플레이 주소의 호스팅과 사이트 런타임. 무료 호스팅·무제한 사용을 주장하지 않습니다. | [ChatGPT Sites 약관](https://openai.com/policies/chatgpt-sites-terms/), [OpenAI 서비스 약관](https://openai.com/policies/service-terms/) |
| Cloudflare Workers / D1 | 서버 실행 및 저장 어댑터의 기반 기술. 직접 서비스 계약이나 무료·유료 티어는 확인하지 않았습니다. 개발 패키지 라이선스와 서비스 이용 조건은 별개입니다. | [Cloudflare 약관](https://www.cloudflare.com/terms/) — 기반 서비스 참고 |

검토한 소스에서 특정 **외부 무료 콘텐츠·AI API**를 게임 실행 중 호출한다는 증거는 찾지 못했습니다. 이미지 제작에 생성 도구를 사용한 것과 게임 실행 중 AI API를 연동한 것은 구별합니다. 전수 네트워크 검증은 수행하지 않았습니다.

## 배포물의 추가 확인

이 소개 저장소의 고지가 실제 게임 배포물의 라이선스 의무를 모두 충족한다는 보증은 아닙니다. 기존 로컬 빌드에서 Lucide·Feather·OpenAI의 원문 고지나 별도 LICENSE/NOTICE 파일은 발견되지 않았고, 해당 빌드와 최신 운영 배포물의 일치도 확인하지 못했습니다.

최신 배포물의 실제 포함 목록을 확인하고 필요한 저작권·LICENSE·NOTICE를 게임의 배포 파일과 함께 제공해야 합니다. 배포되는 라이선스 파일 묶음과 게임 안의 고지 링크를 통해 접근 가능 여부를 검증하는 방식으로 보완할 수 있습니다. 이번 작업은 운영 사이트를 수정하거나 배포하지 않았습니다.

## English summary

The v0.1.0 UI uses Lucide React 1.31.0 and some project-authored SVG icon elements. The version-specific Lucide notice above includes both ISC and Feather-derived MIT terms. The current start and region background, `sect-landscape-v1.png`, includes material generated with OpenAI image-generation tools; this does not itself grant an open-source license or establish exclusive ownership of all third-party rights. The current cultivation overlay uses `cultivation-meditation-brush-v3.png`, despite its prototype-folder location. Records describe a transparent regeneration from an earlier generated image, but the providers and applicable terms for both generations remain unverified. The browser uses `favicon.svg`; its original provenance and rights were not established, so it is not classified here as project-authored. The reviewed source and local build use system font families; no downloaded webfont or redistributed font-file evidence was found.

The preserved Sites Vite Plugin 0.2.0 notice is MIT. The preserved shadcn Tailwind CSS 4.13.0 notice is MIT, but current game inclusion was not established; it is separate from `@shadcn/react`. Apart from the currently used cultivation diagram above, provenance and redistribution rights for some retained legacy/prototype images and basic SVG files remain unverified if those files are deployed. `dungeon.webp`, `file.svg`, `globe.svg`, and `window.svg` have no current UI reference identified, but were included in the inspected older local static build; their presence in the latest live deployment was not verified.

Hosting through ChatGPT Sites and the use of Cloudflare Workers/D1 infrastructure are subject to service terms, separate from software licenses. Direct Cloudflare contracting and service pricing tiers were not established. No specific external free content or AI API was evidenced in the reviewed runtime source; a full network audit was not performed.

These repository notices do not certify compliance of the deployed game. Verify the current deployment inventory and include the required copyright, license, and notice texts with the actual game distribution, with working access from the game. The existing local build was not confirmed to match the live deployment. No production files or deployment were changed in this work.
