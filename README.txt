업로드 및 SEO 보조 파일 안내

1. 이 패키지의 파일
- sitemap.xml : 검색엔진 제출용 사이트맵입니다. HTML 정규 URL만 포함했습니다.
- rss.xml : RSS 2.0 피드입니다. 네이버·일반 RSS 리더 호환성을 우선했습니다.
- feed.xml : Atom 1.0 피드입니다. 표준 Atom 구독기 및 일부 크롤러 호환용입니다.
- README.txt : 현재 파일입니다.

2. 권장 업로드 위치
아래 4개 파일을 도메인 루트에 업로드하십시오.

https://apgujeonglounge.kr/sitemap.xml
https://apgujeonglounge.kr/rss.xml
https://apgujeonglounge.kr/feed.xml
https://apgujeonglounge.kr/README.txt

3. URL 정책
이 패키지는 폴더/index.html 구조를 전제로 하여 서브페이지 정규 URL을 trailing slash 포함 형태로 통일했습니다.
예: https://apgujeonglounge.kr/apgujeong-club-guide/

현재 HTML 내부의 바로가기 href는 apgujeong-club-guide처럼 슬래시가 없는 상대경로입니다.
서버가 자동으로 /apgujeong-club-guide/로 보정하면 문제는 작지만, 가능하면 내부 링크도 아래처럼 맞추는 것이 좋습니다.

href="/apgujeong-club-guide/"
href="/apgujeong-lounge-guide-2026/"
href="/apgujeong-lounge-club-2026/"
href="/apgujeong-club-recommendation-2026/"
href="/apgujeong-lounge-table/"
href="/apgujeong-club-entry-guide/"
href="/apgujeong-rodeo-club-review/"

4. 메인 HTML head에 추가 권장
현재 index.html에는 sitemap 링크만 확인됩니다. RSS와 Atom을 검색엔진 및 브라우저가 명확히 발견하도록 다음 2줄을 head에 추가하십시오.

<link rel="alternate" type="application/rss+xml" title="APGUJEONG LOUNGE & CLUB RSS" href="/rss.xml">
<link rel="alternate" type="application/atom+xml" title="APGUJEONG LOUNGE & CLUB Atom" href="/feed.xml">

5. Search Console 제출
Google Search Console에는 아래 주소를 제출하십시오.
https://apgujeonglounge.kr/sitemap.xml

6. 운영상 주의사항
- lastmod는 실제 페이지 내용이 수정된 날짜로 유지해야 합니다. 이 파일은 현재 원본의 2026-05-17 기준 정보를 반영했습니다.
- 업장 운영 여부, 가격, 입장 기준은 변동 가능성이 큽니다. 실제 변경 시 HTML 본문, sitemap lastmod, RSS/Atom updated/pubDate를 함께 수정하십시오.
- 기존 파일에는 코어가 일부 문구에서 "오픈예정"으로 표시되고, 현재 메인 HTML에는 운영중 업장에 포함되는 불일치가 있었습니다. 본 패키지는 메인 HTML 기준에 맞춰 코어를 운영중 목록에 포함하는 방향으로 정리했습니다.
- 이미지 사이트맵에 기재된 /assets/*-hero.webp 파일은 실제 서버에 존재해야 합니다. 없는 경우 해당 image:image 항목을 삭제하거나 실제 파일명으로 교체하십시오.

7. 생성 기준
도메인: https://apgujeonglounge.kr/
페이지 기준일: 2026-05-17
피드 빌드일: 2026-05-26T09:00:00+09:00
