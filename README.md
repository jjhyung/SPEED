# SPEED Lab 웹사이트

국립부경대학교 제어계측공학전공 지능형 전력전자 연구실(SPEED Lab) 홈페이지입니다.
GitHub Pages에서 호스팅하는 정적 사이트이고, 서버는 없습니다. 내용(데이터)과 화면이 모두 `index.html` 파일 하나에 들어 있습니다.

## 폴더 구조
```
index.html                 사이트 본체 (내용 데이터 포함)
.nojekyll                  GitHub Pages 설정 파일 (지우지 마세요)
images/research_overview.png   Overview 페이지 연구 개요 그림
images/research1.png, research2.png   Research 페이지 연구 분야 그림
images/members/            교수·학생 사진
images/projects/           연구 과제 사진 (과제를 추가할 때 사용)
files/CV_Jun-Hyung_Jung.pdf    Professor 페이지 CV
files/lectures/            강의자료 PDF
```

## 처음 올리기 (GitHub Pages)
1. GitHub에 로그인한 뒤 오른쪽 위 **+ → New repository**를 누릅니다.
   - 이름 예: `SPEED` (주소는 `https://<계정>.github.io/SPEED/` 가 됩니다)
   - 계정 이름을 그대로 쓴 `<계정>.github.io` 로 만들면 주소가 `https://<계정>.github.io/` 가 됩니다.
   - **Public**으로 설정하고 **Create repository**를 누릅니다.
2. 새 저장소 화면에서 **uploading an existing file**을 누르고, 이 폴더의 **내용물 전체**(`index.html`, `.nojekyll`, `images`, `files`, `README.md`)를 끌어다 놓은 뒤 **Commit changes**를 누릅니다.
   - Windows 탐색기에서는 `.nojekyll`이 숨김 파일이라 안 보일 수 있습니다. 파일이 빠져도 사이트는 동작하지만, 올릴 수 있으면 함께 올려 주세요.
3. 저장소의 **Settings → Pages**로 가서 *Build and deployment* 항목을 설정합니다.
   - Source: **Deploy from a branch**
   - Branch: **main** / **/(root)** → **Save**
4. 1~2분 뒤 같은 화면 위쪽에 사이트 주소가 표시됩니다.

## 내용 수정하기 (관리자 모드)
1. 사이트 주소 뒤에 `#admin`을 붙여 접속합니다(예: `https://<계정>.github.io/SPEED/#admin`). 페이지에서 `Ctrl+Shift+A`를 눌러도 됩니다.
2. 점선으로 표시된 글자를 클릭하면 바로 고칠 수 있습니다. 위쪽 메뉴로 페이지를 옮겨 다니며 수정하면 됩니다.
   - `↑ ↓ ✕`로 항목의 순서를 바꾸거나 삭제하고, `+ 추가`로 새 항목을 만듭니다.
   - 한국어와 영어는 따로 저장됩니다. `EN` 버튼으로 언어를 바꾼 뒤 영어 내용도 고쳐 주세요.
3. 사진을 넣는 방법은 두 가지입니다.
   - **사진 선택**: 사진이 `index.html` 안에 함께 저장됩니다. 가장 간단한 방법입니다.
   - **경로 입력**: 예를 들어 `images/projects/nrf2027.jpg`처럼 경로를 적고, 같은 파일을 저장소의 해당 폴더에 올립니다.
4. 아래쪽의 **저장** 버튼을 누르면 새 `index.html`이 내려받아집니다.
5. GitHub 저장소에서 **Add file → Upload files**로 그 `index.html`을 올리고 **Commit**하면, 1~2분 뒤 사이트에 반영됩니다.

**자주 하는 수정**
- **연구 과제 추가** (Research 페이지): `+ 연구 과제 추가`를 누른 뒤 과제명, 발주기관, 기간, 요약을 적고, 상태(ongoing/completed/planned)를 고릅니다.
- **강의자료 추가** (Lecture 페이지): PDF를 저장소의 `files/lectures/` 폴더에 올린 뒤, 관리자 모드에서 해당 과목의 `+ 강의자료 추가`를 누르고 파일 경로를 `files/lectures/파일명.pdf`로 적습니다.
- **새 학기 추가**: `+ 학기 추가`를 누르고, 상태 글자를 "진행 중" 또는 "개설 예정"으로 적습니다.
- **구성원 추가** (Members 페이지): 해당 그룹에서 `+ 구성원 추가`를 누릅니다.
- **소식 추가** (News 페이지): `+ 소식 추가`를 누르면 새 소식이 맨 위에 생기고, Overview 페이지에는 최근 3건이 표시됩니다.
- **논문 추가** (Publications 페이지): 해당 연도에서 `+ 논문 추가`를 누릅니다. 새 연도가 필요하면 `+ 연도 추가`를 누르세요(맨 위에 생깁니다). 페이지 위쪽의 숫자 통계는 직접 고쳐야 합니다.

## 백업
- 관리자 바의 **데이터 백업(.json)** 으로 내용만 따로 저장할 수 있고, **백업 불러오기**로 되돌릴 수 있습니다.
- GitHub는 모든 파일의 수정 이력을 보관합니다. 잘못 올렸을 때는 저장소에서 `index.html`의 **History**를 열어 이전 버전으로 되돌릴 수 있습니다.
