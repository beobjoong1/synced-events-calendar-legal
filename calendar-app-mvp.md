
## 3단계 — 달력을 9점으로 (2026-09-08 저녁, v1.14.0·v1.15.0)

- 위젯(Pro): 일간 보기(뷰 버튼 + 월 그리드의 날짜 숫자 클릭 → 그 날), 이벤트 검색창(`show-search`, 제목·장소·설명·캘린더명, 결과는 창 전체를 날짜별로 나열, 다른 해는 연도 표시), Wix Events RSVP 상태(`registration.status` → `rsvp: open|closed`, 열림이면 채워진 "RSVP / Register", 닫힘이면 "Registration closed"+Details). 위젯 렌더는 본문만 다시 그려서 검색창 포커스가 유지됨.
- 디자인: 스켈레톤 로딩, 포커스 링, 필은 왼쪽 색 막대, 오늘 표시 원형, 요일/날짜 머리글 소문자 대문자화, 상세 팝오버에 아이콘 메타 행, 좁은 폭에서 툴바 줄바꿈(v1.15.0에서 수정 — 모바일 스크린샷에서 Subscribe가 잘리는 걸 발견).
- 실측: 프리뷰·릴리스 호스트에서 월/일/검색/팝오버 렌더(데브 사이트 데이터), RSVP는 데브 사이트가 미게시라 이벤트 URL이 없어 URL을 주입해 버튼 렌더 확인(데이터의 `rsvp: 'open'`은 실측).
- 리스팅 스크린샷 5장 재생성(`calendar-app-assets/screenshot-*.png`, 로컬 dist를 CORS 서버로 띄워 `listing-page.html?mock=pro&script=…`), 공개 URL은 legal 저장소 `media/`(GitHub Pages).
- 남은 것: 데브센터 미디어 교체·App Info/요금제 문구 갱신(주간·일간 보기, 검색), 무료 체험 켜고 새 버전 제출.
- 리스팅 갱신(2026-09-08 저녁): 미디어 5장 교체(미디어 매니저 "Link (URL)" 가져오기 → GitHub Pages 이미지 → 각 타일 Replace → Add to Page; `input.files` 주입 업로드는 "URI is not a string" 오류로 0/5에서 멈춤), App Info 기능 2·3과 설명 마지막 문단에 일간 보기·검색·구독·RSVP 반영, Pro 혜택 "Week & day views, search, styling" / "Add-to-calendar, subscribe & RSVP", 무료 체험 14일 켬. 배포 페이지에서 "Publish market listing"으로 리스팅 변경 제출.
- 제출 결과: Distribute → "Publish market listing" → "Successfully published market listing", 사이드바에 "App submitted for review — 리뷰 중엔 새 변경 불가". 리스팅 변경은 즉시 반영된다는 확인 모달이 떴음(가격·앱 정보·미디어 포함).
