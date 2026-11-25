# 면책 고지 / Disclaimer

> **이 프로젝트는 개인 학습·개인 사용 목적의 비공식 도구입니다.**
> 株式会社メルカリ(Mercari, Inc.)와 관련이 없으며, 메루카리가 승인하거나 후원하지 않습니다.

## 한국어

### 1. 비공식 접근 방식과 약관 위반 가능성
- 이 도구는 jp.mercari.com 웹사이트가 내부적으로 사용하는 **비공개(문서화되지 않은) API**를 [`mercapi`](https://github.com/take-kun/mercapi) 라이브러리로 호출합니다. 메루카리가 개발자에게 공식 제공하는 API가 아닙니다.
- 메루카리 이용약관 제8조가 참조하는 가이드 「その他、不適切と判断される行為」에는 「弊社が提供するインターフェイスとは別の手法を用いてサービスにアクセスすること」가 금지 행위로 명시되어 있습니다. **이 도구를 사용하는 것만으로도 해당 조항에 위반될 수 있습니다.**
- 위반 시 메루카리는 계정 이용 제한, IP 차단 등의 조치를 취할 수 있으며(약관 제5조), 약관을 위반한 이용자는 손해배상 책임을 질 수 있습니다(약관 제24조).
- 약관과 가이드는 일본어 원문만 효력이 있으며, 언제든 개정될 수 있습니다. **사용 전에 최신 원문을 직접 확인하세요.**
  - 이용약관: https://static.jp.mercari.com/tos
  - 금지 행위 가이드: https://help.jp.mercari.com/guide/articles/900/

### 2. 이 도구가 하지 않는 것
위반 소지가 큰 기능은 의도적으로 넣지 않았습니다.
- 로그인, 계정 정보·쿠키 사용
- 구매, 출품, 좋아요, 댓글, 팔로우 등 **쓰기 동작 일체**
- 판매자 프로필·판매자별 상품 목록 조회 등 **개인 정보 수집**
- 대량 수집, 상시 크롤링, 결과 데이터의 저장·재배포
- 프록시·IP 순환, 키·식별자 순환 등 **차단 우회 기능**

> 참고: 요청에는 `mercapi` 라이브러리의 기본 User-Agent(일반 웹 브라우저 문자열)가 사용됩니다. 메루카리가 요청을 제한(HTTP 429·403)하면 도구는 우회를 시도하지 않고 중단합니다.

### 3. 사용 조건
- **개인적·비상업적 용도로만** 사용하세요. 사전 서면 허가 없이 서비스 밖에서 상업 목적으로 이용하는 것은 가이드에서 금지합니다.
- 기본 설정된 요청 간격 제한, 캐시, 페이지 수 상한을 **낮추거나 끄지 마세요.** 메루카리 서버에 부담을 주는 행위는 금지 행위에 해당합니다.
- HTTP 429·403 응답을 받으면 도구가 요청을 멈춥니다. 우회하려 하지 마세요.

### 4. 데이터 권리
- 검색 결과의 상품명, 설명, 이미지 등의 권리는 메루카리 또는 각 출품자에게 있습니다(약관 제21조).
- 결과는 개인 열람 용도로만 사용하고, 복제·게시·재배포하지 마세요. 캐시는 사용자 기기에만 짧은 기간 보관됩니다.

### 5. 책임 제한
- 이 소프트웨어는 [MIT 라이선스](./LICENSE)에 따라 **"있는 그대로(AS IS)"** 제공되며, 어떠한 보증도 하지 않습니다.
- 이 도구의 사용으로 발생하는 약관 위반, 계정 제한, 손해 등 **모든 결과의 책임은 사용자 본인**에게 있습니다.
- 이 문서는 법률 자문이 아닙니다.

### 6. 권리자 요청
메루카리 또는 권리자로부터 요청이 있으면 저장소를 즉시 비공개 처리하거나 삭제합니다. 연락은 GitHub Issues로 해 주세요.

---

## English

**Unofficial project for personal, non-commercial use. Not affiliated with, endorsed by, or sponsored by Mercari, Inc.**

1. **Unofficial access.** This tool calls the undocumented internal API used by the jp.mercari.com website, via the [`mercapi`](https://github.com/take-kun/mercapi) library. Mercari's prohibited-conduct guide (referenced by Article 8 of its Terms of Service) forbids "accessing the service by methods other than the interfaces provided by the company." **Using this tool may by itself violate Mercari's terms**, which can lead to account restrictions, IP blocking, or liability for damages (ToS Articles 5 and 24). Only the Japanese text of the terms is binding, and it may change at any time; read the current version before use.
2. **What this tool does not do.** No login or cookies; no write actions (purchase, listing, likes, comments, follows); no seller-profile or seller-inventory lookups; no bulk collection or redistribution; no proxy/IP rotation, key/identifier rotation, or other block-circumvention features. Requests use the default User-Agent of the `mercapi` library (a standard web-browser string); if Mercari limits requests (HTTP 429/403), the tool stops instead of retrying around the limit.
3. **Conditions of use.** Personal, non-commercial use only. Do not lower or disable the built-in rate limiting, caching, or page caps. The tool stops on HTTP 429/403; do not work around this.
4. **Data rights.** Listing content belongs to Mercari or the respective sellers (ToS Article 21). Do not copy, publish, or redistribute results.
5. **No warranty.** Provided "AS IS" under the [MIT License](./LICENSE). You are solely responsible for any consequences of using this tool. This is not legal advice.
6. **Takedown.** On request from Mercari or a rights holder, this repository will be made private or removed. Please open a GitHub Issue.
