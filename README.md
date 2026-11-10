# 배포 사이트 올리는 법 (GitHub Pages + Releases)

## 1. 링크 3곳 바꾸기
`index.html`에서 계정(SAMOSLMO)과 저장소(samo)는 이미 채워져 있습니다.
- 다운로드 버튼 2개: `https://github.com/SAMOSLMO/samo/releases/latest/download/SAMO.zip`
- 업데이트 내역: `https://github.com/SAMOSLMO/samo/releases`

`[용량]`, `v[버전]` 같은 빈칸도 실제 값으로 채워 주세요.

## 2. 사이트 올리기 (GitHub Pages)
1. GitHub에서 Public 저장소를 새로 만듭니다.
2. 이 폴더 안의 내용(index.html, assets 폴더, .nojekyll)을 그대로 업로드합니다.
3. 저장소의 Settings → Pages → Source를 "Deploy from a branch"로 고르고, `main` / `(root)`를 선택한 뒤 저장합니다.
4. 1~2분 뒤 `https://samoslmo.github.io/samo/` 주소로 사이트가 열립니다.

## 3. 게임 파일 올리기 (Releases)
1. 저장소 오른쪽의 Releases → "Create a new release"를 누릅니다.
2. Tag를 `v1.0.0`처럼 입력합니다.
3. 빌드한 게임을 압축해서 **파일 이름을 반드시 `SAMO.zip`으로** 첨부합니다. 파일 하나는 2GB 미만이어야 합니다.
4. Publish를 누르면 사이트의 DOWNLOAD 버튼이 바로 이 파일을 받습니다.

새 버전을 낼 때는 같은 방법으로 새 Release를 만들고 `SAMO.zip`을 첨부하면 됩니다. 사이트는 따로 고치지 않아도 버튼이 자동으로 최신 버전을 가리킵니다.

## 파일 구성
- `index.html`: 페이지 본문
- `assets/css/style.css`: 디자인. PC, 태블릿, 모바일 반응형 포함
- `assets/img/`: 스탠딩, 카드, 스크린샷, 공유용 이미지(og_image.jpg), 파비콘
- `assets/fonts/`: SUIT 폰트

이미지를 바꾸고 싶으면 `assets/img/` 안의 파일을 **같은 이름으로** 덮어쓰면 됩니다.
