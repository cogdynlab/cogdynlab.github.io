# Contributing to CogDyn Lab Website

## Editing workflow

1. Create a new branch.
2. Edit the relevant `.qmd` or `.bib` file.
3. Open a pull request.
4. Ask one lab member to review.
5. Merge after the Quarto build succeeds.

## Common files

- `people.qmd`: lab members
- `publications.bib`: publications
- `news.qmd`: lab news
- `join.qmd`: open positions
- `contact.qmd`: contact information

## Style

- Use English for public-facing pages.
- Use YYYY-MM-DD or Month YYYY consistently.
- Store images under `assets/`.
- Do not edit `_site/` directly.


index.qmd             첫 화면
research.qmd          연구 주제
people.qmd            구성원
publications.qmd      논문 페이지 레이아웃
publications.bib      논문 BibTeX 목록
projects.qmd          프로젝트, 코드, 데이터셋
news.qmd              랩실 소식
join.qmd              모집 안내
contact.qmd           주소, 이메일, 지도
_quarto.yml           메뉴, 사이트 제목, 기본 설정
assets/               로고, 사진, 스타일 파일

.qmd 파일 = 사람이 읽고 수정하는 페이지 원본
.bib 파일 = 논문 정보 원본
_site 폴더 = Quarto가 자동 생성하는 결과물
