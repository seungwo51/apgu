# Apgujeong Lounge SEO Files

생성일: 2026-06-03  
대상 사이트: `https://apgujeonglounge.kr`  
메인 키워드: **압구정 클럽**

이 문서는 `압구정 클럽` 메인 인덱스와 8개 서브 인덱스 키워드를 기준으로 재구성한 SEO 보조 파일의 적용 기준을 정리한 문서입니다.

## 1. 목적

본 구성의 목적은 Google 및 네이버 검색엔진이 사이트의 핵심 페이지를 명확히 발견, 크롤링, 색인할 수 있도록 하는 것입니다.

단, 본 파일 구성은 기술 SEO 기반 작업이며, 검색결과 최상단 노출을 보장하지 않습니다. 실제 순위는 본문 품질, 사용자 반응, 외부 링크, 경쟁 페이지 상태, 도메인 신뢰도, 색인 상태 등에 따라 달라집니다.

## 2. 생성 파일

| 파일명 | 역할 |
|---|---|
| `robots.txt` | 검색엔진 크롤러 접근 허용, sitemap/feed/rss 위치 안내 |
| `sitemap.xml` | 메인 및 서브 인덱스 URL을 검색엔진에 제출하기 위한 XML 사이트맵 |
| `feed.xml` | Atom 형식 피드맵 |
| `rss.xml` | RSS 2.0 형식 피드 |
| `README.md` | 마크다운 형식 적용 안내 문서 |
| `README.txt` | 일반 텍스트 형식 적용 안내 문서 |

## 3. 반영 URL 및 키워드

| URL | 타깃 키워드 | 구분 |
|---|---|---|
| `https://apgujeonglounge.kr/` | 압구정 클럽 | 메인 인덱스 |
| `https://apgujeonglounge.kr/apgujeong-club-lounge` | 압구정 클럽 라운지 | 서브 인덱스 |
| `https://apgujeonglounge.kr/apgujeong-club-recommend` | 압구정 클럽 추천 | 서브 인덱스 |
| `https://apgujeonglounge.kr/apgujeong-club-entry-denial` | 압구정 클럽 입뺀 | 서브 인덱스 |
| `https://apgujeonglounge.kr/apgujeong-club-entry-fee` | 압구정 클럽 입장료 | 서브 인덱스 |
| `https://apgujeonglounge.kr/apgujeong-club-review` | 압구정 클럽 후기 | 서브 인덱스 |
| `https://apgujeonglounge.kr/apgujeong-club-alone` | 압구정 클럽 혼자 | 서브 인덱스 |
| `https://apgujeonglounge.kr/apgujeong-club-guest` | 압구정 클럽 게스트 | 서브 인덱스 |
| `https://apgujeonglounge.kr/apgujeong-club-table` | 압구정 클럽 테이블 | 서브 인덱스 |

## 4. 루트 업로드 위치

아래 파일들은 모두 사이트 루트에 업로드해야 합니다.

```text
/robots.txt
/sitemap.xml
/feed.xml
/rss.xml
/README.md
/README.txt
```

예상 접근 경로는 다음과 같습니다.

```text
https://apgujeonglounge.kr/robots.txt
https://apgujeonglounge.kr/sitemap.xml
https://apgujeonglounge.kr/feed.xml
https://apgujeonglounge.kr/rss.xml
https://apgujeonglounge.kr/README.md
https://apgujeonglounge.kr/README.txt
```

## 5. robots.txt 구성 취지

`robots.txt`는 주요 검색엔진 크롤러의 접근을 허용하고, 검색엔진이 `sitemap.xml`, `feed.xml`, `rss.xml` 위치를 쉽게 확인할 수 있도록 구성했습니다.

반영 대상 크롤러는 다음을 포함합니다.

- Googlebot
- Googlebot-Image
- 네이버 Yeti
- Bingbot
- Daumoa

관리자 페이지나 비공개 경로가 없는 정적 사이트 기준으로 전체 크롤링을 허용하는 방식입니다.

## 6. sitemap.xml 구성 취지

`sitemap.xml`은 현재 실제 존재하는 메인 1개 및 서브 8개 URL만 포함합니다.

기존 ZIP 내부에서 확인된 과거 URL 또는 현재 HTML 구조와 불일치하는 URL은 제외했습니다.

제외 대상 예시는 다음과 같습니다.

```text
/apgujeong-club-guide/
/apgujeong-lounge-guide-2026/
/apgujeong-lounge-club-2026/
/apgujeong-club-recommendation-2026/
/apgujeong-lounge-table/
/apgujeong-club-entry-guide/
/apgujeong-rodeo-club-review/
```

## 7. feed.xml 및 rss.xml 구성 취지

`feed.xml`과 `rss.xml`은 검색엔진 및 외부 수집기가 사이트의 주요 페이지 구조를 더 쉽게 이해할 수 있도록 메인·서브 페이지별 제목, 링크, 설명, 카테고리 정보를 포함합니다.

각 피드는 다음 키워드를 기준으로 구성했습니다.

- 압구정 클럽
- 압구정 클럽 라운지
- 압구정 클럽 추천
- 압구정 클럽 입뺀
- 압구정 클럽 입장료
- 압구정 클럽 후기
- 압구정 클럽 혼자
- 압구정 클럽 게스트
- 압구정 클럽 테이블

## 8. 검색엔진 제출 절차

### Google Search Console

1. 사이트 속성 선택
2. `Sitemaps` 메뉴 이동
3. `sitemap.xml` 입력 후 제출
4. 주요 페이지 URL 검사
5. 색인 생성 요청

제출 예시:

```text
sitemap.xml
```

### 네이버 서치어드바이저

1. 사이트 등록 확인
2. `요청 > 사이트맵 제출` 메뉴 이동
3. `sitemap.xml` 제출
4. `요청 > RSS 제출` 메뉴 이동
5. `rss.xml` 제출
6. 주요 페이지 수집 요청

제출 예시:

```text
https://apgujeonglounge.kr/sitemap.xml
https://apgujeonglounge.kr/rss.xml
```

## 9. 배포 후 확인 항목

배포 후 브라우저에서 아래 URL이 정상적으로 열리는지 확인해야 합니다.

```text
https://apgujeonglounge.kr/robots.txt
https://apgujeonglounge.kr/sitemap.xml
https://apgujeonglounge.kr/feed.xml
https://apgujeonglounge.kr/rss.xml
```

확인 기준은 다음과 같습니다.

- 404 오류가 없어야 함
- XML 문법 오류가 없어야 함
- 잘못된 과거 URL이 남아 있지 않아야 함
- canonical URL과 sitemap URL이 충돌하지 않아야 함
- `robots.txt`에서 sitemap 위치가 정상 노출되어야 함

## 10. 추가 SEO 보완 권장사항

현재 기술 SEO 파일은 재구성되었으나, 상단 노출 가능성을 높이려면 다음 보완이 필요합니다.

1. 각 서브페이지의 meta description 구체화
2. 본문 내 검색 의도 보강
3. 메인에서 8개 서브페이지로 연결되는 내부링크 유지
4. 서브페이지 간 관련 링크 유지
5. 이미지 alt 문구를 실제 주제와 일치시키기
6. 블로그, SNS, 지도, 유튜브 등 외부 유입 신호 확보
7. Search Console과 네이버 서치어드바이저에서 색인 상태 주기 확인

## 11. 주의사항

- `sitemap.xml`은 검색엔진에 URL 발견을 돕는 파일이지, 상위 노출을 보장하는 파일이 아닙니다.
- `robots.txt`에서 허용하더라도 검색엔진이 모든 페이지를 반드시 색인하는 것은 아닙니다.
- URL 구조를 변경할 경우 `sitemap.xml`, `feed.xml`, `rss.xml`, canonical 태그를 함께 수정해야 합니다.
- HTML 파일의 canonical URL과 sitemap URL은 반드시 일치해야 합니다.
- 폐쇄된 페이지, 삭제된 페이지, 과거 URL은 sitemap에 넣지 않는 것이 원칙입니다.

## 12. 최종 적용 요약

이번 구성은 다음 기준으로 정리되었습니다.

```text
메인 인덱스: 압구정 클럽
서브 인덱스: 압구정 클럽 라운지
서브 인덱스: 압구정 클럽 추천
서브 인덱스: 압구정 클럽 입뺀
서브 인덱스: 압구정 클럽 입장료
서브 인덱스: 압구정 클럽 후기
서브 인덱스: 압구정 클럽 혼자
서브 인덱스: 압구정 클럽 게스트
서브 인덱스: 압구정 클럽 테이블
```

기존 잘못된 과거 URL은 배제하고, 현재 실제 HTML 구조와 키워드 대응 관계를 기준으로 SEO 보조 파일을 재구성했습니다.
