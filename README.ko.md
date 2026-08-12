# Project Shield

[English](README.md)

AI 코더와 MCP 사용자를 위한 로컬 보안 스캐너입니다. 프로젝트와 AI 에이전트 설정에서 시크릿 노출, 개인정보, 안전하지 않은 MCP 설정, 프롬프트 인젝션, 위험한 Claude Code 훅을 점검합니다.

[![npm version](https://img.shields.io/npm/v/project-shield)](https://www.npmjs.com/package/project-shield)

## 무료로 실행하기

```bash
npx project-shield scan ./my-project
```

Project Shield v2.0.0은 로컬에서 실행되며 보안 등급, 수정 가이드, AI 코딩 환경 감사를 제공합니다.

## Free와 Pro 비교

| 기능 | Free | Pro |
|---|---:|---:|
| 프로젝트 스캔 | 월 5회 | 월 50회 |
| 환경 감사 | 월 3회 | 월 20회 |
| Fix-it 가이드 | 상위 3개 요약 | 전체 가이드와 코드·참조 |
| 배지 | 워터마크 | UUID·검증 URL이 포함된 클린 배지 |
| Evidence Pack | 미포함 | 무결성 봉인 JSON + PDF |
| 개인정보 발견 정보 | 개수만 | 파일과 줄 위치 |

Project Shield Pro는 **월 $29**이며 Polar의 자동 라이선스 키 혜택으로 제공됩니다.

결제 화면에는 Project Shield의 Polar 게시자 계정인 **Clouvel**이 표시됩니다. 적용되는 세금은 구매자의 청구 주소에 따라 Polar가 계산하여 결제 전에 보여줍니다.

- [Project Shield 제품 보기](https://shield.codemeant.dev)
- [Project Shield Pro 월 $29 구매](https://buy.polar.sh/polar_cl_eiXDc9bwtIpz99P8tjt3K1NZgS8oJN9WCwYIO1pgBDt)
- [npm 패키지 보기](https://www.npmjs.com/package/project-shield)

## 주요 명령

```bash
# 프로젝트 스캔
npx project-shield scan ./my-project

# 로컬 AI 코딩 환경 감사
npx project-shield audit

# Polar에서 받은 Pro 라이선스 활성화
project-shield activate PSH-XXXX-XXXX-XXXX-XXXX

# 라이선스 상태 확인
project-shield status
```

## Pro에서 제공되는 기능

- 코드 예제와 참조가 포함된 전체 Fix-it 가이드
- JSON 및 PDF Evidence Pack
- UUID와 검증 URL이 포함된 클린 배지
- 전체 Claude Code 환경 검사와 훅 분석
- 더 높은 월간 스캔·감사 한도

## 보안 안내

- 본인이 소유하거나 점검 권한이 있는 프로젝트에만 실행하세요.
- 코드나 설정을 바꾸기 전에 발견 내용을 직접 검토하세요.
- 공개 이슈에 시크릿이나 고객 데이터를 올리지 마세요.

## 라이선스

MIT
